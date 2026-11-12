# Robustness Profiles of Three Classification Algorithms Under Gaussian Noise in Test Features: A Controlled Case Study

**Author(s):** [ЗАПОВНИТИ ЗА РЕАЛЬНИМ ВНЕСКОМ]  
**Affiliation(s):** [ЗАПОВНИТИ]  
**Document status:** Educational manuscript example — NOT REVIEWED / NOT PUBLISHED  
**Source:** Results and Discussion v1.0, Sprint 6; experimental results from Sprint 4–5.

## Abstract

We examine how additive Gaussian noise in test features affects the classification performance of Logistic Regression, Random Forest, and Gradient Boosting. Three models are trained without artificial noise using a fixed train/test split of the Wine dataset, and independent Gaussian perturbations are added to standardized test features at four positive noise levels. We evaluate macro-F1, degradation relative to each model's clean reference, and variability across five fixed noise seeds. At the highest studied noise level (σ = 0.6), the mean degradation is 0.0339 for Logistic Regression, 0.0765 for Random Forest, and 0.1227 for Gradient Boosting. The observed degradation profiles differ across the three models, supporting the study hypothesis descriptively. The experiment provides a reproducible comparison of model behavior under the specified perturbation protocol.

**Keywords:** classification robustness; Gaussian noise; macro-F1; logistic regression; random forest; gradient boosting; reproducibility.

## 1. Introduction

Reliability under perturbed input data is an important consideration in classification systems. While predictive performance is often reported on unmodified test data, it does not directly describe how a fixed classifier behaves when feature measurements are distorted. This study compares the degradation profiles of three trained classification algorithms under a controlled test-time perturbation.

We ask how macro-F1 changes with noise intensity (RQ1), whether model-specific degradation profiles differ (RQ2), and how much the results vary across noise realizations (RQ3). Our hypothesis H1 is that the three algorithms exhibit different degradation profiles under the same experimental conditions.

## 2. Related Work

**[ПОТРІБНА ЗВІРКА З LITERATURE REVIEW MATRIX (SPRINT 2)]**: вставляємо 3–5 релевантних перевірених праць, конкретизуємо їхні методи, висновки й дослідницьку прогалину. *Це обов'язковий незавершений розділ навчального прикладу, а не готовий огляд.*

## 3. Materials and Methods

We used the `load_wine` classification dataset and a fixed train/test split. Numerical features were standardized using statistics estimated exclusively from the training set. Logistic Regression, Random Forest, and Gradient Boosting were tuned by cross-validation on clean training data using macro-F1; fitted models were then held fixed. Gaussian noise with zero mean and standard deviation σ was added to standardized test features at σ ∈ {0.1, 0.2, 0.4, 0.6}. Five prespecified seeds were used at each positive noise level, applying the same noise realization to every model within a (σ, seed) condition. Clean reference performance was evaluated once per model.

Performance Q(m,σ) was measured by macro-F1. Degradation was defined as D(m,σ) = Q(m,0) − Q(m,σ). We summarize results using means and sample standard deviations over the five noise realizations. The complete configuration, model hyperparameters, exact split and software versions are documented in the Experimental Protocol, code, and saved manifests. **[У ФІНАЛЬНОМУ РУКОПИСІ ДОДАТИ ТОЧНІ ПАРАМЕТРИ З АРТЕФАКТІВ]**.

## 4. Results

Mean macro-F1 did not increase with increasing noise on the investigated grid for any model. At σ = 0.6, the mean macro-F1 was 0.9661 for Logistic Regression, 0.9235 for Random Forest, and 0.8226 for Gradient Boosting.

| Model | Clean Q | Mean Q at σ=0.6 | Mean D at σ=0.6 | SD(D) at σ=0.6 |
|---|---:|---:|---:|---:|
| Logistic Regression | 1.0000 | 0.9661 | 0.0339 | 0.0232 |
| Random Forest | 1.0000 | 0.9235 | 0.0765 | 0.0314 |
| Gradient Boosting | 0.9453 | 0.8226 | 0.1227 | 0.0307 |

**Figure 1:** Mean macro-F1 against σ (`rq1_quality.png`).  
**Figure 2:** Mean degradation against σ (`rq2_degradation.png`).  
**Figure 3 (optional):** individual degradation realizations (`rq3_variability_*.png`).

## 5. Discussion

**RQ1.** Across the investigated levels, the mean macro-F1 profiles were non-increasing as noise increased. **RQ2.** The models differed in the magnitude of performance degradation; at σ=0.6, Logistic Regression had the smallest observed mean degradation and Gradient Boosting the largest. **RQ3.** Nonzero variability across five noise seeds indicates sensitivity to individual noise realizations. These findings are descriptively consistent with H1. No separate statistical test for between-model differences was included in the protocol.

**Literature comparison:** **[ДОДАТИ ПІСЛЯ ПЕРЕВІРКИ ДЖЕРЕЛ СПРИНТУ 2]**.

## 6. Limitations, Open Questions, Future Research

This case study uses one dataset and split, three fitted model configurations, one perturbation family, five fixed noise realizations per positive noise level, and descriptive hypothesis evaluation. Relevant open questions concern the impact of alternative model configurations, different types of perturbations, and changes in data characteristics. Follow-up research can vary hyperparameters, perturbation mechanisms, and datasets under separately specified protocols.

## 7. Conclusions

This controlled experiment documents different degradation profiles for three fixed classifiers under Gaussian perturbations of standardized test features. Logistic Regression showed the smallest mean performance loss and Gradient Boosting the largest at the highest tested noise intensity. Reporting both mean degradation and its across-seed variability helps characterize the observed behavior. The experimental artifacts and reproducibility audit provide a traceable basis for subsequent verification and extensions.

## Data and Code Availability

Source code and intermediate artifacts are held in the teaching research workspace (`Sprint_04`–`Sprint_06`, `research_artifacts/`). **[ВКАЗАТИ ПОГОДЖЕНУ ПУБЛІЧНУ АДРЕСУ, ЛІЦЕНЗІЮ ТА DOI ЛИШЕ ПІСЛЯ ФАКТИЧНОГО ОПРИЛЮДНЕННЯ]**.

## References

**[ПОТРІБНА ПЕРЕВІРЕНА БІБЛІОГРАФІЯ З MENDELEY; НЕ ВИГАДУВАТИ]**.
