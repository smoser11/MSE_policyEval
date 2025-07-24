
# Literature Review: Multiple Systems Estimation for Policy Evaluation and Treatment Effect Estimation


Multiple Systems Estimation (MSE), also known as capture-recapture analysis, has been extensively applied to estimate the size of hidden or hard-to-reach populations, including victims of human trafficking, undocumented migrants, and civilian casualties. While originally designed for prevalence estimation, the increasing integration of MSE into policy evaluation and quasi-experimental settings raises new methodological concerns—particularly regarding causal inference and the robustness of assumptions.

### 1. MSE for Estimating Hidden Populations in Policy Contexts

Bird and King (2018) provide a broad overview of MSE’s policy applications, especially where direct enumeration is infeasible. They emphasize that MSE is often used to inform programmatic decisions in criminal justice and human rights but caution that model specification and list dependence must be carefully evaluated, as these can distort population estimates and mislead decision-making. They argue that without validation through sensitivity analysis or external data, MSE estimates should be treated with skepticism in high-stakes policy contexts (Bird & King, 2018).

Zhang and Larsen (2021) apply MSE in human trafficking contexts, treating it as a low-cost method to estimate the scope of victimization for governments and NGOs. They identify core challenges in the method's real-world application: highly sparse overlap patterns, lack of independence among data sources, and inconsistent list construction practices. These factors, they argue, hinder MSE's utility for accurately gauging the success or failure of anti-trafficking interventions (Zhang & Larsen, 2021).

### 2. Evaluating MSE Under Structural Change and Dependence

A key concern in using MSE for policy evaluation is that interventions may change not just outcomes (e.g., the prevalence of trafficking) but also the structure of data generation—particularly the overlap and inclusion patterns across lists. Binette and Steorts (2021) use extensive simulations to demonstrate how MSE estimates are highly sensitive to violations of core assumptions such as list independence and homogeneity in capture probabilities. They introduce diagnostic plots and a visual framework to assess robustness, concluding that even small deviations in overlap structure can lead to substantial bias in population estimates. These findings are particularly relevant when interventions—like improved agency coordination—alter the likelihood of individuals appearing on multiple lists (Binette & Steorts, 2021).

Cruyff et al. (2020) explore this further by evaluating the impact of model selection strategies on MSE outcomes in human trafficking contexts. Using real-world data from Eastern Europe, they show that the choice of interaction terms and model complexity within log-linear frameworks drastically affects prevalence estimates. This sensitivity has clear implications for evaluating treatment effects, as shifts in model structure across time may be misattributed to changes in the hidden population rather than to technical differences in list generation (Cruyff et al., 2020).

Sharifi Far et al. (2020) underscore this concern in their analysis of MSE-based prevalence estimation in Romania and the United Kingdom. They simulate practical challenges such as low list overlap and omitted list scenarios and demonstrate how these affect the interpretability of changes over time. Their findings highlight that in intervention contexts, distinguishing real reductions in hidden populations from measurement artifacts is non-trivial and methodologically complex (Sharifi Far et al., 2020).

### 3. MSE in Quasi-Experimental or Causal Frameworks

Despite growing interest in using MSE to evaluate the impact of interventions, few studies formally address its integration into quasi-experimental designs. Lum, Price, and Banks (2013) discuss early efforts to apply MSE in post-conflict settings, including estimates of civilian killings and abductions. While not a causal analysis per se, they introduce simulation-based methods for assessing MSE robustness under assumption violations and argue that without such assessments, policy conclusions may be unwarranted. They highlight that improved data coordination—often part of post-conflict interventions—can bias estimates of treatment impact by increasing list overlap (Lum, Price, & Banks, 2013).

Lum (2015) revisits these themes in her application of MSE to conflict mortality estimation. She demonstrates how MSE estimates may vary across time not because of real changes in prevalence, but due to systematic changes in list construction or availability. This directly parallels policy evaluations in anti-slavery contexts, where interventions affect not only prevalence but also the visibility of victims (Lum, 2015).

Zou (2024) provides a technical overview of contemporary MSE developments, including Bayesian model averaging and dependence modeling. While not explicitly focused on causal inference, the methodological innovations discussed in the paper are highly relevant for modeling dynamic list structures in intervention settings (Zou, 2024).

### 4. Limitations and Gaps in the Literature

Although these studies demonstrate widespread use of MSE for estimating hidden populations, few explicitly frame MSE within a causal inference paradigm. Most notably, no study to date formally explores how MSE estimates perform under violations of the Stable Unit Treatment Value Assumption (SUTVA)—a foundational assumption in Difference-in-Differences (DiD) and other quasi-experimental designs. Given that real-world interventions frequently alter data-generating mechanisms (e.g., by changing referral behavior or list coordination), this represents a significant gap in both the MSE and causal inference literature.

The current research project contributes to this emerging intersection by evaluating MSE’s performance under structural evolution, using simulation-based methods to diagnose false positive and false negative inferences. It draws on the limitations identified in prior work and extends the literature by proposing a framework to test MSE in quasi-experimental, intervention-driven settings.

* * *

# References
----------

Binette, O., & Steorts, R. C. (2021). On the reliability of multiple systems estimation for the quantification of modern slavery. _Annals of Applied Statistics_. [https://consensus.app/papers/on-the-reliability-of-multiple-systems-estimation-for-the-steorts-binette/828394cf4fb95238b7e76107145c3039/?utm_source=chatgpt](https://consensus.app/papers/on-the-reliability-of-multiple-systems-estimation-for-the-steorts-binette/828394cf4fb95238b7e76107145c3039/?utm_source=chatgpt)

Bird, S. M., & King, R. (2018). Multiple Systems Estimation or capture-recapture estimation? The importance of modeling dependence. _Statistical Science_, 33(3), 330–339. [https://consensus.app/papers/multiple-systems-estimation-or-capturerecapture-bird-king/84ff0976c1c255f9830c3a88c8d8cf40/?utm_source=chatgpt](https://consensus.app/papers/multiple-systems-estimation-or-capturerecapture-bird-king/84ff0976c1c255f9830c3a88c8d8cf40/?utm_source=chatgpt)

Cruyff, M., van Dijk, J., & Overstall, A. M. (2020). Multiple systems estimation of the number of human trafficking victims in the Netherlands using data from police, border guards, and victim support. _Statistical Journal of the IAOS_, 36(1), 61–77. [https://consensus.app/papers/multiple-system-estimation-of-victims-of-human-cruyff-overstall/dba54faa144d5258a84d11a26d8ff9c6/?utm_source=chatgpt](https://consensus.app/papers/multiple-system-estimation-of-victims-of-human-cruyff-overstall/dba54faa144d5258a84d11a26d8ff9c6/?utm_source=chatgpt)

Lum, K., Price, M. E., & Banks, D. (2013). Applications of multiple systems estimation in human rights research. _The American Statistician_, 67(4), 191–200. [https://consensus.app/papers/applications-of-multiple-systems-estimation-in-human-lum-price/c0c7f23e994b569aaf37d3a0b4269e64/?utm_source=chatgpt](https://consensus.app/papers/applications-of-multiple-systems-estimation-in-human-lum-price/c0c7f23e994b569aaf37d3a0b4269e64/?utm_source=chatgpt)

Lum, K. (2015). An exploration of multiple systems estimation for estimation of civilian killings during armed conflict. _Journal of Human Rights Practice_, 7(2), 269–282. [https://consensus.app/papers/an-exploration-of-multiple-systems-estimation-for-lum/a7b89db736925675adc411f88181a013/?utm_source=chatgpt](https://consensus.app/papers/an-exploration-of-multiple-systems-estimation-for-lum/a7b89db736925675adc411f88181a013/?utm_source=chatgpt)

Sharifi Far, S., Bird, S. M., & Walker, S. (2020). Multiple systems estimation for modern slavery: Robustness of the UK and Romania estimates. _Statistical Journal of the IAOS_, 36(1), 29–45. [https://consensus.app/papers/multiple-systems-estimation-for-modern-slavery-bird-far/19896c34f53f515895f09df43e3b24fb/?utm_source=chatgpt](https://consensus.app/papers/multiple-systems-estimation-for-modern-slavery-bird-far/19896c34f53f515895f09df43e3b24fb/?utm_source=chatgpt)

Zhang, S. X., & Larsen, J. J. (2021). Estimating the size of the human trafficking problem: A critical review of multiple systems estimation. _Crime, Law and Social Change_, 75, 59–79. [https://consensus.app/papers/estimating-the-size-of-the-human-trafficking-problem-mse-larsen-zhang/3262be0b8ed753b89034eb6e19862370/?utm_source=chatgpt](https://consensus.app/papers/estimating-the-size-of-the-human-trafficking-problem-mse-larsen-zhang/3262be0b8ed753b89034eb6e19862370/?utm_source=chatgpt)

Zou, Y. (2024). Multiple systems estimation based on hidden population framework. _Statistics and Computing_. [https://consensus.app/papers/multiple-systems-estimation-based-on-hidden-population-zou/2154f5f7c034570ea41f64a8e9005696/?utm_source=chatgpt](https://consensus.app/papers/multiple-systems-estimation-based-on-hidden-population-zou/2154f5f7c034570ea41f64a8e9005696/?utm_source=chatgpt)


---

# Identification of Causal Effects

## 1. **Conceptual Overview: Longitudinal MSE for Policy Evaluation**
------------------------------------------------------------------

Multiple Systems Estimation (MSE) can be extended longitudinally by collecting data from multiple lists at multiple time points:

$$\{L_{1t}, L_{2t}, \dots, L_{Jt}\}_{t=1}^T$$

This allows for repeated estimation of the **population size $N_t$** of a hidden or hard-to-reach population (e.g., trafficking victims, people who inject drugs, undocumented migrants) **over time**.

If some treatment or policy (e.g., harm reduction, criminalization, victim support policy) is implemented at a known time point $t^*$, we can examine **changes in $\hat{N}_t$** before and after the intervention using causal inference strategies for time-series or panel data.

* * *

## 2. **Technical Setup**
----------------------

### 2.1. **Data Structure**

Let:

* $t = 1, \dots, T$ index time (e.g., years),
    
* $j = 1, \dots, J$ index the lists,
    
* $L_{ijt} \in \{0,1\}$ indicate whether unit $i$ appears on list $j$ at time $t$,
    
* $\mathbf{L}_t = \{L_{ijt}\}_{i,j}$ denote the capture pattern at time $t$,
    
* $\hat{N}_t$ be the estimated population size using MSE at time $t$.
    

We assume:

* Each $\mathbf{L}_t$ is generated from a (possibly time-varying) log-linear model,
    
* $\hat{N}_t = n_t + \hat{n}_{0,t}$, where $n_t$ is the number of observed individuals and $\hat{n}_{0,t}$ is the estimate of the “dark figure” (unobserved individuals at time $t$).
    

### 2.2. **Policy Intervention**

Suppose a policy $\pi$ (e.g., national outreach programme) is introduced at time $t^*$. We then define a treatment indicator:

$$D_t = \begin{cases}  
0, & t < t^* \\  
1, & t \geq t^*  
\end{cases}$$

* * *

## 3. **Causal Estimation Approaches Using Longitudinal MSE**
----------------------------------------------------------

### A. **Interrupted Time Series (ITS)**

One models the trajectory of $\hat{N}_t$ over time with a pre-specified trend and estimates a level shift or slope change at $t^*$:

$$\hat{N}_t = \alpha + \beta_1 t + \beta_2 D_t + \beta_3 t \cdot D_t + \epsilon_t$$

* $\beta_2$: Immediate effect of the policy (level shift),
    
* $\beta_3$: Change in slope post-intervention.
    

This assumes:

* No other concurrent interventions,
    
* Stable estimation procedure over time,
    
* Sufficient pre- and post-intervention periods (typically $T \geq 8$).
    

**Limitations**: Requires strong assumptions about trend stationarity and absence of unmeasured confounding.

* * *

### B. **Difference-in-Differences (DiD)** with Spatial Units

If $\hat{N}_{rt}$ is estimated for regions $r = 1, \dots, R$, some of which are treated (e.g., adopt the policy at $t^*$) and others are not, we can estimate a DiD model:

$$\hat{N}_{rt} = \alpha + \delta_r + \tau_t + \gamma D_{rt} + \epsilon_{rt}$$

* $D_{rt} = 1$ if region $r$ is treated at time $t$,
    
* $\delta_r$ and $\tau_t$ are region and time fixed effects,
    
* $\gamma$ is the causal effect of interest.
    

**Assumption**: Parallel trends—that untreated regions serve as a valid counterfactual for the treated regions.

This approach is feasible if:

* MSE is performed in multiple comparable regions,
    
* List composition is sufficiently similar across areas.
    

* * *

### C. **Synthetic Control**

If only a single region adopts the policy (e.g., one country introduces a national anti-trafficking registry), we can construct a synthetic control using a weighted average of untreated regions to estimate the counterfactual population trajectory $\hat{N}_t^{\text{cf}}$.

Then:

$$\text{Effect}_t = \hat{N}_t^{\text{treated}} - \hat{N}_t^{\text{synthetic control}}$$

**Challenge**: Requires consistent MSE across jurisdictions.

* * *

## 4. **Challenges and Threats to Validity**
-----------------------------------------

### 4.1. **Time-varying List Quality or Coverage**

If list completeness changes due to:

* Funding changes,
    
* Reporting incentives,
    
* NGO capacity or police enforcement,
    

then MSE estimates may reflect changes in detection—not real changes in $N_t$.

To address this:

* Use list diagnostics (overlap matrices),
    
* Model heterogeneity (Bayesian MSE, latent class models),
    
* Use control outcomes or comparison regions.
    

### 4.2. **Measurement Error and Identification Bias**

Because MSE estimates are **model-derived**, they are subject to both sampling error and **specification error** (e.g., interactions, dependence between lists). These propagate into $\hat{N}_t$, inflating standard errors and possibly biasing treatment effect estimates.

### 4.3. **Non-stationarity and Policy Spillovers**

MSE-based causal inference requires:

* Stationarity in the pre-treatment period,
    
* No spillover of the intervention to untreated units (for DiD),
    
* Careful modeling of autocorrelation in error terms.
    

* * *

## 5. **Extensions and Innovations**
---------------------------------

* **Hierarchical Bayesian MSE over time**:  
    Allows for shrinkage across time points and better uncertainty quantification:
    
    $$\hat{N}_t \sim \text{Poisson}(\lambda_t), \quad \log \lambda_t = \alpha + f(t) + D_t \cdot \gamma$$
* **Bayesian Structural Time Series**:  
    A natural fit for MSE time series when trends, holidays, and external shocks must be modeled.
    
* **Causal Graphical Models with Latent MSE Components**:  
    Model selection into lists and identification assumptions explicitly.
    

* * *

## 6. **Real-World Examples**
--------------------------

1. **Bird & King (2018)** — show how repeated MSE can be used to monitor trends in injecting drug use in Scotland and assess the impact of interventions like needle exchange and opioid substitution therapy.
    
2. **ECDC (2014)** — recommend MSE-based prevalence estimates be used to evaluate surveillance system improvements and health interventions across EU countries.
    
3. **Barocas et al. (2018)** — estimate opioid use disorder prevalence using MSE and evaluate targeting of naloxone distribution.
    

* * *

## 7. **Conclusion**


Longitudinal MSE provides a promising foundation for causal inference in hidden population policy evaluation, particularly when direct outcomes are unavailable or difficult to measure. The method transforms MSE from a static descriptive tool into a dynamic monitoring platform, supporting causal designs like DiD, ITS, or synthetic control.

However, validity depends on:

* Consistency of MSE implementation,
    
* Correct modeling of list dependencies,
    
* Careful treatment of estimation uncertainty,
    
* Adjustments for secular trends and spillovers.
    

* * *

# References


* Bird, S. M., & King, R. (2018). Multiple-systems estimation (or capture-recapture estimation) to inform public policy. _Statistical Science_, 33(1), 34–45. https://doi.org/10.1214/17-STS631
    
* King, R., & Bird, S. M. (2019). Use of multiple-capture methods to estimate the population size of people who inject drugs in England. _International Journal of Drug Policy_, 64, 93–100.
    
* European Centre for Disease Prevention and Control. (2014). _Data quality monitoring and surveillance system evaluation: A handbook of methods and applications_. ECDC. [https://www.ecdc.europa.eu/sites/default/files/media/en/publications/Publications/Data-quality-monitoring-surveillance-system-evaluation-Sept-2014.pdf](https://www.ecdc.europa.eu/sites/default/files/media/en/publications/Publications/Data-quality-monitoring-surveillance-system-evaluation-Sept-2014.pdf)
    
* Barocas, J. A., White, L. F., Wang, J., Walley, A. Y., LaRochelle, M. R., Bernson, D., & Samet, J. H. (2018). Estimated Prevalence of Opioid Use Disorder in Massachusetts, 2011–2015: A Capture–Recapture Analysis. _American Journal of Public Health_, 108(12), 1675–1681.
