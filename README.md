# [Edward][http://edwardlib.org]

Describe the matter of Edward with TensorFlow.

## What is Edward

[Edward][http://edwardlib.org] is a Python library for probabilistic modeling[概率建模], inference[推理], and criticism[评论]. It is a testbed[实验台] for fast experimentation and research with probabilistic models, ranging from classical hierarchical models[分层模式] on small data sets to complex deep probabilistic models on large data sets. Edward fuses[使融合] three fields: Bayesian statistics and machine learning, deep learning, and probabilistic programming.

## Getting Started Edward

### Installation

To install the latest stable version, run

 ` pip install edward `

To install the latest development version, run

` pip install -e "git+https://github.com/blei-lab/edward.git#egg=edward" `

See the [troubleshooting page][http://edwardlib.org/troubleshooting] for detailed installation instruction.

#### Basic Installation

**Note: TensorFlow v1.1.0rc0 made breaking API changes. Edward's latest stable version only supports up to TensorFlow v1.0.1. If you aim to use TensorFlow v1.1.0rc0 or beyond, use the following development branch of Edward:**

``` pip install -e "git+https://github.com/blei-lab/edward.git@bugfix/issue-451#egg=edward"``` 

Edward depends on

* NumPy (>=1.7)
* Six (>=1.1.0)
* TensorFlow (>=1.0.0a0, <=1.0.1)

Installing `edward` by default also installs `numpy` and `six` if they are not available (or are out-of-date in your system).

Installing `edward` does not automatically install TensorFlow (or update an existing TensorFlow verion). We recommend installing it via

``` pip install tensorflow ```

To use Edward with GPUs, install `tensorflow-gpu` instead of `tensorflow` as

``` pip install tensorflow-gpu ```

See TensorFlow's [installation instructions][https://www.tensorflow.org/install/] for details, including how to setup up NV