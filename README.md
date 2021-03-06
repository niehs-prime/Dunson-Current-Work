# Dunson-Current-Work

Much of our work is ongoing across multiple repositories, so we have collected links and descriptions here:

**Bayesian Factor Analysis for Inference on Interactions**<br />
*Authors*: Federico Ferrari and David B. Dunson <br /> 
*Github*: https://github.com/fedfer/factor_interactions <br /> 
*ArXiv*: https://arxiv.org/abs/1904.11603 <br /> 
This article is motivated by the problem of inference on interactions among chemical exposures impacting human health outcomes. Chemicals often co-occur in the environment or in synthetic mixtures and as a result exposure levels can be highly correlated. We propose a latent factor joint model, which includes shared factors in both the predictor and response components while assuming conditional independence. By including a quadratic regression in the latent variables in the response component, we induce flexible dimension reduction in characterizing main effects and interactions. We propose a Bayesian approach to inference under this Factor analysis for INteractions (FIN) framework. Through appropriate modifications of the factor modeling structure, FIN can accommodate higher order interactions and multivariate outcomes. We provide theory on posterior consistency and the impact of misspecifying the number of factors. We evaluate the performance using a simulation study and data from the National Health and Nutrition Examination Survey (NHANES). Code is available on GitHub.

**Bayesian Sparse and Smooth Supervised Factor Analysis (bs3fa):** <br /> 
*Authors*: Kelly R. Moran and David B. Dunson <br /> 
*Github*: https://github.com/kelrenmor/bs3fa <br /> 
*ArXiv*: http://arxiv.org/abs/1912.12228 <br /> 
bs3fa is a package for Bayesian sparse and smooth supervised factor analysis. This model is appropriate for data in which you observe functional Y and numeric (continuous, binary, count) data X. The model assumes all variation in Y is explained by some low-dimensional factors eta, and these factors also explain part (but not all) of the variation in X. The bs3fa model is motivated by data from the ToxCast high throughput screening program. The article described the model and its application to an assay from the ToxCast database.


**Bayesian Factor Analysis and Postprocessing in R:** <br /> 
*Authors*: Evan Poworoznek, Federico Ferrari and David B. Dunson <br /> 
*Github*: https://github.com/poworoznek/sparse_bayesian_infinite_factor_models <br /> 
Bayesian latent factor models are key tools for modelling linear structure in data and performing dimension reduction. Recent advances in prior selection allow the posterior computation of semi- and non-parametric infinite factor models. These data-informed latent spaces show significant advantages in reproducibility and robustness in comparison to frequentist methods at the cost of computationally intensive sampling. We provide a package for the R programming environment with functions for sampling from the posterior distributions of several popular and recent factor models and priors with attractive properties for a wide class of inference.


**Nonparametric Bayesian multi-armed bandits for single cell experiment design** <br /> 
*Authors*: Federico Camerlenghi, Bianca Dumitrascu, Federico Ferrari, Barbara E. Engelhardt, Stefano Favaro  <br /> 
*Github*: https://github.com/fedfer/HPYsinglecell <br /> 
*ArXiv*: https://arxiv.org/abs/1904.11603 <br /> 
The problem of maximizing cell type discovery under budget constraints is a fundamental challenge in the collection and the analysis of single-cell RNA-sequencing (scRNA-seq) data. In this paper, we introduce a simple, computationally efficient, and scalable Bayesian nonparametric sequential approach to optimize the budget allocation when designing a large scale collection of scRNA-seq data for the purpose of, but not limited to, creating cell atlases. Our approach relies on i) a hierarchical Pitman-Yor prior that recapitulates biological assumptions regarding cellular differentiation, and ii) a Thompson sampling multi-armed bandit strategy that balances exploitation and exploration to prioritize experiments across a sequence of trials. Posterior inference is performed through a sequential Monte Carlo approach, which allows us to fully exploit the sequential nature of our species sampling problem. We empirically show that our approach outperforms state-of-the-art methods and achieves near-Oracle performance on simulated and real data alike. HPY-TS code is available at https://github.com/fedfer/HPYsinglecell.


**Identifying main effects and interactions among exposures using Gaussian processes** <br /> 
*Authors*: Federico Ferrari and David B. Dunson <br /> 
*Github*: https://github.com/fedfer/gp <br /> 
*ArXiv*: https://arxiv.org/abs/1911.01910 <br /> 
This article is motivated by the problem of studying the joint effect of different chemical exposures on human health outcomes. This is essentially a nonparametric regression problem, with interest being focused not on a black box for prediction but instead on selection of main effects and interactions. For interpretability, we decompose the expected health outcome into a linear main effect, pairwise interactions, and a non-linear deviation. Our interest is in model selection for these different components, accounting for uncertainty and addressing non-identifability between the linear and nonparametric components of the semiparametric model. We propose a Bayesian approach to inference, placing variable selection priors on the different components, and developing a Markov chain Monte Carlo (MCMC) algorithm. A key component of our approach is the incorporation of a heredity constraint to only include interactions in the presence of main effects, effectively reducing dimensionality of the model search. We adapt a projection approach developed in the spatial statistics literature to enforce identifiability in modeling the nonparametric component using a Gaussian process. We also employ a dimension reduction strategy to sample the non-linear random effects that aids the mixing of the MCMC algorithm. The proposed MixSelect framework is evaluated using a simulation study, and is illustrated using a simulation study and data from the National Health and Nutrition Examination Survey (NHANES). Code is available on GitHub.


**Bayesian Hierarchical Modelling of Functions** <br /> 
*Authors*: Bora Jin, David B. Dunson, and Amy H. Herring <br /> 
Motivated by the challenge of borrowing information for sparse functional data, we propose a Bayesian hierarchical framework for capturing changes in the expectation or variance of a functional response. In this framework, a latent variable approach is used to borrow information across exposures as well as across multivariate outcomes. We demonstrate the performance of these methods via extensive simulation studies and apply our approach to data from the EPA’s ToxCast program, in which sparse dose-response data are available for a plethora of chemicals and assay endpoints. Our methods allow more stable estimation of potential associations as shown for two key biological pathways: neurodevelopment and obesity. Extensive information about chemical structure is used to inform borrowing of information across chemicals and their ability to disrupt assay endpoints of interest, and the framework easily facilitates out-of-sample prediction of toxic potential for chemicals not yet assayed.


**Structural Equation Models for Environmental Health Outcomes** <br /> 
*Authors*: Melody Jiang, Federico Ferrari and David B. Dunson <br /> 
This work is motivated by the problem of inference on interactions among chemical exposures impacting multivariate human health outcomes. Typical analyses consider the effect of correlated chemical exposures on univariate quantities. However, data from environmental epidemiology studies usually contain multiple correlated measurements, like BMI, waist circumference and other body measures. We propose to use latent factor models both for the exposures and outcomes and we induce a multivariate regression via the latent variables. We propose a Bayesian approach to inference under this Structural Equation Model framework, which allows for joint modeling of multivariate outcomes while characterizing the covariance structure of both exposure measurements and dependent variables. We include a quadratic regression in the latent variables associated with the multivariate response and the latent variables associated with the predictor, which provides dimension reduction in characterizing main effects and interactions. With this specification we allow for shrinkage on the regression coefficients whenever the outcomes load on the same set of factors. We evaluate the performance using a simulation study and data from the National Health and Nutrition Examination Survey (NHANES). Code is available on GitHub. 

