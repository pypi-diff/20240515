# Comparing `tmp/preliz-0.6.2.tar.gz` & `tmp/preliz-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.6.2.tar` & `preliz-0.6.3.tar`

### file list

```diff
@@ -1,103 +1,104 @@
--rw-r--r--   0        0        0    11357 2024-05-09 16:13:24.830106 preliz-0.6.2/LICENSE
--rw-r--r--   0        0        0     4324 2024-05-09 16:13:24.830106 preliz-0.6.2/README.md
--rw-r--r--   0        0        0      649 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/__init__.py
--rw-r--r--   0        0        0     2772 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/__init__.py
--rw-r--r--   0        0        0     6930 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/asymmetric_laplace.py
--rw-r--r--   0        0        0     4977 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/bernoulli.py
--rw-r--r--   0        0        0     7804 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/beta.py
--rw-r--r--   0        0        0     6721 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/betabinomial.py
--rw-r--r--   0        0        0     7169 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/betascaled.py
--rw-r--r--   0        0        0     5368 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/binomial.py
--rw-r--r--   0        0        0     4730 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/categorical.py
--rw-r--r--   0        0        0     4302 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/cauchy.py
--rw-r--r--   0        0        0     7488 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/censored.py
--rw-r--r--   0        0        0     4135 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/chi_squared.py
--rw-r--r--   0        0        0    21635 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0     5071 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/discrete_uniform.py
--rw-r--r--   0        0        0     4942 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/discrete_weibull.py
--rw-r--r--   0        0        0    25870 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0     5946 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/exgaussian.py
--rw-r--r--   0        0        0     4397 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/exponential.py
--rw-r--r--   0        0        0     5941 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/gamma.py
--rw-r--r--   0        0        0     3987 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/geometric.py
--rw-r--r--   0        0        0     4489 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/gumbel.py
--rw-r--r--   0        0        0     3991 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/halfcauchy.py
--rw-r--r--   0        0        0     4920 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/halfnormal.py
--rw-r--r--   0        0        0     8033 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/halfstudentt.py
--rw-r--r--   0        0        0     5386 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/hurdle.py
--rw-r--r--   0        0        0     6141 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/hypergeometric.py
--rw-r--r--   0        0        0     6527 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/inversegamma.py
--rw-r--r--   0        0        0     4899 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/kumaraswamy.py
--rw-r--r--   0        0        0     4061 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/laplace.py
--rw-r--r--   0        0        0     3938 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/logistic.py
--rw-r--r--   0        0        0     5742 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/logitnormal.py
--rw-r--r--   0        0        0     5093 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/lognormal.py
--rw-r--r--   0        0        0     4710 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/moyal.py
--rw-r--r--   0        0        0     6104 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/negativebinomial.py
--rw-r--r--   0        0        0     5017 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/normal.py
--rw-r--r--   0        0        0     5070 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/pareto.py
--rw-r--r--   0        0        0     4265 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/poisson.py
--rw-r--r--   0        0        0     5851 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/rice.py
--rw-r--r--   0        0        0     6212 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/skewnormal.py
--rw-r--r--   0        0        0     7610 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/studentt.py
--rw-r--r--   0        0        0     6875 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/triangular.py
--rw-r--r--   0        0        0     5680 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/truncated.py
--rw-r--r--   0        0        0    14719 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/truncatednormal.py
--rw-r--r--   0        0        0     4692 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/uniform.py
--rw-r--r--   0        0        0     4987 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/vonmises.py
--rw-r--r--   0        0        0     5712 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/wald.py
--rw-r--r--   0        0        0     5152 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/weibull.py
--rw-r--r--   0        0        0     5601 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/zi_binomial.py
--rw-r--r--   0        0        0     7262 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/zi_negativebinomial.py
--rw-r--r--   0        0        0     5707 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/zi_poisson.py
--rw-r--r--   0        0        0       64 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4602 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0    13819 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/optimization.py
--rw-r--r--   0        0        0     5596 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/parser.py
--rw-r--r--   0        0        0    19087 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     9785 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0     2028 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/predictive_helper.py
--rw-r--r--   0        0        0    12000 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/special.py
--rw-r--r--   0        0        0     6565 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/ppls/pymc_io.py
--rw-r--r--   0        0        0      145 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14606 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     2251 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/ppe.py
--rw-r--r--   0        0        0     2160 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/predictive_explorer.py
--rw-r--r--   0        0        0     1946 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1787 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0   477854 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/ppa.ipynb
--rw-r--r--   0        0        0     2787 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/predictive_explorer.ipynb
--rw-r--r--   0        0        0     1439 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/quartile_int.ipynb
--rw-r--r--   0        0        0     1472 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0      661 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_beta_mode.py
--rw-r--r--   0        0        0     1967 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_censored.py
--rw-r--r--   0        0        0      757 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_dirichlet_mode.py
--rw-r--r--   0        0        0     1144 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_discrete_weibull.py
--rw-r--r--   0        0        0     7265 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      346 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_distributions_helper.py
--rw-r--r--   0        0        0      626 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_helper.py
--rw-r--r--   0        0        0     2292 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_hurdle.py
--rw-r--r--   0        0        0      338 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6654 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2919 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_mle.py
--rw-r--r--   0        0        0      987 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_optimization.py
--rw-r--r--   0        0        0     6153 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_plots.py
--rw-r--r--   0        0        0       85 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_ppa.py
--rw-r--r--   0        0        0      117 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_predictive_explorer.py
--rw-r--r--   0        0        0     3475 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      103 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_quartile_int.py
--rw-r--r--   0        0        0      910 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0    11083 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_scipy.py
--rw-r--r--   0        0        0     2287 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_special.py
--rw-r--r--   0        0        0     2568 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_truncated.py
--rw-r--r--   0        0        0      325 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     2244 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/beta_mode.py
--rw-r--r--   0        0        0     2341 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/dirichlet_mode.py
--rw-r--r--   0        0        0     4125 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1654 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3259 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     6136 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/quartile_int.py
--rw-r--r--   0        0        0    12994 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1559 2024-05-09 16:13:24.894106 preliz-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 preliz-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 19:06:31.789746 preliz-0.6.3/LICENSE
+-rw-r--r--   0        0        0     4324 2024-05-15 19:06:31.789746 preliz-0.6.3/README.md
+-rw-r--r--   0        0        0      649 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/__init__.py
+-rw-r--r--   0        0        0     2830 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0     6649 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/asymmetric_laplace.py
+-rw-r--r--   0        0        0     4977 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/bernoulli.py
+-rw-r--r--   0        0        0     7804 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/beta.py
+-rw-r--r--   0        0        0     6302 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/betabinomial.py
+-rw-r--r--   0        0        0     7169 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/betascaled.py
+-rw-r--r--   0        0        0     5368 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/binomial.py
+-rw-r--r--   0        0        0     4730 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/categorical.py
+-rw-r--r--   0        0        0     4302 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/cauchy.py
+-rw-r--r--   0        0        0     7502 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/censored.py
+-rw-r--r--   0        0        0     4135 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/chi_squared.py
+-rw-r--r--   0        0        0    21635 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0     5071 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/discrete_uniform.py
+-rw-r--r--   0        0        0     4942 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/discrete_weibull.py
+-rw-r--r--   0        0        0    25870 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0     5700 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/exgaussian.py
+-rw-r--r--   0        0        0     4397 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/exponential.py
+-rw-r--r--   0        0        0     5941 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/gamma.py
+-rw-r--r--   0        0        0     3987 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/geometric.py
+-rw-r--r--   0        0        0     4489 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/gumbel.py
+-rw-r--r--   0        0        0     3991 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/halfcauchy.py
+-rw-r--r--   0        0        0     4920 2024-05-15 19:06:31.845747 preliz-0.6.3/preliz/distributions/halfnormal.py
+-rw-r--r--   0        0        0     8033 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/halfstudentt.py
+-rw-r--r--   0        0        0     5386 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/hurdle.py
+-rw-r--r--   0        0        0     6040 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/hypergeometric.py
+-rw-r--r--   0        0        0     6527 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/inversegamma.py
+-rw-r--r--   0        0        0     4899 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/kumaraswamy.py
+-rw-r--r--   0        0        0     4061 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/laplace.py
+-rw-r--r--   0        0        0     3938 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/logistic.py
+-rw-r--r--   0        0        0     5742 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/logitnormal.py
+-rw-r--r--   0        0        0     5093 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/lognormal.py
+-rw-r--r--   0        0        0     4710 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/moyal.py
+-rw-r--r--   0        0        0     6104 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/negativebinomial.py
+-rw-r--r--   0        0        0     5017 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/normal.py
+-rw-r--r--   0        0        0     5070 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/pareto.py
+-rw-r--r--   0        0        0     4265 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/poisson.py
+-rw-r--r--   0        0        0     5851 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/rice.py
+-rw-r--r--   0        0        0     9518 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/skew_studentt.py
+-rw-r--r--   0        0        0     6598 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/skewnormal.py
+-rw-r--r--   0        0        0     7610 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/studentt.py
+-rw-r--r--   0        0        0     6953 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/triangular.py
+-rw-r--r--   0        0        0     5694 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/truncated.py
+-rw-r--r--   0        0        0    14787 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/truncatednormal.py
+-rw-r--r--   0        0        0     4692 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/uniform.py
+-rw-r--r--   0        0        0     4987 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/vonmises.py
+-rw-r--r--   0        0        0     5712 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/wald.py
+-rw-r--r--   0        0        0     5152 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/weibull.py
+-rw-r--r--   0        0        0     5601 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/zi_binomial.py
+-rw-r--r--   0        0        0     7262 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/zi_negativebinomial.py
+-rw-r--r--   0        0        0     5707 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/distributions/zi_poisson.py
+-rw-r--r--   0        0        0       64 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4667 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0    13819 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     5596 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/parser.py
+-rw-r--r--   0        0        0    19087 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     9785 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0     2028 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/predictive_helper.py
+-rw-r--r--   0        0        0    12204 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/internal/special.py
+-rw-r--r--   0        0        0     6565 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/ppls/pymc_io.py
+-rw-r--r--   0        0        0      145 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14606 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     2251 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/ppe.py
+-rw-r--r--   0        0        0     2160 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/predictive/predictive_explorer.py
+-rw-r--r--   0        0        0     1946 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1787 2024-05-15 19:06:31.849747 preliz-0.6.3/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0   477854 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/ppa.ipynb
+-rw-r--r--   0        0        0     2787 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/predictive_explorer.ipynb
+-rw-r--r--   0        0        0     1439 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/quartile_int.ipynb
+-rw-r--r--   0        0        0     1472 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0      661 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_beta_mode.py
+-rw-r--r--   0        0        0     1967 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_censored.py
+-rw-r--r--   0        0        0      757 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_dirichlet_mode.py
+-rw-r--r--   0        0        0     1144 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_discrete_weibull.py
+-rw-r--r--   0        0        0     7521 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      346 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_distributions_helper.py
+-rw-r--r--   0        0        0      626 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0     2292 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_hurdle.py
+-rw-r--r--   0        0        0      338 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6842 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     3387 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0      987 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_optimization.py
+-rw-r--r--   0        0        0     6153 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0       85 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_ppa.py
+-rw-r--r--   0        0        0      117 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_predictive_explorer.py
+-rw-r--r--   0        0        0     3557 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      103 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_quartile_int.py
+-rw-r--r--   0        0        0      910 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0    11197 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_scipy.py
+-rw-r--r--   0        0        0     2287 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_special.py
+-rw-r--r--   0        0        0     2568 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/tests/test_truncated.py
+-rw-r--r--   0        0        0      325 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/beta_mode.py
+-rw-r--r--   0        0        0     2341 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/dirichlet_mode.py
+-rw-r--r--   0        0        0     4125 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1654 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3259 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     6136 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/quartile_int.py
+-rw-r--r--   0        0        0    12994 2024-05-15 19:06:31.853747 preliz-0.6.3/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1559 2024-05-15 19:06:31.853747 preliz-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 preliz-0.6.3/PKG-INFO
```

### Comparing `preliz-0.6.2/LICENSE` & `preliz-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/README.md` & `preliz-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/__init__.py` & `preliz-0.6.3/preliz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.6.2/preliz/distributions/__init__.py` & `preliz-0.6.3/preliz/distributions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .laplace import Laplace
 from .logistic import Logistic
 from .logitnormal import LogitNormal
 from .lognormal import LogNormal
 from .moyal import Moyal
 from .normal import Normal
 from .pareto import Pareto
+from .skew_studentt import SkewStudentT
 from .skewnormal import SkewNormal
 from .studentt import StudentT
 from .rice import Rice
 from .triangular import Triangular
 from .truncatednormal import TruncatedNormal
 from .uniform import Uniform
 from .vonmises import VonMises
@@ -74,14 +75,15 @@
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
+    SkewStudentT,
     StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
```

### Comparing `preliz-0.6.2/preliz/distributions/asymmetric_laplace.py` & `preliz-0.6.3/preliz/distributions/asymmetric_laplace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numpy as np
 import numba as nb
 
 from .distributions import Continuous
 from ..internal.distribution_helper import all_not_none, eps
+from ..internal.optimization import optimize_ml
 
 
 class AsymmetricLaplace(Continuous):
     r"""
     Asymmetric-Laplace distribution.
 
     The pdf of this distribution is
@@ -174,17 +175,16 @@
 
     def _fit_moments(self, mean, sigma):
         # Assume symmetry
         mu = mean
         b = (sigma / 2) * (2**0.5)
         self._update(1, mu, b)
 
-    def _fit_mle(self, sample, **kwargs):
-        kappa, mu, b = nb_fit_mle(sample)
-        self._update(kappa, mu, b)
+    def _fit_mle(self, sample):
+        optimize_ml(self, sample)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_cdf(x, mu, b, kappa):
     x = (x - mu) / b
     kap_inv = 1 / kappa
     kap_kapinv = kappa + kap_inv
@@ -226,17 +226,7 @@
     sgn = np.sign(random_samples)
     return mu - (1 / (1 / b * sgn * kappa**sgn)) * np.log(1 - random_samples * sgn * kappa**sgn)
 
 
 @nb.njit(cache=True)
 def nb_entropy(b, kappa):
     return 1 + np.log(kappa + 1 / kappa) + np.log(b)
-
-
-@nb.njit(cache=True)
-def nb_fit_mle(sample):
-    new_mu = np.median(sample)
-    new_b = np.mean(np.abs(sample - new_mu))
-    new_kappa = np.sum((sample - new_mu) * np.sign(sample - new_mu)) / np.sum(
-        np.abs(sample - new_mu)
-    )
-    return new_kappa, new_mu, new_b
```

### Comparing `preliz-0.6.2/preliz/distributions/bernoulli.py` & `preliz-0.6.3/preliz/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/beta.py` & `preliz-0.6.3/preliz/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/betabinomial.py` & `preliz-0.6.3/preliz/distributions/betabinomial.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,24 +177,15 @@
     def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.binomial(
             n=self.n, p=random_state.beta(self.alpha, self.beta, size=size)
         )
 
     def _fit_moments(self, mean, sigma):
-        # Crude aproximation for n (as in Binomial distribution)
-        # For alpha and beta see:
-        # https://en.wikipedia.org/wiki/Beta-binomial_distribution#Method_of_moments
-        n = mean + sigma * 2
-        p = mean / n
-        rho = ((sigma**2 / (mean * (1 - p))) - 1) / (n - 1)
-        alpha = max(0.5, (p / rho) - p)
-        beta = max(0.5, (alpha / p) - alpha)
-        params = alpha, beta, n
-        optimize_moments(self, mean, sigma, params)
+        optimize_moments(self, mean, sigma)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, alpha, beta, n, lower, upper):
```

### Comparing `preliz-0.6.2/preliz/distributions/betascaled.py` & `preliz-0.6.3/preliz/distributions/betascaled.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/binomial.py` & `preliz-0.6.3/preliz/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/categorical.py` & `preliz-0.6.3/preliz/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/cauchy.py` & `preliz-0.6.3/preliz/distributions/cauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/censored.py` & `preliz-0.6.3/preliz/distributions/censored.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
         self.params = (*dist_params, self.lower, self.upper)
         self.param_names = (*self.dist.param_names, "lower", "upper")
         if all_not_none(*dist_params):
             self.dist._parametrization(**kwargs)
             self.is_frozen = True
 
         self.support = (
-            max(self.dist.support[0], self.lower),
-            min(self.dist.support[1], self.upper),
+            np.maximum(self.dist.support[0], self.lower),
+            np.minimum(self.dist.support[1], self.upper),
         )
         self.lower, self.upper = self.support
         self.params_support = (*self.dist.params_support, self.dist.support, self.dist.support)
 
     def mean(self):
         if self.kind == "discrete":
             p_low = self.dist.cdf(self.lower - 1)
```

### Comparing `preliz-0.6.2/preliz/distributions/chi_squared.py` & `preliz-0.6.3/preliz/distributions/chi_squared.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/continuous_multivariate.py` & `preliz-0.6.3/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/discrete_uniform.py` & `preliz-0.6.3/preliz/distributions/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/discrete_weibull.py` & `preliz-0.6.3/preliz/distributions/discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/distributions.py` & `preliz-0.6.3/preliz/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/distributions_multivariate.py` & `preliz-0.6.3/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/exgaussian.py` & `preliz-0.6.3/preliz/distributions/exgaussian.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
 from scipy.stats import skew
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, all_not_none
-from ..internal.special import erf, erfc, erfcx, mean_and_std
+from ..internal.special import erf, mean_and_std, norm_logcdf
 from ..internal.optimization import find_ppf
 
 
 class ExGaussian(Continuous):
     r"""
     Exponentially modified Gaussian (EMG) Distribution
 
@@ -139,28 +139,28 @@
         nus2 = (self.nu / self.sigma) ** 2
         opnus2 = 1.0 + nus2
         return 6.0 * nus2 * nus2 * opnus2 ** (-2)
 
     def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.normal(self.mu, self.sigma, size) + random_state.exponential(
-            1 / self.nu, size
+            self.nu, size
         )
 
     def _fit_moments(self, mean, sigma):
         # Just assume this is a approximately Gaussian
         self._update(mean, sigma, 1e-4)
 
     def _fit_mle(self, sample):
         mean, std = mean_and_std(sample)
-        skweness = skew(sample)
+        skweness = max(1e-4, skew(sample))
         nu = std * (skweness / 2) ** (1 / 3)
         mu = mean - nu
         var = std**2 * (1 - (skweness / 2) ** (2 / 3))
-        self._update(mu, var**0.5, 1 / nu)
+        self._update(mu, var**0.5, nu)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_cdf(x, mu, sigma, nu):
     cdf_n = 0.5 * (1 + erf((x - mu) / (sigma * 2**0.5)))
     if x == -np.inf:
         return 0
@@ -175,25 +175,16 @@
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, sigma, nu):
     if nu > 0.05 * sigma:
         return (
             -np.log(nu)
             + (mu - x) / nu
             + 0.5 * (sigma / nu) ** 2
-            + normal_lcdf(x, mu + (sigma**2) / nu, sigma)
+            + norm_logcdf((x - (mu + (sigma**2) / nu)) / sigma)
         )
     else:
         return -np.log(sigma) - 0.5 * np.log(2 * np.pi) - 0.5 * ((x - mu) / sigma) ** 2
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, sigma, nu):
     return -(nb_logpdf(x, mu, sigma, nu)).sum()
-
-
-@nb.vectorize(nopython=True, cache=True)
-def normal_lcdf(x, mu, sigma):
-    z_val = (x - mu) / sigma
-    if z_val < -1:
-        return np.log(erfcx(-z_val / 2**0.5) / 2) - abs(z_val) ** 2 / 2
-    else:
-        return np.log1p(-erfc(z_val / 2**0.5) / 2)
```

### Comparing `preliz-0.6.2/preliz/distributions/exponential.py` & `preliz-0.6.3/preliz/distributions/exponential.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/gamma.py` & `preliz-0.6.3/preliz/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/geometric.py` & `preliz-0.6.3/preliz/distributions/geometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/gumbel.py` & `preliz-0.6.3/preliz/distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/halfcauchy.py` & `preliz-0.6.3/preliz/distributions/halfcauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/halfnormal.py` & `preliz-0.6.3/preliz/distributions/halfnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/halfstudentt.py` & `preliz-0.6.3/preliz/distributions/halfstudentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/hurdle.py` & `preliz-0.6.3/preliz/distributions/hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/hypergeometric.py` & `preliz-0.6.3/preliz/distributions/hypergeometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,19 +162,15 @@
         )
 
     def rvs(self, size=None, random_state=None):
         random_state = np.random.default_rng(random_state)
         return random_state.hypergeometric(self.k, self.N - self.k, self.n, size=size)
 
     def _fit_moments(self, mean, sigma):
-        n = mean + sigma * 4
-        k = n
-        N = k * n / mean
-        params = N, k, n
-        optimize_moments(self, mean, sigma, params)
+        optimize_moments(self, mean, sigma)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, N, k, n, lower, upper):
```

### Comparing `preliz-0.6.2/preliz/distributions/inversegamma.py` & `preliz-0.6.3/preliz/distributions/inversegamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/kumaraswamy.py` & `preliz-0.6.3/preliz/distributions/kumaraswamy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/laplace.py` & `preliz-0.6.3/preliz/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/logistic.py` & `preliz-0.6.3/preliz/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/logitnormal.py` & `preliz-0.6.3/preliz/distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/lognormal.py` & `preliz-0.6.3/preliz/distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/moyal.py` & `preliz-0.6.3/preliz/distributions/moyal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/negativebinomial.py` & `preliz-0.6.3/preliz/distributions/negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/normal.py` & `preliz-0.6.3/preliz/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/pareto.py` & `preliz-0.6.3/preliz/distributions/pareto.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/poisson.py` & `preliz-0.6.3/preliz/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/rice.py` & `preliz-0.6.3/preliz/distributions/rice.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/skewnormal.py` & `preliz-0.6.3/preliz/distributions/skewnormal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
+from scipy.stats import skew  # pylint: disable=no-name-in-module
 from scipy.special import owens_t  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, to_precision, from_precision, all_not_none
-from ..internal.special import erf
-from ..internal.optimization import find_ppf, optimize_ml
+from ..internal.special import erf, norm_logcdf
+from ..internal.optimization import find_ppf, optimize_ml, optimize_moments
 
 
 class SkewNormal(Continuous):
     r"""
     SkewNormal distribution.
 
     The pdf of this distribution is
@@ -171,30 +172,41 @@
         u_0 = random_state.normal(size=size)
         v = random_state.normal(size=size)
         d = self.alpha / np.sqrt(1 + self.alpha**2)
         u_1 = d * u_0 + v * np.sqrt(1 - d**2)
         return np.sign(u_0) * u_1 * self.sigma + self.mu
 
     def _fit_moments(self, mean, sigma):
-        # Assume gaussian
-        self._update(mean, sigma, 0)
+        if self.alpha is None:
+            self.alpha = 0
+        optimize_moments(self, mean, sigma)
 
     def _fit_mle(self, sample):
+        skewness = skew(sample)
+        self.alpha = skewness / (1 - skewness**2) ** 0.5
         optimize_ml(self, sample)
 
 
 def nb_cdf(x, mu, sigma, alpha):
     return 0.5 * (1 + erf((x - mu) / (sigma * 2**0.5))) - 2 * owens_t((x - mu) / sigma, alpha)
 
 
-@nb.njit(cache=True)
+@nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, sigma, alpha):
-    return (
-        np.log1p(erf(((x - mu) * alpha) / np.sqrt(2 * sigma**2)))
-        - 0.5 * (x - mu) ** 2 / sigma**2
-        + np.log(1 / (sigma**2 * np.pi * 2.0)) / 2.0
-    )
+    if x == np.inf:
+        return -np.inf
+    elif x == -np.inf:
+        return -np.inf
+    else:
+        z_val = (x - mu) / sigma
+        return (
+            np.log(2)
+            - np.log(sigma)
+            - z_val**2 / 2.0
+            - np.log((2 * np.pi) ** 0.5)
+            + norm_logcdf(alpha * z_val)
+        )
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, sigma, alpha):
     return -(nb_logpdf(x, mu, sigma, alpha)).sum()
```

### Comparing `preliz-0.6.2/preliz/distributions/studentt.py` & `preliz-0.6.3/preliz/distributions/studentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/triangular.py` & `preliz-0.6.3/preliz/distributions/triangular.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 # pylint: disable=invalid-name
 import numpy as np
 import numba as nb
 
-from ..internal.optimization import optimize_ml
 from ..internal.distribution_helper import all_not_none
 from .distributions import Continuous
 
 
 class Triangular(Continuous):
     r"""
     Triangular distribution
@@ -168,15 +167,18 @@
         # Assume symmetry
         lower = mean - 6**0.5 * sigma
         upper = mean + 6**0.5 * sigma
         c = mean
         self._update(lower, c, upper)
 
     def _fit_mle(self, sample):
-        optimize_ml(self, sample)
+        lower = np.min(sample)
+        upper = np.max(sample)
+        middle = (np.mean(sample) * 3) - lower - upper
+        self._update(lower, middle, upper)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_cdf(x, lower, c, upper):
     if x <= lower:
         return 0
     elif lower < x <= c:
```

### Comparing `preliz-0.6.2/preliz/distributions/truncated.py` & `preliz-0.6.3/preliz/distributions/truncated.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         self.params = (*dist_params, self.lower, self.upper)
         self.param_names = (*self.dist.param_names, "lower", "upper")
         if all_not_none(*dist_params):
             self.dist._parametrization(**kwargs)
             self.is_frozen = True
 
         self.support = (
-            max(self.dist.support[0], self.lower),
-            min(self.dist.support[1], self.upper),
+            np.maximum(self.dist.support[0], self.lower),
+            np.minimum(self.dist.support[1], self.upper),
         )
         self.params_support = (*self.dist.params_support, self.dist.support, self.dist.support)
 
     def mean(self):
         x_values = self.xvals("full")
         pdf = self.pdf(x_values)
         if self.kind == "discrete":
```

### Comparing `preliz-0.6.2/preliz/distributions/truncatednormal.py` & `preliz-0.6.3/preliz/distributions/truncatednormal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numpy as np
 import numba as nb
 
-from ..internal.special import cdf_bounds, erf, erfinv, mean_and_std, ppf_bounds_cont
+from ..internal.special import cdf_bounds, erf, erfinv, ppf_bounds_cont
 from ..internal.optimization import optimize_ml
 from ..internal.distribution_helper import eps, all_not_none
 from .distributions import Continuous
 
 
 class TruncatedNormal(Continuous):
     r"""
@@ -124,127 +124,127 @@
 
     def entropy(self):
         return nb_entropy(self.mu, self.sigma, self.lower, self.upper)
 
     def mean(self):
         alpha = (self.lower - self.mu) / self.sigma
         beta = (self.upper - self.mu) / self.sigma
-        z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+        z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
         return (
             self.mu
             + (
                 (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * alpha**2))
                 - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * beta**2))
             )
-            / z
+            / z_val
             * self.sigma
         )
 
     def median(self):
         alpha = (self.lower - self.mu) / self.sigma
         beta = (self.upper - self.mu) / self.sigma
         inv_phi = 2**0.5 * erfinv(
             2 * ((0.5 * (1 + erf(alpha / 2**0.5)) + 0.5 * (1 + erf(beta / 2**0.5))) / 2) - 1
         )
         return self.mu + inv_phi * self.sigma
 
     def var(self):
         alpha = (self.lower - self.mu) / self.sigma
         beta = (self.upper - self.mu) / self.sigma
-        z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+        z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
         # Handle for -np.inf or np.inf
         psi_alpha = (0, 0) if alpha == -np.inf else (1, alpha)
         psi_beta = (0, 0) if beta == np.inf else (1, beta)
         return self.sigma**2 * (
             1
             - (
                 psi_beta[1] * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                 - psi_alpha[1] * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
             )
-            / z
+            / z_val
             - (
                 (
                     (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                     - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                 )
-                / z
+                / z_val
             )
             ** 2
         )
 
     def std(self):
         return self.var() ** 0.5
 
     def skewness(self):
         alpha = (self.lower - self.mu) / self.sigma
         beta = (self.upper - self.mu) / self.sigma
-        z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+        z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
         # Handle for -np.inf or np.inf
         psi_alpha = (0, 0) if alpha == -np.inf else (1, alpha)
         psi_beta = (0, 0) if beta == np.inf else (1, beta)
         numerator = (
             (
                 (psi_alpha[1] ** 2 - 1)
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                 * psi_alpha[0]
                 - (psi_beta[1] ** 2 - 1)
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                 * psi_beta[0]
             )
-            / z
+            / z_val
             - 3
             * (
                 psi_alpha[1]
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                 * psi_alpha[0]
                 - psi_beta[1]
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                 * psi_beta[0]
             )
             * (
                 (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                 - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
             )
-            / z**2
+            / z_val**2
             + 2
             * (
                 (
                     (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                     - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                 )
-                / z
+                / z_val
             )
             ** 3
         )
         denominator = (
             1
             + (
                 psi_alpha[1]
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                 * psi_alpha[0]
                 - psi_beta[1]
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                 * psi_beta[0]
             )
-            / z
+            / z_val
             - (
                 (
                     (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                     - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                 )
-                / z
+                / z_val
             )
             ** 2
         ) ** (3 / 2)
         return numerator / denominator
 
     def kurtosis(self):
         alpha = (self.lower - self.mu) / self.sigma
         beta = (self.upper - self.mu) / self.sigma
-        z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+        z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
         # Handle for -np.inf or np.inf
         psi_alpha = (0, 0) if alpha == -np.inf else (1, alpha)
         psi_beta = (0, 0) if beta == np.inf else (1, beta)
 
         numerator = (
             (
                 12
@@ -257,15 +257,15 @@
                     * psi_beta[0]
                 )
                 * (
                     (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                     - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                 )
                 ** 2
-                / z**3
+                / z_val**3
             )
             - (
                 4
                 * (
                     (psi_alpha[1] ** 2 - 1)
                     * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                     * psi_alpha[0]
@@ -273,70 +273,70 @@
                     * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                     * psi_beta[0]
                 )
                 * (
                     (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                     - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                 )
-                / z**2
+                / z_val**2
             )
             - (
                 3
                 * (
                     (
                         psi_alpha[1]
                         * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                         * psi_alpha[0]
                         - psi_beta[1]
                         * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                         * psi_beta[0]
                     )
-                    / z
+                    / z_val
                 )
                 ** 2
             )
             - (
                 6
                 * (
                     (
                         (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                         - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                     )
-                    / z
+                    / z_val
                 )
                 ** 4
             )
             + (
                 (psi_alpha[1] ** 3 - 3 * psi_alpha[1])
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                 * psi_alpha[0]
                 - (psi_beta[1] ** 3 - 3 * psi_beta[1])
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                 * psi_beta[0]
             )
-            / z
+            / z_val
         )
 
         denominator = (
             1
             + (
                 psi_alpha[1]
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2))
                 * psi_alpha[0]
                 - psi_beta[1]
                 * (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2))
                 * psi_beta[0]
             )
-            / z
+            / z_val
             - (
                 (
                     (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[0]
                     - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[0]
                 )
-                / z
+                / z_val
             )
             ** 2
         ) ** 2
 
         return numerator / denominator
 
     def rvs(self, size=None, random_state=None):
@@ -345,26 +345,25 @@
         return nb_rvs(random_samples, self.mu, self.sigma, self.lower, self.upper)
 
     def _fit_moments(self, mean, sigma):
         # Assume gaussian
         self._update(mean, sigma)
 
     def _fit_mle(self, sample):
-        mean, sigma = mean_and_std(sample)
-        self._update(mean, sigma, np.min(sample), np.max(sample))
+        self._update(None, None, np.min(sample), np.max(sample))
         optimize_ml(self, sample)
 
 
 @nb.njit(cache=True)
 def nb_cdf(x, mu, sigma, lower, upper):
     xi = (x - mu) / sigma
     alpha = (lower - mu) / sigma
     beta = (upper - mu) / sigma
-    z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
-    prob = (0.5 * (1 + erf(xi / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))) / z
+    z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+    prob = (0.5 * (1 + erf(xi / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))) / z_val
     return cdf_bounds(prob, x, lower, upper)
 
 
 @nb.njit(cache=True)
 def nb_ppf(q, mu, sigma, lower, upper):
     alpha = (lower - mu) / sigma
     beta = (upper - mu) / sigma
@@ -379,42 +378,44 @@
     return ppf_bounds_cont(inv_phi * sigma + mu, q, lower, upper)
 
 
 @nb.njit(cache=True)
 def nb_entropy(mu, sigma, lower, upper):
     alpha = (lower - mu) / sigma
     beta = (upper - mu) / sigma
-    z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+    z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
     # Handle for -np.inf or np.inf
     psi_alpha = (0, 0) if alpha == -np.inf else (1, alpha)
     psi_beta = (0, 0) if beta == np.inf else (1, beta)
-    return np.log((2 * np.pi * np.e) ** 0.5 * sigma * z) + (
+    return np.log((2 * np.pi * np.e) ** 0.5 * sigma * z_val) + (
         (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_alpha[1] ** 2)) * psi_alpha[1] * psi_alpha[0]
         - (1 / (2 * np.pi) ** 0.5 * np.exp(-0.5 * psi_beta[1] ** 2)) * psi_beta[1] * psi_beta[0]
-    ) / (2 * z)
+    ) / (2 * z_val)
 
 
 @nb.vectorize(nopython=True, cache=True)
 def nb_logpdf(x, mu, sigma, lower, upper):
     if x < lower or x > upper:
         return -np.inf
     else:
         xi = (x - mu) / sigma
         alpha = (lower - mu) / sigma
         beta = (upper - mu) / sigma
-        z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+        z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
         logphi = np.log(1 / (2 * np.pi) ** 0.5) - xi**2 / 2
-        return logphi - (np.log(sigma) + np.log(z))
+        return logphi - (np.log(sigma) + np.log(z_val))
 
 
 @nb.njit(cache=True)
 def nb_neg_logpdf(x, mu, sigma, lower, upper):
     return -(nb_logpdf(x, mu, sigma, lower, upper)).sum()
 
 
 @nb.njit(cache=True)
 def nb_rvs(random_samples, mu, sigma, lower, upper):
     alpha = (lower - mu) / sigma
     beta = (upper - mu) / sigma
-    z = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
-    inv_phi = 2**0.5 * erfinv(2 * (0.5 * (1 + erf(alpha / 2**0.5)) + random_samples * z) - 1)
+    z_val = 0.5 * (1 + erf(beta / 2**0.5)) - 0.5 * (1 + erf(alpha / 2**0.5))
+    inv_phi = 2**0.5 * erfinv(
+        2 * (0.5 * (1 + erf(alpha / 2**0.5)) + random_samples * z_val) - 1
+    )
     return inv_phi * sigma + mu
```

### Comparing `preliz-0.6.2/preliz/distributions/uniform.py` & `preliz-0.6.3/preliz/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/vonmises.py` & `preliz-0.6.3/preliz/distributions/vonmises.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/wald.py` & `preliz-0.6.3/preliz/distributions/wald.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/weibull.py` & `preliz-0.6.3/preliz/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/zi_binomial.py` & `preliz-0.6.3/preliz/distributions/zi_binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/zi_negativebinomial.py` & `preliz-0.6.3/preliz/distributions/zi_negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/distributions/zi_poisson.py` & `preliz-0.6.3/preliz/distributions/zi_poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/internal/distribution_helper.py` & `preliz-0.6.3/preliz/internal/distribution_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     "LogNormal": {"mu": 0.0, "sigma": 0.5},
     "LogitNormal": {"mu": 0.0, "sigma": 0.5},
     "Moyal": {"mu": 0.0, "sigma": 1.0},
     "Normal": {"mu": 0.0, "sigma": 1.0},
     "Pareto": {"alpha": 5, "m": 2.0},
     "Rice": {"nu": 2.0, "sigma": 1.0},
     "SkewNormal": {"mu": 0.0, "sigma": 1, "alpha": 6.0},
+    "SkewStudentT": {"mu": 0.0, "sigma": 1, "a": 2.0, "b": 2.0},
     "StudentT": {"nu": 7, "mu": 0.0, "sigma": 1},
     "Triangular": {"lower": -2, "c": 0.0, "upper": 2.0},
     "TruncatedNormal": {"mu": 0.0, "sigma": 1, "lower": -2, "upper": 3.0},
     "Uniform": {"lower": 0.0, "upper": 1.0},
     "VonMises": {"mu": 0.0, "kappa": 1.0},
     "Wald": {"mu": 1, "lam": 3.0},
     "Weibull": {"alpha": 5.0, "beta": 2.0},
```

### Comparing `preliz-0.6.2/preliz/internal/optimization.py` & `preliz-0.6.3/preliz/internal/optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/internal/parser.py` & `preliz-0.6.3/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/internal/plot_helper.py` & `preliz-0.6.3/preliz/internal/plot_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/internal/plot_helper_multivariate.py` & `preliz-0.6.3/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/internal/predictive_helper.py` & `preliz-0.6.3/preliz/internal/predictive_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/internal/special.py` & `preliz-0.6.3/preliz/internal/special.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,14 +487,23 @@
     if np.isinf(x):
         return 0
     else:
         return x * y
 
 
 @nb.vectorize(nopython=True, cache=True)
+def norm_logcdf(x):
+    t = x * 0.7071067811865476
+    if x < -1.0:
+        return np.log(erfcx(-t) / 2) - t * t
+    else:
+        return np.log1p(-erfc(t) / 2)
+
+
+@nb.vectorize(nopython=True, cache=True)
 def cdf_bounds(prob, x, lower, upper):
     if x < lower:
         return 0
     elif x >= upper:
         return 1
     else:
         return prob
```

### Comparing `preliz-0.6.2/preliz/ppls/pymc_io.py` & `preliz-0.6.3/preliz/ppls/pymc_io.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/predictive/ppa.py` & `preliz-0.6.3/preliz/predictive/ppa.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/predictive/ppe.py` & `preliz-0.6.3/preliz/predictive/ppe.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/predictive/predictive_explorer.py` & `preliz-0.6.3/preliz/predictive/predictive_explorer.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.6.3/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/plot_interactive.ipynb` & `preliz-0.6.3/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/ppa.ipynb` & `preliz-0.6.3/preliz/tests/ppa.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/predictive_explorer.ipynb` & `preliz-0.6.3/preliz/tests/predictive_explorer.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/quartile_int.ipynb` & `preliz-0.6.3/preliz/tests/quartile_int.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/roulette.ipynb` & `preliz-0.6.3/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_beta_mode.py` & `preliz-0.6.3/preliz/tests/test_beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_censored.py` & `preliz-0.6.3/preliz/tests/test_censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_dirichlet_mode.py` & `preliz-0.6.3/preliz/tests/test_dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_discrete_weibull.py` & `preliz-0.6.3/preliz/tests/test_discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_distributions.py` & `preliz-0.6.3/preliz/tests/test_distributions.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,29 +184,36 @@
                 0.8,
                 4.5,
             ),
         ),
     ],
 )
 def test_mle(distribution, params):
-    dist = distribution(*params)
-    sample = dist.rvs(20000)
-    dist_ = distribution()
-    dist_._fit_mle(sample)
+    for _ in range(10):
+        dist = distribution(*params)
+        sample = dist.rvs(20_000)
+        dist_ = distribution()
+        dist_._fit_mle(sample)
 
-    if dist.__class__.__name__ in ["Pareto", "ExGaussian"]:
-        tol = 0
+        if dist.__class__.__name__ in ["Pareto", "ExGaussian"]:
+            tol = 0
+        else:
+            tol = 1
+        try:
+            assert_almost_equal(dist.mean(), dist_.mean(), tol)
+            assert_almost_equal(dist.std(), dist_.std(), tol)
+            if dist.__class__.__name__ == "StudentT":
+                assert_almost_equal(params[1:], dist_.params[1:], 0)
+            else:
+                assert_almost_equal(params, dist_.params, 0)
+            break
+        except AssertionError:
+            pass
     else:
-        tol = 1
-    assert_almost_equal(dist.mean(), dist_.mean(), tol)
-    assert_almost_equal(dist.std(), dist_.std(), tol)
-    if dist.__class__.__name__ == "StudentT":
-        assert_almost_equal(params[1:], dist_.params[1:], 0)
-    else:
-        assert_almost_equal(params, dist_.params, 0)
+        raise AssertionError("Test failed after 10 attempts")
 
 
 @pytest.mark.parametrize("fmt", (".2f", ".1g"))
 @pytest.mark.parametrize("mass", (0.5, 0.95))
 def test_summary_args(fmt, mass):
     result = Normal(0, 1).summary(mass, fmt)
     assert result.mean == 0
```

### Comparing `preliz-0.6.2/preliz/tests/test_helper.py` & `preliz-0.6.3/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_hurdle.py` & `preliz-0.6.3/preliz/tests/test_hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_maxent.py` & `preliz-0.6.3/preliz/tests/test_maxent.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
+    SkewStudentT,
     StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
@@ -101,16 +102,18 @@
         (Normal(), 10, 12, 0.99, (-np.inf, np.inf), (11, 0.388)),
         (Normal(mu=0.5), -1, 1, 0.8, (-np.inf, np.inf), (0.581)),
         (Pareto(), 1, 4, 0.9, (1, np.inf), (1.660, 1)),
         (Pareto(m=2), 1, 4, 0.9, (2, np.inf), (3.321)),
         (Rice(), 0, 4, 0.7, (0, np.inf), (0, 2.577)),
         (Rice(), 1, 10, 0.9, (0, np.inf), (3.454, 3.734)),
         (Rice(nu=4), 0, 6, 0.9, (0, np.inf), (1.402)),
-        (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (4.061, 3.648, -0.021)),
+        (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (4, 3.647, 0)),
         (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.292, 4.903)),
+        (SkewStudentT(), -1, 1, 0.9, (-np.inf, np.inf), (-0.095, 0.52, 3.488, 3.112)),
+        (SkewStudentT(mu=0.7, sigma=0.4), -1, 1, 0.9, (-np.inf, np.inf), (2.004, 5.212)),
         (StudentT(), -1, 1, 0.683, (-np.inf, np.inf), (99.999, 0, 0.994)),
         (StudentT(nu=7), -1, 1, 0.683, (-np.inf, np.inf), (0, 0.928)),
         (
             Triangular(),
             0,
             4,
             0.8,
@@ -137,23 +140,23 @@
         (Uniform(), -2, 10, 0.9, (-2.666, 10.666), (-2.666, 10.666)),
         (VonMises(), -1, 1, 0.9, (-np.pi, np.pi), (0.0, 3.294)),
         (VonMises(mu=0.5), -1, 1, 0.9, (-np.pi, np.pi), (6.997)),
         (Wald(), 0, 10, 0.9, (0, np.inf), (5.061, 7.937)),
         (Wald(mu=5), 0, 10, 0.9, (0, np.inf), (7.348)),
         (Weibull(), 0, 10, 0.9, (0, np.inf), (1.411, 5.537)),
         (Weibull(alpha=2), 0, 10, 0.9, (0, np.inf), (6.590)),
-        (BetaBinomial(), 2, 8, 0.9, (0, 8), (1.951, 1.345, 8)),
-        (BetaBinomial(n=10), 2, 6, 0.6, (0, 10), (1.837, 2.181)),
+        (BetaBinomial(), 2, 8, 0.9, (0, 10), (4.945, 4.945, 10)),
+        (BetaBinomial(n=10), 2, 6, 0.6, (0, 10), (1.838, 2.181)),
         # # results for binomial are close to the correct result, but still off
         (Binomial(), 3, 9, 0.9, (0, 9), (9, 0.490)),
         (Binomial(n=12), 3, 9, 0.9, (0, 12), (0.612)),
         (DiscreteUniform(), -2, 10, 0.9, (-3, 11), (-2, 10)),
         (DiscreteWeibull(), 1, 6, 0.7, (0, np.inf), (0.939, 1.608)),
         (Geometric(), 1, 4, 0.99, (0, np.inf), (0.6837)),
-        (HyperGeometric(), 2, 14, 0.9, (0, 21), (56, 21, 21)),
+        (HyperGeometric(), 2, 14, 0.9, (0, 10), (50, 10, 20)),
         (NegativeBinomial(), 0, 15, 0.9, (0, np.inf), (7.573, 2.077)),
         (NegativeBinomial(p=0.2), 0, 15, 0.9, (0, np.inf), (1.848)),
         (Poisson(), 0, 3, 0.7, (0, np.inf), (2.763)),
         (ZeroInflatedBinomial(), 1, 10, 0.9, (0, 10), (0.902, 9.0, 0.485)),
         (ZeroInflatedBinomial(psi=0.7), 1, 10, 0.7, (0, 11), (10, 0.897)),
         (ZeroInflatedNegativeBinomial(), 2, 15, 0.8, (0, np.inf), (1.0, 9.862, 3.429)),
         (ZeroInflatedNegativeBinomial(psi=0.9), 2, 15, 0.8, (0, np.inf), (8.965, 6.174)),
```

### Comparing `preliz-0.6.2/preliz/tests/test_mle.py` & `preliz-0.6.3/preliz/tests/test_mle.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
+    SkewStudentT,
     StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
@@ -53,66 +54,81 @@
 @pytest.mark.parametrize(
     "distribution, params",
     [
         (AsymmetricLaplace, (2, 3, 1)),
         (Beta, (2, 5)),
         (BetaScaled, (2, 5, -1, 4)),
         (Cauchy, (0, 1)),
-        (ChiSquared, (1,)),
+        (ChiSquared, (5,)),
         (ExGaussian, (0, 1, 3)),
         (Exponential, (5,)),
         (Gamma, (2, 5)),
         (Gumbel, (0, 2)),
         (HalfCauchy, (1,)),
         (HalfNormal, (1,)),
-        (HalfStudentT, (3, 1)),
+        (HalfStudentT, (5, 1)),
         (HalfNormal, (2,)),
         (InverseGamma, (3, 5)),
         (Kumaraswamy, (2, 3)),
         (Laplace, (0, 2)),
         (Logistic, (0, 1)),
         (LogNormal, (0, 1)),
         (LogitNormal, (0, 0.5)),
         (Moyal, (0, 2)),
         (Normal, (0, 1)),
         (Pareto, (5, 1)),
         (Rice, (0, 2)),
-        (SkewNormal, (0, 1, 6)),
+        (SkewNormal, (0, 1, -6)),
+        (SkewStudentT, (0, 1, 2, 2)),
         (StudentT, (4, 0, 1)),
-        (Triangular, (0, 2, 4)),
-        (TruncatedNormal, (0, 1, -1, 1)),
+        (Triangular, (0, 3, 4)),
+        (TruncatedNormal, (0, 0.5, -1, 1)),
         (Uniform, (2, 5)),
         (VonMises, (1, 2)),
         (Wald, (2, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.5,)),
-        (BetaBinomial, (1, 2, 10)),
+        (BetaBinomial, (2, 5, 10)),
         (Binomial, (5, 0.5)),
         (DiscreteUniform, (-2, 2)),
         (DiscreteWeibull, (0.9, 1.3)),
         (Geometric, (0.75,)),
-        (HyperGeometric, (50, 20, 10)),
-        (NegativeBinomial, (10, 0.5)),
+        (HyperGeometric, (50, 10, 20)),
+        (NegativeBinomial, (10, 2.5)),
         (Poisson, (4.2,)),
-        (ZeroInflatedBinomial, (0.5, 10, 0.8)),
+        (ZeroInflatedBinomial, (0.5, 10, 0.6)),
         (ZeroInflatedNegativeBinomial, (0.7, 8, 4)),
         (
             ZeroInflatedPoisson,
             (
                 0.8,
                 4.2,
             ),
         ),
     ],
 )
 def test_auto_recover(distribution, params):
-    dist = distribution(*params)
-    sample = dist.rvs(10000)
-    pz.mle([distribution()], sample)
-    assert_allclose(dist.params, params, atol=1)
+    for _ in range(10):
+        sample = distribution(*params).rvs(10_000)
+        dist = distribution()
+        try:
+            if dist.__class__.__name__ in [
+                "BetaScaled",
+                "TruncatedNormal",
+            ]:
+                tol = 1
+            else:
+                tol = 0.1
+            pz.mle([dist], sample)
+            assert_allclose(dist.params, params, atol=tol)
+            break
+        except AssertionError:
+            pass
+    else:
+        raise AssertionError(f"Test failed after 10 attempts.{dist.params}")
 
 
 def test_recover_right():
     dists = [Normal(), Gamma(), Poisson()]
     sample = Normal(0, 1).rvs(10000)
     pz.mle(dists, sample)
     assert dists[0].__class__.__name__ == "Normal"
```

### Comparing `preliz-0.6.2/preliz/tests/test_optimization.py` & `preliz-0.6.3/preliz/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_plots.py` & `preliz-0.6.3/preliz/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_quartile.py` & `preliz-0.6.3/preliz/tests/test_quartile.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     Logistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
+    SkewStudentT,
     StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
@@ -68,14 +69,15 @@
         (Logistic(), -1, 0, 1, (0, 0.910)),
         (LogNormal(), 0.5, 1, 2, (0, 1.027)),
         (LogitNormal(), 0.3, 0.45, 0.6, (-0.212, 0.929)),
         (Moyal(), 0.5, 1, 2, (0.620, 0.567)),
         (Normal(), -1, 0, 1, (0, 1.482)),
         (Pareto(), 0.5, 1, 4, (0.541, 0.289)),
         (Rice(), 2, 4, 6, (0, 3.395)),
+        (SkewStudentT(), 2, 4, 6, (4, 2.648, 1.663, 1.663)),
         pytest.param(
             StudentT(),
             -1,
             0,
             1,
             (84576.43, 0, 1.482),
             marks=pytest.mark.skipif(
@@ -85,19 +87,19 @@
         (StudentT(nu=4), -1, 0, 1, (0, 1.350)),
         (Triangular(), 0, 1, 2, (-2.414, 1.0, 4.414)),
         (TruncatedNormal(), -1, 0, 1, (0, 1.482)),
         (Uniform(), -1, 0, 1, (-2, 2)),
         (VonMises(), -1, 0, 1, (0, 0.656)),
         (Wald(), 0.5, 1, 2, (1.698, 1.109)),
         (Weibull(), 0.5, 1, 2, (1.109, 1.456)),
-        (BetaBinomial(), 2, 5, 8, (1.182, 1.53, 13.0)),
+        (BetaBinomial(), 3, 5, 7, (2.323, 1.949, 10.0)),
         (DiscreteUniform(), -2, 0, 2, (-5, 5)),
         (DiscreteWeibull(), 2, 6, 7, (0.951, 1.487)),
         (Geometric(), 2, 4, 6, (0.17)),
-        (HyperGeometric(), 2, 3, 4, (26, 8, 8)),
+        (HyperGeometric(), 3, 4, 5, (50, 10, 20)),
         (NegativeBinomial(), 3, 5, 10, (7.283, 2.167)),
         (Poisson(), 4, 5, 6, (5.641)),
         (ZeroInflatedBinomial(), 1, 4, 7, (0.660, 10.947, 0.670)),
         (ZeroInflatedBinomial(psi=0.7), 2, 4, 6, (10.0, 0.571)),
         (ZeroInflatedNegativeBinomial(), 2, 4, 6, (0.87, 5.24, 17.49)),
         (ZeroInflatedNegativeBinomial(psi=0.9), 2, 4, 6, (5.16, 11.32)),
         (ZeroInflatedPoisson(), 4, 5, 6, (1, 5.641)),
```

### Comparing `preliz-0.6.2/preliz/tests/test_roulette.py` & `preliz-0.6.3/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_scipy.py` & `preliz-0.6.3/preliz/tests/test_scipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     LogitNormal,
     LogNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
+    SkewStudentT,
     StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
@@ -66,16 +67,16 @@
             {"a": 2, "b": 5, "loc": -1, "scale": 4},
         ),
         (Cauchy, stats.cauchy, {"alpha": 2, "beta": 4.5}, {"loc": 2, "scale": 4.5}),
         (ChiSquared, stats.chi2, {"nu": 3}, {"df": 3}),
         (
             ExGaussian,
             stats.exponnorm,
-            {"mu": -1, "sigma": 0.5, "nu": 1},
-            {"loc": -1, "scale": 0.5, "K": 1 / 0.5},
+            {"mu": -1, "sigma": 2, "nu": 5},
+            {"loc": -1, "scale": 2, "K": 5 / 2},
         ),
         (Exponential, stats.expon, {"beta": 3.7}, {"scale": 3.7}),
         (Gamma, stats.gamma, {"alpha": 2, "beta": 1 / 3}, {"a": 2, "scale": 3}),
         (Gumbel, stats.gumbel_r, {"mu": 2.5, "beta": 3.5}, {"loc": 2.5, "scale": 3.5}),
         (HalfCauchy, stats.halfcauchy, {"beta": 3.5}, {"scale": 3.5}),
         (HalfNormal, stats.halfnorm, {"sigma": 2}, {"scale": 2}),
         (
@@ -96,14 +97,20 @@
         (
             SkewNormal,
             stats.skewnorm,
             {"mu": 1, "sigma": 0.5, "alpha": 2},
             {"a": 2, "loc": 1, "scale": 0.5},
         ),
         (Rice, stats.rice, {"nu": 0.5, "sigma": 2}, {"b": 0.25, "scale": 2}),
+        (
+            SkewStudentT,
+            stats.jf_skew_t,
+            {"mu": 0.5, "sigma": 2, "a": 3, "b": 5},
+            {"loc": 0.5, "scale": 2, "a": 3, "b": 5},
+        ),
         (StudentT, stats.t, {"nu": 5, "mu": 0, "sigma": 2}, {"df": 5, "loc": 0, "scale": 2}),
         (Triangular, stats.triang, {"lower": 0, "upper": 1, "c": 0.45}, {"c": 0.45}),
         (
             TruncatedNormal,
             stats.truncnorm,
             {"mu": 0, "sigma": 1, "lower": -1, "upper": 1},
             {"loc": 0, "scale": 1, "a": -1, "b": 1},
@@ -168,14 +175,15 @@
         if preliz_dist.kind == "discrete":
             assert_almost_equal(actual, expected, decimal=1)
         elif preliz_name in [
             "HalfStudentT",
             "Moyal",
             "LogitNormal",
             "SkewNormal",
+            "SkewStudentT",
             "Rice",
             "ExGaussian",
         ]:
             assert_almost_equal(actual, expected, decimal=2)
         else:
             assert_almost_equal(actual, expected, decimal=4)
 
@@ -255,24 +263,22 @@
     else:
         expected_logpdf = scipy_dist.logpmf(extended_vals)
 
     if preliz_name == "HalfStudentT":
         assert_almost_equal(actual_logpdf, expected_logpdf, decimal=0)
     elif preliz_name == "LogitNormal":
         assert_almost_equal(actual_logpdf, expected_logpdf, decimal=1)
-    elif preliz_name in ["SkewNormal"]:
-        assert_almost_equal(actual_logpdf, expected_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_logpdf, expected_logpdf)
 
     actual_neg_logpdf = preliz_dist._neg_logpdf(extended_vals)
     expected_neg_logpdf = -expected_logpdf.sum()
     if preliz_name in ["HalfStudentT", "LogitNormal"]:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=1)
-    elif preliz_name in ["TruncatedNormal", "SkewNormal"]:
+    elif preliz_name in ["TruncatedNormal"]:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf)
 
     if preliz_dist.__class__.__name__ not in [
         "HalfStudentT",
         "Rice",
@@ -303,11 +309,11 @@
         assert_almost_equal(actual_moments, expected_moments)
 
     actual_median = preliz_dist.median()
     expected_median = scipy_dist.median()
 
     if preliz_name == "HalfStudentT":
         assert_almost_equal(actual_median, expected_median, decimal=1)
-    elif preliz_name == "SkewNormal":
+    elif preliz_name in ["SkewNormal", "ExGaussian"]:
         assert_almost_equal(actual_median, expected_median, decimal=6)
     else:
         assert_almost_equal(actual_median, expected_median)
```

### Comparing `preliz-0.6.2/preliz/tests/test_special.py` & `preliz-0.6.3/preliz/tests/test_special.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/tests/test_truncated.py` & `preliz-0.6.3/preliz/tests/test_truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/beta_mode.py` & `preliz-0.6.3/preliz/unidimensional/beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/dirichlet_mode.py` & `preliz-0.6.3/preliz/unidimensional/dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/maxent.py` & `preliz-0.6.3/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/mle.py` & `preliz-0.6.3/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/quartile.py` & `preliz-0.6.3/preliz/unidimensional/quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/quartile_int.py` & `preliz-0.6.3/preliz/unidimensional/quartile_int.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/preliz/unidimensional/roulette.py` & `preliz-0.6.3/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/pyproject.toml` & `preliz-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `preliz-0.6.2/PKG-INFO` & `preliz-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.6.2
+Version: 0.6.3
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
```

