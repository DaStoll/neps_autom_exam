# Neural Pipeline Search (NePS)

[![PyPI version](https://img.shields.io/pypi/v/neural-pipeline-search?color=informational)](https://pypi.org/project/neural-pipeline-search/)
[![Python versions](https://img.shields.io/pypi/pyversions/neural-pipeline-search)](https://pypi.org/project/neural-pipeline-search/)
[![License](https://img.shields.io/pypi/l/neural-pipeline-search?color=informational)](LICENSE)
[![Tests](https://github.com/automl/neps/actions/workflows/tests.yaml/badge.svg)](https://github.com/automl/neps/actions)

Welcome to NePS, a powerful and flexible Python library for hyperparameter optimization (HPO) and neural architecture search (NAS) with its primary goal: enable HPO adoption in practice for deep learners!

NePS houses recently published and some more well-established algorithms that are all capable of being run massively parallel on any distributed setup, with tools to analyze runs, restart runs, etc.


## Key Features

In addition to the common features offered by traditional HPO and NAS libraries, NePS stands out with the following key features:

1. [**Hyperparameter Optimization (HPO) With Prior Knowledge:**](neps_examples/template/priorband_template.py)
    - NePS excels in efficiently tuning hyperparameters using algorithms that enable users to make use of their prior knowledge within the search space. This is leveraged by the insights presented in:
        - [PriorBand: Practical Hyperparameter Optimization in the Age of Deep Learning](https://arxiv.org/abs/2306.12370)
        - [πBO: Augmenting Acquisition Functions with User Beliefs for Bayesian Optimization](https://arxiv.org/abs/2204.11051)

2. [**Neural Architecture Search (NAS) With Context-free Grammar Search Spaces:**](neps_examples/basic_usage/architecture.py)
    - NePS is equipped to handle context-free grammar search spaces, providing advanced capabilities for designing and optimizing architectures. this is leveraged by the insights presented in:
        - [Construction of Hierarchical Neural Architecture Search Spaces based on Context-free Grammars](https://arxiv.org/abs/2211.01842)

3. [**Easy Parallelization:**](docs/parallelization.md)
    - NePS simplifies the parallelization of optimization tasks. Whether experiments are running on a single machine or a distributed computing environment.

4. [**Resume Runs After Termination:**](docs/parallelization.md)
    - NePS allows users to easily resume optimization runs after termination, providing a convenient and efficient workflow for long-running experiments.

5. [**Seamless User Code Integration:**](neps_examples/template/)
    - NePS's modular design ensures flexibility and extensibility. Integrate NePS effortlessly into existing machine learning workflows.
