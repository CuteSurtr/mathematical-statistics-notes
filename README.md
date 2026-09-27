# Mathematical Statistics Notes

These are my notes on probability and mathematical statistics. The first half builds up the probability (random variables, the standard distributions, the central limit theorem) and then does estimation and hypothesis testing. The second half is the applied side: two-sample methods, chi-square tests, regression, ANOVA, block designs, and nonparametric tests.

The compiled book is [mathematical-statistics-notes.pdf](mathematical-statistics-notes.pdf), about 1,000 pages.

## Chapters

The chapter numbers start at 2; there is no Chapter 1.

2. Probability: sample spaces, the axioms, conditional probability and Bayes' rule, independence, counting.
3. Random variables: pmfs, densities and cdfs, expected value and variance, joint densities, transformations, order statistics, conditional densities, moment-generating functions.
4. Special distributions: Poisson, normal, geometric, negative binomial, and gamma, plus the normal approximation and the central limit theorem.
5. Estimation: maximum likelihood and the method of moments, confidence intervals, unbiasedness and efficiency, the Cramér-Rao bound, sufficiency, consistency, Bayesian estimation.
6. Hypothesis testing: decision rules, type I and type II errors, power and sample size, z and t tests for a mean, tests for a proportion and for a variance, likelihood ratio tests.
7. Inferences based on the normal distribution: the t distribution, sampling distributions, intervals and tests for a normal mean and variance, robustness and checking normality.
8. Types of data: measurement scales, experiments versus observational studies, sample structures, and picking the right procedure.
9. Two-sample inferences: the pooled and Welch t tests, paired data, the F test for two variances, comparing two proportions.
10. Goodness-of-fit tests: chi-square goodness of fit, contingency tables, and the tests of independence and homogeneity.
11. Regression: least squares, inference for the slope and intercept, confidence and prediction intervals, correlation, the ANOVA decomposition.
12. The analysis of variance: one-way ANOVA, multiple comparisons, contrasts, diagnostics.
13. Randomized block designs: the block model and its F test, the paired t test as a block design, efficiency and additivity.
14. Nonparametric statistics: the sign test, the Wilcoxon signed-rank and rank-sum tests, Kruskal-Wallis, Friedman, runs tests and rank correlation.

Every section opens with a short guide for telling which method a problem needs. Each rule is stated and justified and then used in worked examples, and every example says which rule applies and why before it solves the problem step by step. Each chapter ends with exercises and full solutions.

## Building the PDF

The book is `mathematical-statistics-notes.tex`, and the macros and plot styles are in `preamble.tex`. It builds with pdflatex on any recent TeX Live (it uses pgfplots for the density curves). Run it three times so the table of contents and the cross-references settle:

```bash
pdflatex mathematical-statistics-notes.tex
pdflatex mathematical-statistics-notes.tex
pdflatex mathematical-statistics-notes.tex
```
