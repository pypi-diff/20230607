# Comparing `tmp/inference-tools-0.9.1.tar.gz` & `tmp/inference-tools-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-tools-0.9.1.tar", last modified: Sun Oct  2 18:08:23 2022, max compression
+gzip compressed data, was "inference-tools-0.9.2.tar", last modified: Sat Dec  3 16:03:41 2022, max compression
```

## Comparing `inference-tools-0.9.1.tar` & `inference-tools-0.9.2.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.334055 inference-tools-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.338055 inference-tools-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-10-02 18:08:09.000000 inference-tools-0.9.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-10-02 18:08:09.000000 inference-tools-0.9.1/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-10-02 18:08:09.000000 inference-tools-0.9.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-10-02 18:08:09.000000 inference-tools-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-02 18:08:09.000000 inference-tools-0.9.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-02 18:08:09.000000 inference-tools-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-10-02 18:08:23.358055 inference-tools-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-10-02 18:08:09.000000 inference-tools-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.342055 inference-tools-0.9.1/demos/
--rw-r--r--   0 runner    (1001) docker     (121)   113682 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/density_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   829844 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/gaussian_fitting_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   212412 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/gibbs_sampling_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   186252 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/gp_linear_inversion_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   204235 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/gp_optimisation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   204558 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/gp_regression_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   303140 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/hamiltonian_mcmc_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   366363 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/parallel_tempering_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   266533 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/peak_fitting_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.342055 inference-tools-0.9.1/demos/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/ChainPool_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/GaussianKDE_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4277 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/GibbsChain_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5110 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/GpOptimiser_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/HamiltonianChain_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/ParallelTempering_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/UnimodalPdf_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     6522 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/gaussian_fitting_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/parameter_constraints_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     5149 2022-10-02 18:08:09.000000 inference-tools-0.9.1/demos/scripts/spectroscopy_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.342055 inference-tools-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.346055 inference-tools-0.9.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/EnsembleSampler.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/GibbsChain.rst
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/GpLinearInverter.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1758 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/GpOptimiser.rst
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/GpRegressor.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/HamiltonianChain.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/ParallelTempering.rst
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/PcaChain.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/acquisition_functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/covariance_functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/distributions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8491 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/gp.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.338055 inference-tools-0.9.1/docs/source/images/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.346055 inference-tools-0.9.1/docs/source/images/GibbsChain_images/
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GibbsChain_images/GibbsChain_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)    73941 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GibbsChain_images/burned_scatter.png
--rw-r--r--   0 runner    (1001) docker     (121)   133658 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GibbsChain_images/gibbs_diagnostics.png
--rw-r--r--   0 runner    (1001) docker     (121)    34173 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GibbsChain_images/gibbs_marginals.png
--rw-r--r--   0 runner    (1001) docker     (121)    59978 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GibbsChain_images/initial_scatter.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.346055 inference-tools-0.9.1/docs/source/images/GpOptimiser_images/
--rw-r--r--   0 runner    (1001) docker     (121)     3949 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpOptimiser_images/GpOptimiser_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)  1568032 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpOptimiser_images/GpOptimiser_iteration.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.346055 inference-tools-0.9.1/docs/source/images/GpRegressor_images/
--rw-r--r--   0 runner    (1001) docker     (121)     6646 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpRegressor_images/GpRegressor_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)    93530 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpRegressor_images/gradient_prediction.png
--rw-r--r--   0 runner    (1001) docker     (121)   156918 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpRegressor_images/posterior_samples.png
--rw-r--r--   0 runner    (1001) docker     (121)    85187 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpRegressor_images/regression_estimate.png
--rw-r--r--   0 runner    (1001) docker     (121)    48246 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/GpRegressor_images/sampled_data.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.346055 inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/HamiltonianChain_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)    58144 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/hmc_matrix_plot.png
--rw-r--r--   0 runner    (1001) docker     (121)  3629051 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/hmc_scatterplot.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.350055 inference-tools-0.9.1/docs/source/images/ParallelTempering_images/
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/ParallelTempering_images/ParallelTempering_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)    46620 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/ParallelTempering_images/parallel_tempering_matrix.png
--rw-r--r--   0 runner    (1001) docker     (121)   478063 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/ParallelTempering_images/parallel_tempering_trace.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.354055 inference-tools-0.9.1/docs/source/images/gallery_images/
--rw-r--r--   0 runner    (1001) docker     (121)    30317 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_density_estimation.png
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_density_estimation.py
--rw-r--r--   0 runner    (1001) docker     (121)    63238 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gibbs_sampling.png
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gibbs_sampling.py
--rw-r--r--   0 runner    (1001) docker     (121)    47210 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gpr.png
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gpr.py
--rw-r--r--   0 runner    (1001) docker     (121)    32366 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hdi.png
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hdi.py
--rw-r--r--   0 runner    (1001) docker     (121)   122651 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hmc.png
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hmc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/gallery_images/gallery_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.354055 inference-tools-0.9.1/docs/source/images/getting_started_images/
--rw-r--r--   0 runner    (1001) docker     (121)    24291 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/getting_started_images/gaussian_data.png
--rw-r--r--   0 runner    (1001) docker     (121)     6829 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/getting_started_images/getting_started_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)    61108 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/getting_started_images/matrix_plot_example.png
--rw-r--r--   0 runner    (1001) docker     (121)    64729 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/getting_started_images/pdf_summary_example.png
--rw-r--r--   0 runner    (1001) docker     (121)   167783 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/getting_started_images/plot_diagnostics_example.png
--rw-r--r--   0 runner    (1001) docker     (121)    48769 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/getting_started_images/prediction_uncertainty_example.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.354055 inference-tools-0.9.1/docs/source/images/matrix_plot_images/
--rw-r--r--   0 runner    (1001) docker     (121)    65466 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/matrix_plot_images/matrix_plot_example.png
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/images/matrix_plot_images/matrix_plot_image_production.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/likelihoods.rst
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/mcmc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/pdf.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/posterior.rst
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-10-02 18:08:09.000000 inference-tools-0.9.1/docs/source/priors.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/inference/
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/inference/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    23592 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/__pycache__/gp_tools.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    25397 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/__pycache__/mcmc.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    18038 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/__pycache__/pdf_tools.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-02 18:08:23.000000 inference-tools-0.9.1/inference/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     8181 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (121)    18800 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)    45366 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/gp.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/gp_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    10597 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (121)    95270 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3958 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/mean.py
--rw-r--r--   0 runner    (1001) docker     (121)    24546 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/pdf_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    18665 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/posterior.py
--rw-r--r--   0 runner    (1001) docker     (121)    14770 2022-10-02 18:08:09.000000 inference-tools-0.9.1/inference/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/inference_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-10-02 18:08:23.000000 inference-tools-0.9.1/inference_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4807 2022-10-02 18:08:23.000000 inference-tools-0.9.1/inference_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-02 18:08:23.000000 inference-tools-0.9.1/inference_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-02 18:08:23.000000 inference-tools-0.9.1/inference_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-02 18:08:23.000000 inference-tools-0.9.1/inference_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-10-02 18:08:09.000000 inference-tools-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-10-02 18:08:23.358055 inference-tools-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-02 18:08:09.000000 inference-tools-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/tests/gp/
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/gp/test_GpLinearInverter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/gp/test_GpOptimiser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/gp/test_GpRegressor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-02 18:08:23.358055 inference-tools-0.9.1/tests/mcmc/
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/mcmc/mcmc_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/mcmc/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     9159 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/mcmc/test_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/mcmc/test_hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/mcmc/test_pca.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/test_covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)     7897 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/test_likelihoods.py
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3018 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/test_posterior.py
--rw-r--r--   0 runner    (1001) docker     (121)    12803 2022-10-02 18:08:09.000000 inference-tools-0.9.1/tests/test_priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.486428 inference-tools-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.458428 inference-tools-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.458428 inference-tools-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-03 16:03:27.000000 inference-tools-0.9.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-03 16:03:27.000000 inference-tools-0.9.2/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-03 16:03:27.000000 inference-tools-0.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2022-12-03 16:03:27.000000 inference-tools-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2022-12-03 16:03:27.000000 inference-tools-0.9.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-03 16:03:27.000000 inference-tools-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2022-12-03 16:03:41.486428 inference-tools-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2022-12-03 16:03:27.000000 inference-tools-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.462428 inference-tools-0.9.2/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)   113682 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/density_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   829844 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/gaussian_fitting_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   212412 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/gibbs_sampling_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   186252 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/gp_linear_inversion_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   204235 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/gp_optimisation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   204558 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/gp_regression_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   303140 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/hamiltonian_mcmc_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   366363 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/parallel_tempering_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   266533 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/peak_fitting_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.466428 inference-tools-0.9.2/demos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/ChainPool_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/GaussianKDE_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/GibbsChain_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/GpOptimiser_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/HamiltonianChain_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/ParallelTempering_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/UnimodalPdf_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/gaussian_fitting_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/parameter_constraints_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2022-12-03 16:03:27.000000 inference-tools-0.9.2/demos/scripts/spectroscopy_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.466428 inference-tools-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.466428 inference-tools-0.9.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/EnsembleSampler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/GibbsChain.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/GpLinearInverter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/GpOptimiser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/GpRegressor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/HamiltonianChain.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/ParallelTempering.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/PcaChain.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/acquisition_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/covariance_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/gp.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.458428 inference-tools-0.9.2/docs/source/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.466428 inference-tools-0.9.2/docs/source/images/GibbsChain_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GibbsChain_images/GibbsChain_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73941 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GibbsChain_images/burned_scatter.png
+-rw-r--r--   0 runner    (1001) docker     (123)   133658 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GibbsChain_images/gibbs_diagnostics.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34173 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GibbsChain_images/gibbs_marginals.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59978 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GibbsChain_images/initial_scatter.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.466428 inference-tools-0.9.2/docs/source/images/GpOptimiser_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpOptimiser_images/GpOptimiser_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1568032 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpOptimiser_images/GpOptimiser_iteration.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.470428 inference-tools-0.9.2/docs/source/images/GpRegressor_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpRegressor_images/GpRegressor_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93530 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpRegressor_images/gradient_prediction.png
+-rw-r--r--   0 runner    (1001) docker     (123)   156918 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpRegressor_images/posterior_samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85187 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpRegressor_images/regression_estimate.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48246 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/GpRegressor_images/sampled_data.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.470428 inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/HamiltonianChain_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58144 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/hmc_matrix_plot.png
+-rw-r--r--   0 runner    (1001) docker     (123)  3629051 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/hmc_scatterplot.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.474428 inference-tools-0.9.2/docs/source/images/ParallelTempering_images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/ParallelTempering_images/ParallelTempering_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46620 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/ParallelTempering_images/parallel_tempering_matrix.png
+-rw-r--r--   0 runner    (1001) docker     (123)   478063 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/ParallelTempering_images/parallel_tempering_trace.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.478428 inference-tools-0.9.2/docs/source/images/gallery_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    30317 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_density_estimation.png
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_density_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63238 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gibbs_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gibbs_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47210 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gpr.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32366 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hdi.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122651 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hmc.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/gallery_images/gallery_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.478428 inference-tools-0.9.2/docs/source/images/getting_started_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    24291 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/getting_started_images/gaussian_data.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/getting_started_images/getting_started_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61108 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/getting_started_images/matrix_plot_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64729 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/getting_started_images/pdf_summary_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   167783 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/getting_started_images/plot_diagnostics_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48769 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/getting_started_images/prediction_uncertainty_example.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.478428 inference-tools-0.9.2/docs/source/images/matrix_plot_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    65466 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/matrix_plot_images/matrix_plot_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/images/matrix_plot_images/matrix_plot_image_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/likelihoods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/mcmc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/pdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/posterior.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2022-12-03 16:03:27.000000 inference-tools-0.9.2/docs/source/priors.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.482428 inference-tools-0.9.2/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.482428 inference-tools-0.9.2/inference/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    23592 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/__pycache__/gp_tools.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    25397 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/__pycache__/mcmc.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/__pycache__/pdf_tools.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-03 16:03:41.000000 inference-tools-0.9.2/inference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21903 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45503 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/gp_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95222 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24522 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/pdf_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2022-12-03 16:03:27.000000 inference-tools-0.9.2/inference/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.482428 inference-tools-0.9.2/inference_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2022-12-03 16:03:41.000000 inference-tools-0.9.2/inference_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2022-12-03 16:03:41.000000 inference-tools-0.9.2/inference_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 16:03:41.000000 inference-tools-0.9.2/inference_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-03 16:03:41.000000 inference-tools-0.9.2/inference_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-03 16:03:41.000000 inference-tools-0.9.2/inference_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-03 16:03:27.000000 inference-tools-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2022-12-03 16:03:41.486428 inference-tools-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-03 16:03:27.000000 inference-tools-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.482428 inference-tools-0.9.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.486428 inference-tools-0.9.2/tests/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/gp/test_GpLinearInverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/gp/test_GpOptimiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/gp/test_GpRegressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 16:03:41.486428 inference-tools-0.9.2/tests/mcmc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/mcmc/mcmc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/mcmc/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/mcmc/test_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/mcmc/test_hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/mcmc/test_pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/test_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/test_likelihoods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/test_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2022-12-03 16:03:27.000000 inference-tools-0.9.2/tests/test_priors.py
```

### Comparing `inference-tools-0.9.1/.github/workflows/black.yml` & `inference-tools-0.9.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/.github/workflows/python_publish.yml` & `inference-tools-0.9.2/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/.github/workflows/tests.yml` & `inference-tools-0.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/.gitignore` & `inference-tools-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/.readthedocs.yaml` & `inference-tools-0.9.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/LICENSE` & `inference-tools-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/PKG-INFO` & `inference-tools-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-tools
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of python tools for Bayesian data analysis
 Home-page: https://github.com/C-bowman/inference-tools
 Author: Chris Bowman
 Author-email: chris.bowman.physics@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/C-bowman/inference-tools
 Project-URL: Tracker, https://github.com/C-bowman/inference-tools/issues
```

### Comparing `inference-tools-0.9.1/README.md` & `inference-tools-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/density_estimation_demo.ipynb` & `inference-tools-0.9.2/demos/density_estimation_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/gaussian_fitting_demo.ipynb` & `inference-tools-0.9.2/demos/gaussian_fitting_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/gibbs_sampling_demo.ipynb` & `inference-tools-0.9.2/demos/gibbs_sampling_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/gp_linear_inversion_demo.ipynb` & `inference-tools-0.9.2/demos/gp_linear_inversion_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/gp_optimisation_demo.ipynb` & `inference-tools-0.9.2/demos/gp_optimisation_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/gp_regression_demo.ipynb` & `inference-tools-0.9.2/demos/gp_regression_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/hamiltonian_mcmc_demo.ipynb` & `inference-tools-0.9.2/demos/hamiltonian_mcmc_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/parallel_tempering_demo.ipynb` & `inference-tools-0.9.2/demos/parallel_tempering_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/peak_fitting_demo.ipynb` & `inference-tools-0.9.2/demos/peak_fitting_demo.ipynb`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/ChainPool_demo.py` & `inference-tools-0.9.2/demos/scripts/ChainPool_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/GaussianKDE_demo.py` & `inference-tools-0.9.2/demos/scripts/GaussianKDE_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/GibbsChain_demo.py` & `inference-tools-0.9.2/demos/scripts/GibbsChain_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/GpOptimiser_demo.py` & `inference-tools-0.9.2/demos/scripts/GpOptimiser_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/HamiltonianChain_demo.py` & `inference-tools-0.9.2/demos/scripts/HamiltonianChain_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/ParallelTempering_demo.py` & `inference-tools-0.9.2/demos/scripts/ParallelTempering_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/UnimodalPdf_demo.py` & `inference-tools-0.9.2/demos/scripts/UnimodalPdf_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/gaussian_fitting_demo.py` & `inference-tools-0.9.2/demos/scripts/gaussian_fitting_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/parameter_constraints_demo.py` & `inference-tools-0.9.2/demos/scripts/parameter_constraints_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/demos/scripts/spectroscopy_demo.py` & `inference-tools-0.9.2/demos/scripts/spectroscopy_demo.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/Makefile` & `inference-tools-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/make.bat` & `inference-tools-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/GibbsChain.rst` & `inference-tools-0.9.2/docs/source/GibbsChain.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/GpOptimiser.rst` & `inference-tools-0.9.2/docs/source/GpOptimiser.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/HamiltonianChain.rst` & `inference-tools-0.9.2/docs/source/HamiltonianChain.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/ParallelTempering.rst` & `inference-tools-0.9.2/docs/source/ParallelTempering.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/acquisition_functions.rst` & `inference-tools-0.9.2/docs/source/acquisition_functions.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/conf.py` & `inference-tools-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/covariance_functions.rst` & `inference-tools-0.9.2/docs/source/covariance_functions.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/getting_started.rst` & `inference-tools-0.9.2/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/gp.rst` & `inference-tools-0.9.2/docs/source/gp.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GibbsChain_images/GibbsChain_image_production.py` & `inference-tools-0.9.2/docs/source/images/GibbsChain_images/GibbsChain_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GibbsChain_images/burned_scatter.png` & `inference-tools-0.9.2/docs/source/images/GibbsChain_images/burned_scatter.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GibbsChain_images/gibbs_diagnostics.png` & `inference-tools-0.9.2/docs/source/images/GibbsChain_images/gibbs_diagnostics.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GibbsChain_images/gibbs_marginals.png` & `inference-tools-0.9.2/docs/source/images/GibbsChain_images/gibbs_marginals.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GibbsChain_images/initial_scatter.png` & `inference-tools-0.9.2/docs/source/images/GibbsChain_images/initial_scatter.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpOptimiser_images/GpOptimiser_image_production.py` & `inference-tools-0.9.2/docs/source/images/GpOptimiser_images/GpOptimiser_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpOptimiser_images/GpOptimiser_iteration.gif` & `inference-tools-0.9.2/docs/source/images/GpOptimiser_images/GpOptimiser_iteration.gif`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpRegressor_images/GpRegressor_image_production.py` & `inference-tools-0.9.2/docs/source/images/GpRegressor_images/GpRegressor_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpRegressor_images/gradient_prediction.png` & `inference-tools-0.9.2/docs/source/images/GpRegressor_images/gradient_prediction.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpRegressor_images/posterior_samples.png` & `inference-tools-0.9.2/docs/source/images/GpRegressor_images/posterior_samples.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpRegressor_images/regression_estimate.png` & `inference-tools-0.9.2/docs/source/images/GpRegressor_images/regression_estimate.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/GpRegressor_images/sampled_data.png` & `inference-tools-0.9.2/docs/source/images/GpRegressor_images/sampled_data.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/HamiltonianChain_image_production.py` & `inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/HamiltonianChain_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/hmc_matrix_plot.png` & `inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/hmc_matrix_plot.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/HamiltonianChain_images/hmc_scatterplot.html` & `inference-tools-0.9.2/docs/source/images/HamiltonianChain_images/hmc_scatterplot.html`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/ParallelTempering_images/ParallelTempering_image_production.py` & `inference-tools-0.9.2/docs/source/images/ParallelTempering_images/ParallelTempering_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/ParallelTempering_images/parallel_tempering_matrix.png` & `inference-tools-0.9.2/docs/source/images/ParallelTempering_images/parallel_tempering_matrix.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/ParallelTempering_images/parallel_tempering_trace.png` & `inference-tools-0.9.2/docs/source/images/ParallelTempering_images/parallel_tempering_trace.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_density_estimation.png` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_density_estimation.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_density_estimation.py` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_density_estimation.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gibbs_sampling.png` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gibbs_sampling.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gibbs_sampling.py` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gibbs_sampling.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gpr.png` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gpr.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_gpr.py` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_gpr.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hdi.png` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hdi.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hdi.py` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hdi.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hmc.png` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hmc.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/gallery_images/gallery_hmc.py` & `inference-tools-0.9.2/docs/source/images/gallery_images/gallery_hmc.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/getting_started_images/gaussian_data.png` & `inference-tools-0.9.2/docs/source/images/getting_started_images/gaussian_data.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/getting_started_images/getting_started_image_production.py` & `inference-tools-0.9.2/docs/source/images/getting_started_images/getting_started_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/getting_started_images/matrix_plot_example.png` & `inference-tools-0.9.2/docs/source/images/getting_started_images/matrix_plot_example.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/getting_started_images/pdf_summary_example.png` & `inference-tools-0.9.2/docs/source/images/getting_started_images/pdf_summary_example.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/getting_started_images/plot_diagnostics_example.png` & `inference-tools-0.9.2/docs/source/images/getting_started_images/plot_diagnostics_example.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/getting_started_images/prediction_uncertainty_example.png` & `inference-tools-0.9.2/docs/source/images/getting_started_images/prediction_uncertainty_example.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/matrix_plot_images/matrix_plot_example.png` & `inference-tools-0.9.2/docs/source/images/matrix_plot_images/matrix_plot_example.png`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/images/matrix_plot_images/matrix_plot_image_production.py` & `inference-tools-0.9.2/docs/source/images/matrix_plot_images/matrix_plot_image_production.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/index.rst` & `inference-tools-0.9.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/likelihoods.rst` & `inference-tools-0.9.2/docs/source/likelihoods.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/pdf.rst` & `inference-tools-0.9.2/docs/source/pdf.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/plotting.rst` & `inference-tools-0.9.2/docs/source/plotting.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/docs/source/priors.rst` & `inference-tools-0.9.2/docs/source/priors.rst`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/inference/__pycache__/gp_tools.cpython-36.pyc` & `inference-tools-0.9.2/inference/__pycache__/gp_tools.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/inference/__pycache__/mcmc.cpython-36.pyc` & `inference-tools-0.9.2/inference/__pycache__/mcmc.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/inference/__pycache__/pdf_tools.cpython-36.pyc` & `inference-tools-0.9.2/inference/__pycache__/pdf_tools.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/inference/acquisition.py` & `inference-tools-0.9.2/inference/acquisition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from numpy import sqrt, log, exp, pi
 from numpy import array, ndarray, minimum, maximum
 from numpy.random import random
 from scipy.special import erf, erfcx
 
 
-class AcquisitionFunction(object):
+class AcquisitionFunction:
     gp = None
     opt_func = None
 
     def starting_positions(self, bounds):
         lwr, upr = [array([k[i] for k in bounds], dtype=float) for i in [0, 1]]
         widths = upr - lwr
```

### Comparing `inference-tools-0.9.1/inference/covariance.py` & `inference-tools-0.9.2/inference/covariance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from abc import ABC, abstractmethod
+from collections.abc import Sequence
 from inspect import isclass
+from itertools import chain
 from numpy import abs, exp, eye, log, zeros, ndarray
 
 
 class CovarianceFunction(ABC):
     """
     Abstract base class for covariance functions.
     """
@@ -147,16 +149,16 @@
         Estimates bounds on the hyper-parameters to be
         used during optimisation.
         """
         # construct sensible bounds on the hyperparameter values
         s = log(y.ptp())
         self.bounds = [(s - 8, s + 2)]
 
-    def __call__(self, u, v, theta):
-        return zeros([u.size, v.size])
+    def __call__(self, u: ndarray, v: ndarray, theta):
+        return zeros([u.shape[0], v.shape[0]])
 
     def build_covariance(self, theta):
         """
         Optimized version of self.matrix() specifically for the data
         covariance matrix where the vectors v1 & v2 are both self.x.
         """
         sigma_sq = exp(2 * theta[0])
@@ -360,145 +362,231 @@
 
     def get_bounds(self):
         return self.bounds
 
 
 class ChangePoint(CovarianceFunction):
     r"""
-    ``ChangePoint`` is a covariance function which divides the input space into two
-    regions (at some point along a chosen input dimension), allowing each of the two
-    regions to be modelled using a separate covariance function.
+    ``ChangePoint`` is a covariance function which divides the input space into multiple
+    regions (at various points along a chosen input dimension), allowing each of the
+    regions to be modelled using a separate covariance function. The boundaries which
+    define the extent of each region are referred to as 'change-points'. The locations
+    of the change-points, and the width over which the transition between regions occurs
+    are hyperparameters determined from the data.
 
     This is useful in cases where properties of the data (e.g. the scale-lengths
     over which the data vary) change significantly over the input dimension which is
     used to divide the space.
 
-    The change-point kernel :math:`K_{\mathrm{cp}}` is a weighted-sum of the two
-    input kernels :math:`K_{1}, \, K_{2}` which model each of the two regions:
+    The change-point kernel :math:`K_{\mathrm{cp}}` is a weighted-sum of the
+    input kernels :math:`K_{1}, \, K_{2}, \dots , K_{n}` which model each of the
+    :math:`n` regions:
 
     .. math::
+       K_{\mathrm{cp}}(u, v) = K_1 a_1 + \left(\sum_{i=2}^{n-1} K_i a_{i+1} b_{i}\right) + K_n b_n
 
-       K_{\mathrm{cp}}(u, v) = K_{1}(u, v) (1 - f(u))(1 - f(v)) + K_{2}(u, v) f(u) f(v)
-
-    where the weighting :math:`f(x)` is the logistic function
+    where
 
     .. math::
+       a_{i}(u, v) = (1 - f_i (u)) (1 - f_i (v)), \quad b_{i}(u, v) = f_i (u) f_i (v)
 
-       f(x) = \frac{1}{1 + e^{-(x - x_0) / w}}
+    and :math:`f_i` is the logistic weighting function associated with the :math:`i`'th
+    change-point:
 
-    and :math:`x_0, \, w` are the location and width of the change-point respectively.
-    :math:`x_0` and :math:`w` are hyperparameters which are determined automatically
-    (alongside the hyperparameters for :math:`K_{1}, \, K_{2}`).
+    .. math::
+       f_i(x) = \frac{1}{1 + e^{-(x - c_i) / w_i}}
 
-    :param K1:
-        The covariance kernel which applies to the 'low' side of the change-point.
+    and :math:`c_i, \, w_i` are the location and width of the :math:`i`'th change-point
+    respectively. The :math:`c_i` and :math:`w_i` are hyperparameters which are determined
+    automatically (alongside the hyperparameters for the kernels in each region).
 
-    :param K2:
-        The covariance kernel which applies to the 'high' side of the change-point.
+    :param kernels:
+        A tuple of the kernel objects to be used ``(K1, K2, K3, ...)``
 
     :param int axis:
-        The spatial axis over which the transition between the two kernels occurs.
+        The spatial axis over which the transitions between kernels occur.
 
     :param location_bounds:
-        The bounds for the change-point location hyperparameter
-        :math:`x_0` as a tuple of the form ``(lower_bound, upper_bound)``.
+        The bounds for the change-point location hyperparameters :math:`c_i` as a tuple
+        of the form ``((lower_bound_0, upper_bound_0),(lower_bound_1, upper_bound_1),...)``.
+        There should always be :math:`n-1` pairs of bounds where :math:`n` is the number
+        of kernels specified.
 
     :param width_bounds:
-        The bounds for the change-point width hyperparameter :math:`w` as a tuple
-        of the form ``(lower_bound, upper_bound)``.
+        The bounds for the change-point width hyperparameters :math:`w_i` as a tuple of
+        the form ``((lower_bound_0, upper_bound_0),(lower_bound_1, upper_bound_1),...)``.
+        There should always be :math:`n-1` pairs of bounds where :math:`n` is the number
+        of kernels specified.
     """
 
     def __init__(
         self,
-        K1=SquaredExponential,
-        K2=SquaredExponential,
-        axis=0,
-        location_bounds=None,
-        width_bounds=None,
+        kernels: Sequence,
+        axis: int = 0,
+        location_bounds: Sequence = None,
+        width_bounds: Sequence = None,
     ):
-        self.cov1 = K1() if isclass(K1) else K1
-        self.cov2 = K2() if isclass(K2) else K2
+        # check that all the kernels are valid
+        self.cov = [
+            K() if isclass(K) and issubclass(K, CovarianceFunction) else K
+            for K in kernels
+        ]
+        for K in self.cov:
+            if not isinstance(K, CovarianceFunction):
+                raise TypeError(
+                    """
+                    [ ChangePoint error ]
+                    >> Each of the specified covariance kernels must be an instance of
+                    >> a class which inherits from the 'CovarianceFunction' abstract
+                    >> base-class.
+                    """
+                )
+
+        self.n_kernels = len(kernels)
+
+        if location_bounds is not None:
+            if len(location_bounds) != self.n_kernels - 1:
+                raise ValueError(
+                    """
+                    [ ChangePoint error ]
+                    >> The length of 'location_bounds' must be one less than the number of kernels
+                    """
+                )
+            self.location_bounds = [check_bounds(lb) for lb in location_bounds]
+        else:
+            self.location_bounds = None
+
+        if width_bounds is not None:
+            if len(width_bounds) != self.n_kernels - 1:
+                raise ValueError(
+                    """
+                    [ ChangePoint error ]
+                    >> The length of 'width_bounds' must be one less than the number of kernels
+                    """
+                )
+            self.width_bounds = [check_bounds(wb) for wb in width_bounds]
+        else:
+            self.width_bounds = None
+
         self.axis = axis
-        self.location_bounds = check_bounds(location_bounds)
-        self.width_bounds = check_bounds(width_bounds)
         self.hyperpar_labels = []
         self.bounds = None
 
     def pass_spatial_data(self, x: ndarray):
-        self.cov1.pass_spatial_data(x)
-        self.cov2.pass_spatial_data(x)
+        [K.pass_spatial_data(x) for K in self.cov]
         # Create slices to address the parameters of each component
-        param_counts = [self.cov1.n_params, self.cov2.n_params, 2]
+        param_counts = [K.n_params for K in self.cov]
+        param_counts.extend([2] * (self.n_kernels - 1))
+
         self.n_params = sum(param_counts)
-        self.K1_slc, self.K2_slc, self.CP_slc = slice_builder(param_counts)
-        # combine hyperparameter labels for K1, K2 and the change-point
-        label_groups = [
-            [f"ChngPnt K1: {lab}" for lab in self.cov1.hyperpar_labels],
-            [f"ChngPnt K2: {lab}" for lab in self.cov2.hyperpar_labels],
-            ["ChngPnt location", "ChngPnt width"],
-        ]
+        slices = slice_builder(param_counts)
+        self.cov_slc = slices[: self.n_kernels]
+        self.cp_slc = slices[self.n_kernels :]
+
+        # combine hyperparameter labels for Kernels and the change-point
+        label_groups = []
+        for i, K in enumerate(self.cov):
+            label_groups.append([f"ChngPnt K{i}: {lab}" for lab in K.hyperpar_labels])
+
+        for i in range(self.n_kernels - 1):
+            label_groups.append([f"ChngPnt{i} location", f"ChngPnt{i} width"])
+
         [self.hyperpar_labels.extend(L) for L in label_groups]
 
         # store x-data from the dimension of the change-point
         self.x_cp = x[:, self.axis]
         assert self.n_params == len(self.hyperpar_labels)
 
     def estimate_hyperpar_bounds(self, y: ndarray):
         xr = self.x_cp.min(), self.x_cp.max()
         dx = xr[1] - xr[0]
         # combine parameter bounds for K1, K2 and the change-point
-        if self.cov1.bounds is None:
-            self.cov1.estimate_hyperpar_bounds(y)
-        if self.cov2.bounds is None:
-            self.cov2.estimate_hyperpar_bounds(y)
         self.bounds = []
-        self.bounds.extend(self.cov1.bounds)
-        self.bounds.extend(self.cov2.bounds)
-        self.bounds.extend(
-            [
-                xr if self.location_bounds is None else self.location_bounds,
-                (5e-3 * dx, 0.5 * dx)
-                if self.width_bounds is None
-                else self.width_bounds,
-            ]
-        )
+        for cov in self.cov:
+            cov.estimate_hyperpar_bounds(y)
+            self.bounds.extend(cov.bounds)
+
+        if self.location_bounds is None:
+            self.location_bounds = [xr] * (self.n_kernels - 1)
+
+        if self.width_bounds is None:
+            self.width_bounds = [(5e-3 * dx, 0.5 * dx)] * (self.n_kernels - 1)
+
+        # interleave the location / width bounds using chain and zip
+        cp_bounds = chain.from_iterable(zip(self.location_bounds, self.width_bounds))
+        self.bounds.extend([b for b in cp_bounds])
+
         # check for consistency of length of bounds
         assert self.n_params == len(self.bounds)
 
-    def __call__(self, u, v, theta):
-        K1 = self.cov1(u, v, theta[self.K1_slc])
-        K2 = self.cov2(u, v, theta[self.K2_slc])
-        w_u = self.logistic(u[:, self.axis], theta[self.CP_slc])
-        w_v = self.logistic(v[:, self.axis], theta[self.CP_slc])
-        w1 = (1 - w_u)[:, None] * (1 - w_v)[None, :]
-        w2 = w_u[:, None] * w_v[None, :]
-        return K1 * w1 + K2 * w2
+    def __call__(self, u: ndarray, v: ndarray, theta):
+        kernel_coeffs = [1.0]
+        for slc in self.cp_slc:
+            w_u = self.logistic(u[:, self.axis], theta[slc])
+            w_v = self.logistic(v[:, self.axis], theta[slc])
+
+            w1 = (1 - w_u)[:, None] * (1 - w_v)[None, :]
+            w2 = w_u[:, None] * w_v[None, :]
+
+            kernel_coeffs[-1] *= w1
+            kernel_coeffs.append(w2)
+
+        return sum(
+            self.cov[i](u, v, theta[self.cov_slc[i]]) * kernel_coeffs[i]
+            for i in range(self.n_kernels)
+        )
 
     def build_covariance(self, theta):
-        K1 = self.cov1.build_covariance(theta[self.K1_slc])
-        K2 = self.cov2.build_covariance(theta[self.K2_slc])
-        w = self.logistic(self.x_cp, theta[self.CP_slc])
-        w1 = (1 - w)[:, None] * (1 - w)[None, :]
-        w2 = w[:, None] * w[None, :]
-        return K1 * w1 + K2 * w2
+        kernel_coeffs = [1.0]
+        for slc in self.cp_slc:
+            w = self.logistic(self.x_cp, theta[slc])
+            w1 = (1 - w)[:, None] * (1 - w)[None, :]
+            w2 = w[:, None] * w[None, :]
+
+            kernel_coeffs[-1] *= w1
+            kernel_coeffs.append(w2)
+
+        return sum(
+            self.cov[i].build_covariance(theta[self.cov_slc[i]]) * kernel_coeffs[i]
+            for i in range(self.n_kernels)
+        )
 
     def covariance_and_gradients(self, theta):
-        K1, K1_grads = self.cov1.covariance_and_gradients(theta[self.K1_slc])
-        K2, K2_grads = self.cov2.covariance_and_gradients(theta[self.K2_slc])
-        w, w_grads = self.logistic_and_gradient(self.x_cp, theta[self.CP_slc])
-        w1 = (1 - w)[:, None] * (1 - w)[None, :]
-        w2 = w[:, None] * w[None, :]
-        K = K1 * w1 + K2 * w2
-        gradients = [c * w1 for c in K1_grads]
-        gradients.extend([c * w2 for c in K2_grads])
-        for g in w_grads:
-            A = -g[:, None] * (1 - w)[None, :]
-            B = g[:, None] * w[None, :]
-            gradients.append(K1 * (A + A.T) + K2 * (B + B.T))
-        return K, gradients
+        K_vals = []
+        K_grads = []
+        for i in range(self.n_kernels):
+            K, dK = self.cov[i].covariance_and_gradients(theta[self.cov_slc[i]])
+            K_vals.append(K)
+            K_grads.append(dK)
+
+        kernel_coeffs = [1.0]
+        w_vals = []
+        w_grads = []
+        for slc in self.cp_slc:
+            w, dw = self.logistic_and_gradient(self.x_cp, theta[slc])
+            w1 = (1 - w)[:, None] * (1 - w)[None, :]
+            w2 = w[:, None] * w[None, :]
+            kernel_coeffs[-1] *= w1
+            kernel_coeffs.append(w2)
+            w_grads.append(dw)
+            w_vals.append(w)
+
+        covar = sum(K_vals[i] * kernel_coeffs[i] for i in range(self.n_kernels))
+
+        gradients = []
+        for i in range(self.n_kernels):
+            gradients.extend([dK * kernel_coeffs[i] for dK in K_grads[i]])
+
+        for i in range(self.n_kernels - 1):
+            w = w_vals[i]
+            for dw in w_grads[i]:
+                A = -dw[:, None] * (1 - w)[None, :]
+                B = dw[:, None] * w[None, :]
+                gradients.append(K_vals[i] * (A + A.T) + K_vals[i + 1] * (B + B.T))
+        return covar, gradients
 
     @staticmethod
     def logistic(x, theta):
         z = (x - theta[0]) / theta[1]
         return 1.0 / (1.0 + exp(-z))
 
     @staticmethod
```

### Comparing `inference-tools-0.9.1/inference/gp.py` & `inference-tools-0.9.2/inference/gp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from numpy import sum as npsum
 from numpy.linalg import cholesky, LinAlgError
 from scipy.linalg import solve, solve_triangular
 from scipy.optimize import minimize, differential_evolution, fmin_l_bfgs_b
 from multiprocessing import Pool
 from warnings import warn
 from copy import copy
-from typing import Type
-from collections.abc import Sequence
 
 import matplotlib.pyplot as plt
 
 from inference.covariance import *
 from inference.mean import *
 from inference.acquisition import *
 
@@ -86,16 +84,16 @@
     def __init__(
         self,
         x: ndarray,
         y: ndarray,
         y_err: ndarray = None,
         y_cov: ndarray = None,
         hyperpars: ndarray = None,
-        kernel: Type[CovarianceFunction] = SquaredExponential,
-        mean: Type[MeanFunction] = ConstantMean,
+        kernel: CovarianceFunction = SquaredExponential,
+        mean: MeanFunction = ConstantMean,
         cross_val: bool = False,
         optimizer: str = "bfgs",
         n_processes: int = 1,
         n_starts: int = None,
     ):
 
         # store the data
@@ -499,19 +497,18 @@
 
         This implementation is based on equations (5.10, 5.11, 5.12, 5.13, 5.14)
         from Rasmussen & Williams.
         """
         K_xx, grad_K = self.cov.covariance_and_gradients(theta[self.cov_slice])
         K_xx += self.sig
         mu, grad_mu = self.mean.mean_and_gradients(theta[self.mean_slice])
-        # use the cholesky decomp to get the covariance inverse
+        # use the Cholesky decomp to get the covariance inverse
         L = cholesky(K_xx)
         iK = solve_triangular(L, eye(L.shape[0]), lower=True)
         iK = iK.T @ iK
-        # Use the Cholesky decomposition of the covariance to find its inverse
         alpha = iK.dot(self.y - mu)
         var = 1.0 / diag(iK)
         LOO = -0.5 * (var * alpha**2 + log(var)).sum()
 
         cov_gradients = []
         c1 = alpha * var
         c2 = 0.5 * var * (1 + var * alpha**2)
@@ -607,16 +604,23 @@
             workers = Pool(n_processes)
             results = workers.map(self.launch_bfgs, starting_positions)
 
         # extract best solution
         solution = sorted(results, key=lambda x: x[1])[0][0]
         return solution
 
+    def __str__(self):
+        L_max = max([len(lb) for lb in self.hyperpar_labels])
+        strings = ["\n>>> [ GpRegressor hyperparameters ]\n"]
+        for lb, val in zip(self.hyperpar_labels, self.hyperpars):
+            strings.append(" " * (L_max - len(lb)) + f"{lb} = {val:.4}\n")
+        return "".join(strings)
+
 
-class MarginalisedGpRegressor(object):
+class MarginalisedGpRegressor:
     def __init__(
         self,
         x,
         y,
         y_err=None,
         hyperparameter_samples=None,
         kernel=SquaredExponential,
@@ -720,16 +724,16 @@
     def __init__(
         self,
         x: ndarray,
         y: ndarray,
         bounds: Sequence,
         y_err: ndarray = None,
         hyperpars: ndarray = None,
-        kernel: Type[CovarianceFunction] = SquaredExponential,
-        mean: Type[MeanFunction] = ConstantMean,
+        kernel: CovarianceFunction = SquaredExponential,
+        mean: MeanFunction = ConstantMean,
         cross_val: bool = False,
         acquisition=ExpectedImprovement,
         optimizer: str = "bfgs",
         n_processes: int = 1,
     ):
         self.x = x if isinstance(x, ndarray) else array(x)
         if self.x.ndim == 1:
@@ -967,16 +971,16 @@
 
     def __init__(
         self,
         y: ndarray,
         y_err: ndarray,
         model_matrix: ndarray,
         parameter_spatial_positions: ndarray,
-        prior_covariance_function: Type[CovarianceFunction] = SquaredExponential,
-        prior_mean_function: Type[MeanFunction] = ConstantMean,
+        prior_covariance_function: CovarianceFunction = SquaredExponential,
+        prior_mean_function: MeanFunction = ConstantMean,
     ):
         if model_matrix.ndim != 2:
             raise ValueError(
                 """
                 [ GpLinearInverter error ]
                 >> 'model_matrix' argument must be a 2D numpy.ndarray
                 """
```

### Comparing `inference-tools-0.9.1/inference/likelihoods.py` & `inference-tools-0.9.2/inference/likelihoods.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,21 +68,51 @@
 
         if (_uncertainties <= 0).any():
             raise ValueError(
                 f"All values in {uncertainties_name} argument must be greater than zero"
             )
 
     @abstractmethod
-    def __call__(self, theta):
+    def _log_likelihood(self, predictions):
         pass
 
     @abstractmethod
-    def gradient(self, theta):
+    def _log_likelihood_gradient(self, predictions, predictions_jacobian):
         pass
 
+    def __call__(self, theta):
+        """
+        Returns the log-likelihood value for the given set of model parameters.
+
+        :param theta: \
+            The model parameters as a 1D ``numpy.ndarray``.
+
+        :returns: \
+            The log-likelihood value.
+        """
+        return self._log_likelihood(predictions=self.model(theta))
+
+    def gradient(self, theta):
+        """
+        Returns the gradient of the log-likelihood with respect to model parameters.
+
+        Using this method requires that the ``forward_model_jacobian`` keyword argument
+        was specified when the instance of the class was created.
+
+        :param theta: \
+            The model parameters as a 1D ``numpy.ndarray``.
+
+        :returns: \
+            The gradient of the log-likelihood as a 1D ``numpy.ndarray``.
+        """
+        return self._log_likelihood_gradient(
+            predictions=self.model(theta),
+            predictions_jacobian=self.model_jacobian(theta),
+        )
+
     def cost(self, theta):
         return -self.__call__(theta)
 
     def cost_gradient(self, theta):
         return -self.gradient(theta)
 
 
@@ -114,45 +144,21 @@
 
         # pre-calculate some quantities as an optimisation
         self.n_data = self.y.size
         self.inv_sigma = 1.0 / self.sigma
         self.inv_sigma_sqr = self.inv_sigma**2
         self.normalisation = -log(self.sigma).sum() - 0.5 * log(2 * pi) * self.n_data
 
-    def __call__(self, theta):
-        """
-        Returns the log-likelihood value for the given set of model parameters.
-
-        :param theta: \
-            The model parameters as a 1D ``numpy.ndarray``.
-
-        :returns: \
-            The log-likelihood value.
-        """
-        prediction = self.model(theta)
-        z = (self.y - prediction) * self.inv_sigma
+    def _log_likelihood(self, predictions):
+        z = (self.y - predictions) * self.inv_sigma
         return -0.5 * (z**2).sum() + self.normalisation
 
-    def gradient(self, theta):
-        """
-        Returns the gradient of the log-likelihood with respect to model parameters.
-
-        Using this method requires that the ``forward_model_jacobian`` keyword argument
-        was specified when the instance of ``GaussianLikelihood`` was created.
-
-        :param theta: \
-            The model parameters as a 1D ``numpy.ndarray``.
-
-        :returns: \
-            The gradient of the log-likelihood as a 1D ``numpy.ndarray``.
-        """
-        prediction = self.model(theta)
-        dF_dt = self.model_jacobian(theta)
-        dL_dF = (self.y - prediction) * self.inv_sigma_sqr
-        return dL_dF.dot(dF_dt)
+    def _log_likelihood_gradient(self, predictions, predictions_jacobian):
+        dL_dF = (self.y - predictions) * self.inv_sigma_sqr
+        return dL_dF @ predictions_jacobian
 
 
 class CauchyLikelihood(Likelihood):
     """
     A class for constructing a Cauchy likelihood function.
 
     :param y_data: \
@@ -178,46 +184,22 @@
         super().__init__(y_data, gamma, "gamma", forward_model, forward_model_jacobian)
 
         # pre-calculate some quantities as an optimisation
         self.n_data = self.y.size
         self.inv_gamma = 1.0 / self.gamma
         self.normalisation = -log(pi * self.gamma).sum()
 
-    def __call__(self, theta):
-        """
-        Returns the log-likelihood value for the given set of model parameters.
-
-        :param theta: \
-            The model parameters as a 1D ``numpy.ndarray``.
-
-        :returns: \
-            The log-likelihood value.
-        """
-        prediction = self.model(theta)
-        z = (self.y - prediction) * self.inv_gamma
+    def _log_likelihood(self, predictions):
+        z = (self.y - predictions) * self.inv_gamma
         return -log(1 + z**2).sum() + self.normalisation
 
-    def gradient(self, theta):
-        """
-        Returns the gradient of the log-likelihood with respect to model parameters.
-
-        Using this method requires that the ``forward_model_jacobian`` keyword argument
-        was specified when the instance of ``CauchyLikelihood`` was created.
-
-        :param theta: \
-            The model parameters as a 1D ``numpy.ndarray``.
-
-        :returns: \
-            The gradient of the log-likelihood as a 1D ``numpy.ndarray``.
-        """
-        prediction = self.model(theta)
-        dF_dt = self.model_jacobian(theta)
-        z = (self.y - prediction) * self.inv_gamma
+    def _log_likelihood_gradient(self, predictions, predictions_jacobian):
+        z = (self.y - predictions) * self.inv_gamma
         dL_dF = 2 * self.inv_gamma * z / (1 + z**2)
-        return dL_dF.dot(dF_dt)
+        return dL_dF @ predictions_jacobian
 
 
 class LogisticLikelihood(Likelihood):
     """
     A class for constructing a Logistic likelihood function.
 
     :param y_data: \
@@ -244,46 +226,22 @@
 
         # pre-calculate some quantities as an optimisation
         self.n_data = self.y.size
         self.scale = self.sigma * (sqrt(3) / pi)
         self.inv_scale = 1.0 / self.scale
         self.normalisation = -log(self.scale).sum()
 
-    def __call__(self, theta):
-        """
-        Returns the log-likelihood value for the given set of model parameters.
-
-        :param theta: \
-            The model parameters as a 1D ``numpy.ndarray``.
-
-        :returns: \
-            The log-likelihood value.
-        """
-        prediction = self.model(theta)
-        z = (self.y - prediction) * self.inv_scale
+    def _log_likelihood(self, predictions):
+        z = (self.y - predictions) * self.inv_scale
         return z.sum() - 2 * log(1 + exp(z)).sum() + self.normalisation
 
-    def gradient(self, theta):
-        """
-        Returns the gradient of the log-likelihood with respect to model parameters.
-
-        Using this method requires that the ``forward_model_jacobian`` keyword argument
-        was specified when the instance of ``LogisticLikelihood`` was created.
-
-        :param theta: \
-            The model parameters as a 1D ``numpy.ndarray``.
-
-        :returns: \
-            The gradient of the log-likelihood as a 1D ``numpy.ndarray``.
-        """
-        prediction = self.model(theta)
-        dF_dt = self.model_jacobian(theta)
-        z = (self.y - prediction) * self.inv_scale
+    def _log_likelihood_gradient(self, predictions, predictions_jacobian):
+        z = (self.y - predictions) * self.inv_scale
         dL_dF = (2 / (1 + exp(-z)) - 1) * self.inv_scale
-        return dL_dF.dot(dF_dt)
+        return dL_dF @ predictions_jacobian
 
 
 def jacobian_not_given(*args):
     raise ValueError(
         """
         The gradient() method of a likelihood class instance was called, however
         the forward_model_jacobian keyword argument was not specified when instance
```

### Comparing `inference-tools-0.9.1/inference/mcmc.py` & `inference-tools-0.9.2/inference/mcmc.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from numpy.random import normal, random, shuffle, seed, randint
 from scipy.linalg import eigh
 
 from inference.pdf import UnimodalPdf, GaussianKDE
 from inference.plotting import matrix_plot, trace_plot, transition_matrix_plot
 
 
-class Parameter(object):
+class Parameter:
     """
     This class is used by the markov-chain samplers in this module
     to manage data specific to each model parameter which is being
     sampled.
 
     The class also adjusts the parameter's proposal distribution
     width automatically as the chain advances in order to ensure
@@ -219,15 +219,15 @@
             self.proposal = self.boundary_proposal
         elif self._non_negative:
             self.proposal = self.abs_proposal
         else:
             self.proposal = self.standard_proposal
 
 
-class MarkovChain(object):
+class MarkovChain:
     """
     Implementation of the metropolis-hastings algorithm using a multivariate-normal
     proposal distribution.
 
     :param func posterior: \
         A function which takes the vector of model parameters as a ``numpy.ndarray``,
         and returns the posterior log-probability.
@@ -1579,15 +1579,15 @@
 
         # build the epsilon selector
         chain.ES.load_items(D)
 
         return chain
 
 
-class EpsilonSelector(object):
+class EpsilonSelector:
     def __init__(self, epsilon):
 
         # storage
         self.epsilon = epsilon
         self.epsilon_values = [copy(epsilon)]  # sigma values after each assessment
         self.epsilon_checks = [0.0]  # chain locations at which sigma was assessed
 
@@ -1646,15 +1646,15 @@
         self.var = float(dictionary["var"])
         self.num = float(dictionary["num"])
         self.accept_rate = float(dictionary["accept_rate"])
         self.chk_int = int(dictionary["chk_int"])
         self.growth_factor = float(dictionary["growth_factor"])
 
 
-class ChainPool(object):
+class ChainPool:
     def __init__(self, objects):
         self.chains = objects
         self.pool_size = len(self.chains)
         self.pool = Pool(self.pool_size)
 
     def advance(self, n):
         self.chains = self.pool.map(
@@ -1703,15 +1703,15 @@
             chain.probs[-1] = D["probability"] * chain.inv_temp
 
         # return the local chain object
         elif task == "send_chain":
             connection.send(chain)
 
 
-class ParallelTempering(object):
+class ParallelTempering:
     """
     A class which enables 'parallel tempering', a sampling algorithm which
     advances multiple Markov-chains in parallel, each with a different
     'temperature', with a probability that the chains will exchange their
     positions during the advancement.
 
     The 'temperature' concept introduces a transformation to the distribution
@@ -2020,15 +2020,15 @@
         Trigger a shutdown event which tells the processes holding each of
         the chains to terminate.
         """
         self.shutdown_evt.set()
         [p.join() for p in self.processes]
 
 
-class EnsembleSampler(object):
+class EnsembleSampler:
     """
     ``EnsembleSampler`` is an implementation of the affine-invariant ensemble sampler
     proposed by Goodman & Weare. This algorithm is based on an 'ensemble' of points
     in the parameter space referred to as 'walkers'. Proposed updates to the position
     of each walker are generated based on the positions of the other walkers in the
     ensemble in such a way that the performance of the algorithm is unaffected by
     affine-transformations of the parameter space.
```

### Comparing `inference-tools-0.9.1/inference/mean.py` & `inference-tools-0.9.2/inference/mean.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/inference/pdf.py` & `inference-tools-0.9.2/inference/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from scipy.optimize import minimize, minimize_scalar, differential_evolution
 from warnings import warn
 from itertools import product
 from functools import reduce
 import matplotlib.pyplot as plt
 
 
-class DensityEstimator(object):
+class DensityEstimator:
     """
     Parent class for the 1D density estimation classes GaussianKDE and UnimodalPdf.
     """
 
     def __init__(self):
         self.lwr_limit = None
         self.upr_limit = None
@@ -542,15 +542,15 @@
 
         :param float frac: Fraction of total probability contained by the desired interval(s).
         :return: A list of tuples which specify the intervals.
         """
         return sample_hdi(self.s, frac, allow_double=True)
 
 
-class KDE2D(object):
+class KDE2D:
     def __init__(self, x=None, y=None):
 
         self.x = array(x)
         self.y = array(y)
         # very simple bandwidth estimate
         s_x, s_y = self.estimate_bandwidth(self.x, self.y)
         self.q_x = 1.0 / (sqrt(2) * s_x)
@@ -660,15 +660,15 @@
     # return the split interval if the width reduction is non-trivial:
     if allow_double and w2 < w1 * 0.99:
         return I1, I2
     else:
         return r1
 
 
-class dbl_interval_length(object):
+class dbl_interval_length:
     def __init__(self, sample, fraction):
         self.sample = sort(sample)
         self.f = fraction
         self.N = len(sample)
         self.L = int(self.f * self.N)
         self.space = self.N - self.L
         self.max_length = self.sample[-1] - self.sample[0]
```

### Comparing `inference-tools-0.9.1/inference/plotting.py` & `inference-tools-0.9.2/inference/plotting.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/inference/posterior.py` & `inference-tools-0.9.2/inference/posterior.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 .. moduleauthor:: Chris Bowman <chris.bowman.physics@gmail.com>
 """
 
 
-class Posterior(object):
+class Posterior:
     """
     Class for constructing a posterior distribution object for a given likelihood and prior.
 
     :param callable likelihood: \
         A callable which returns the log-likelihood probability when passed a vector of
         the model parameters.
```

### Comparing `inference-tools-0.9.1/inference/priors.py` & `inference-tools-0.9.2/inference/priors.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Union, Iterable
 
 from numpy import array, log, pi, zeros, concatenate, float64, where
 from numpy.random import normal, exponential, uniform
 from itertools import chain
 
 
-class JointPrior(object):
+class JointPrior:
     """
     A class which combines multiple prior distribution objects into a single
     joint-prior distribution object.
 
     :param components: \
         A list of prior distribution objects (e.g. GaussianPrior, ExponentialPrior)
         which will be combined into a single joint-prior object.
@@ -113,15 +113,15 @@
         """
         sample = zeros(self.n_variables)
         for c in self.components:
             sample[c.variables] = c.sample()
         return sample
 
 
-class BasePrior(object):
+class BasePrior:
     @staticmethod
     def check_variables(variable_inds: Union[int, Iterable[int]], n_vars: int):
         if not isinstance(variable_inds, (int, Iterable)):
             raise TypeError("'variable_inds' must be an integer or list of integers")
 
         if isinstance(variable_inds, int):
             variable_inds = [variable_inds]
```

### Comparing `inference-tools-0.9.1/inference_tools.egg-info/PKG-INFO` & `inference-tools-0.9.2/inference_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-tools
-Version: 0.9.1
+Version: 0.9.2
 Summary: A collection of python tools for Bayesian data analysis
 Home-page: https://github.com/C-bowman/inference-tools
 Author: Chris Bowman
 Author-email: chris.bowman.physics@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/C-bowman/inference-tools
 Project-URL: Tracker, https://github.com/C-bowman/inference-tools/issues
```

### Comparing `inference-tools-0.9.1/inference_tools.egg-info/SOURCES.txt` & `inference-tools-0.9.2/inference_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/setup.cfg` & `inference-tools-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/gp/test_GpLinearInverter.py` & `inference-tools-0.9.2/tests/gp/test_GpLinearInverter.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/gp/test_GpOptimiser.py` & `inference-tools-0.9.2/tests/gp/test_GpOptimiser.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/mcmc/mcmc_utils.py` & `inference-tools-0.9.2/tests/mcmc/mcmc_utils.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/mcmc/test_ensemble.py` & `inference-tools-0.9.2/tests/mcmc/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/mcmc/test_gibbs.py` & `inference-tools-0.9.2/tests/mcmc/test_gibbs.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/mcmc/test_hamiltonian.py` & `inference-tools-0.9.2/tests/mcmc/test_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/mcmc/test_pca.py` & `inference-tools-0.9.2/tests/mcmc/test_pca.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/test_covariance.py` & `inference-tools-0.9.2/tests/test_covariance.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 @pytest.mark.parametrize(
     "cov",
     [
         SquaredExponential(),
         RationalQuadratic(),
         WhiteNoise(),
         RationalQuadratic() + WhiteNoise(),
-        ChangePoint(),
+        ChangePoint(kernels=[SquaredExponential, SquaredExponential]),
+        ChangePoint(kernels=[SquaredExponential, SquaredExponential]) + WhiteNoise(),
     ],
 )
 def test_covariance_and_gradients(cov):
     x, y = create_data()
     cov.pass_spatial_data(x)
     cov.estimate_hyperpar_bounds(y)
     low = array([a for a, b in cov.bounds])
```

### Comparing `inference-tools-0.9.1/tests/test_likelihoods.py` & `inference-tools-0.9.2/tests/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/test_pdf.py` & `inference-tools-0.9.2/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/test_plotting.py` & `inference-tools-0.9.2/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/test_posterior.py` & `inference-tools-0.9.2/tests/test_posterior.py`

 * *Files identical despite different names*

### Comparing `inference-tools-0.9.1/tests/test_priors.py` & `inference-tools-0.9.2/tests/test_priors.py`

 * *Files identical despite different names*

