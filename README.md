# pstest: An R Package to assess the goodness of fit of parametric propensity score models.


This R package implements the specification tests proposed in Sant'Anna and
Song (2016), 'Specification Tests for the Propensity Score', available at
Pedro H.C. Sant'Anna webpage, http://sites.google.com/site/pedrohcsantanna/ .


In short, this package implement bootstrapped based Kolmogorov-Smirnov and Cramer-von Mises type tests for parametric propensity score models with either logistic ('logit'), or standard normal ('probit') link function.


The tests are based on the integrated conditional moment approach, where the weight function used is based on an orthogonal projection onto the tangent space of nuisance parameters. As a result, the tests enjoy improved power properties, do not suffer from the "curse of dimensionality" when the vector of covariates is of high-dimensionality, are fully data-driven, do not require tuning parameters such as bandwidths, and are able to detect a broad class of local alternatives converging to the null at the parametric rate. These appealing features highlight that the tests can be of great use in practice.


The module was written by Pedro H.C. Sant'Anna (Vanderbilt University) and Xiaojun Song (Peking University).

To install this package, you simply need to run the following two lines of code in R:

        library(devtools)
        install_github("pedrohcgs/pscore")


A help file with examples will be made available in the near future.
