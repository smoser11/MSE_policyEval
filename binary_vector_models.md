**Methodology**

We consider four distinct modeling strategies for the joint distribution over binary list-inclusion vectors \( \mathbf{Z}_i = (Z_{i1}, \ldots, Z_{iK}) \in \{0,1\}^K \), capturing various forms of dependence among the \( K \) lists. These include both exchangeable and non-exchangeable approaches and range from parametric to nonparametric Bayesian models.

---

**1. Log-linear Models (Frequentist & Bayesian)**

Log-linear models provide a flexible parametric framework for modeling dependence structures among binary vectors. Let \( \mathcal{Z} = \{0,1\}^K \) denote the space of binary vectors of length \( K \). The probability mass function of \( \mathbf{Z}_i \in \mathcal{Z} \) is modeled as:
\[
\mathbb{P}(\mathbf{Z}_i = \mathbf{z}) \propto \exp\left( \sum_{s \subseteq \{1, \ldots, K\}} \theta_s \prod_{k \in s} z_k \right),
\]
where the sum is over all subsets \( s \) of \( \{1, \ldots, K\} \), and \( \theta_s \in \mathbb{R} \) are interaction parameters. For example, \( \theta_{\{k\}} \) captures the marginal effect of list \( k \), while \( \theta_{\{k,\ell\}} \) quantifies the pairwise interaction between lists \( k \) and \( \ell \).

In the Bayesian setting, Gaussian priors \( \theta_s \sim \mathcal{N}(0, \sigma^2) \) can be placed on the interaction terms to induce regularization. Due to the exponential growth in the number of parameters (\( 2^K \)), these models are practical only for small \( K \). Computational inference can proceed via Markov Chain Monte Carlo (MCMC), often using data augmentation or Metropolis-Hastings steps.

---

**2. Exchangeable Binary Arrays with Finite Sufficient Statistics**

To mitigate the combinatorial burden of full log-linear modeling, we consider models where the probability of \( \mathbf{Z}_i \) depends only on low-dimensional sufficient statistics. Specifically, let:
\[
\mathbb{P}(\mathbf{Z}_i = \mathbf{z}) = f\left( \sum_{k=1}^K \alpha_k z_k + \sum_{k<\ell} \beta_{k\ell} z_k z_\ell \right),
\]
for some function \( f: \mathbb{R} \rightarrow \mathbb{R}_+ \), where \( \alpha_k \) are main effect parameters and \( \beta_{k\ell} \) encode symmetric pairwise interactions. This model retains parsimony by focusing only on low-order interactions and is naturally exchangeable across individuals \( i \), although not across dimensions \( k \).

Inference proceeds by choosing a parametric or semiparametric form for \( f(\cdot) \), such as exponential or logistic link functions, and fitting via MCMC or variational Bayes. This class of models can be viewed as generalizations of Ising models and belongs to the family of finite exchangeable binary arrays as discussed in Diaconis and Freedman (1980).

---

**3. Po\'lya-Gamma Augmented Multivariate Probit**

The multivariate probit model introduces correlation across binary indicators via latent Gaussian variables. Let \( \mathbf{X}_i = (X_{i1}, \ldots, X_{iK}) \sim \mathcal{N}(\boldsymbol{\mu}, \Sigma) \) denote a latent Gaussian vector, and define:
\[
Z_{ik} = \mathbb{I}(X_{ik} > 0), \quad k = 1, \ldots, K.
\]
This induces a joint distribution over \( \mathbf{Z}_i \in \{0,1\}^K \) where dependence among the \( Z_{ik} \) is encoded entirely in the covariance matrix \( \Sigma \). A P\'olya-Gamma augmentation (Polson et al., 2013) enables efficient Bayesian inference even for the multivariate probit case by transforming the probit link into a conditionally Gaussian form, making Gibbs sampling tractable.

Priors over \( \Sigma \) can be specified using the LKJ distribution for correlation matrices or inverse-Wishart priors for full covariance matrices. This model is parsimonious, interpretable, and suitable for moderate to large \( K \).

---

**4. Canonical Bayesian Nonparametric Model: Dirichlet Process Mixture of Product Bernoullis**

To allow flexible modeling without specifying a fixed number of latent classes, we employ a Dirichlet Process (DP) mixture model. Let each individual's binary vector \( \mathbf{Z}_i \) be generated conditionally independently given a latent parameter vector \( \boldsymbol{\theta}_i \):
\[
Z_{ik} \mid \boldsymbol{\theta}_i \sim \text{Bernoulli}(\theta_{ik}), \quad \boldsymbol{\theta}_i \sim G, \quad G \sim \text{DP}(\alpha, G_0),
\]
where \( G_0 \) is a base measure over \( [0,1]^K \), often taken as a product of independent Beta distributions: \( G_0 = \prod_{k=1}^K \text{Beta}(a, b) \).

Marginalizing over \( G \) induces clustering of individuals with similar list-inclusion profiles. Dependencies among list indicators are induced through the shared latent parameters \( \boldsymbol{\theta}_i \), even though the \( Z_{ik} \) are conditionally independent given \( \boldsymbol{\theta}_i \). Inference is typically performed using Chinese Restaurant Process (CRP) representations or stick-breaking constructions.

This model is exchangeable over individuals and highly flexible, adapting the complexity of the model to the observed data without requiring a fixed number of latent components.

---

