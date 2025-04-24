---
title: Granite Time Series Workshop Pre-work
description: Preparation for the Granite Timeseries Workshop
logo: images/ibm-blue-background.png
---

# Pre-work

The labs in the workshop are [Jupyter notebooks](https://jupyter.org/). The notebooks can be run on your computer or remotely on the [Google Colab](https://colab.research.google.com) service. Check out [Running the Granite Notebooks](#running-the-granite-notebooks) section on how to setup the way you want to run the notebooks.

## Running the Granite Notebooks

The notebooks can be run:

- [Locally on your computer](#running-the-granite-notebooks-locally) OR
- [Remotely on the Google Colab service](#running-the-granite-notebooks-remotely-colab)

Follow the instructions in one of the sections that follow on how you would like to run the notebooks.

## Running the Granite Notebooks Locally

It is recommended if you want to run the lab notebooks locally on your computer that you have:

- A computer or laptop
- Knowledge of [Git](https://git-scm.com/) and [Python](https://www.python.org/)

If not, then it recommended to go to the [Running the Granite Notebooks Remotely (Colab)](#running-the-granite-notebooks-remotely-colab) section instead.

Running the lab notebooks locally on your computer requires the following steps:

- [Local Prerequisites](#local-prerequisites)
- [Clone the Granite Timeseries Workshop Repository](#clone-the-granite-timeseries-workshop-repository)
- [Serving the Granite AI Models](#serving-the-granite-ai-models)
- [Install Jupyter](#install-jupyter)

### Local Prerequisites

- Git
- Python 3.10, 3.11, or 3.12

### Clone the Granite Timeseries Workshop Repository

Clone the workshop repo and cd into the repo directory.

```shell
git clone https://github.com/IBM/granite-timeseries-workshop.git
cd granite-timeseries-workshop
```

### Serving the Granite AI Models

<!-- Which timeseries labs need to be served by an AI model runtime? -->

[Lab 1: Energy Demand Forecasting Basic Inference](../lab-1/README.md), [Lab 2: Energy Demand Forecasting Preprocessing and Performance Evaluation](../lab-2/README.md), [Lab 3: Energy Demand Forecasting Few-shot Fine-tuning](../lab-3/README.md), [Lab 4: Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation](../lab-4/README.md), [Lab 5: Getting Started with Watson X AI SDK](../lab-5/README.md), and [Lab 6: Retail Forecasting using M5 Sales Data Few-shot, Fine-tuning, Evaluation, and Visualization](../lab-6/README.md), require Granite models to be served by an AI model runtime so that the models can be invoked or called.

#### Replicate AI Cloud Platform

[Replicate](https://replicate.com/) is a cloud platform that will host and serve AI models for you.

1. Create a [Replicate](https://replicate.com/) account. You will need a [GitHub](https://github.com/) account to do this.

1. Add credit to your Replicate Account (optional). To remove a barrier to entry to try the Granite models on the Replicate platform, use [this link](https://replicate.com/invites/a8717bfe-2f3d-4a52-88ed-1356231cdf03) to add a small amount of credit to your Replicate account.

1. Create a Replicate [API Token](https://replicate.com/account/api-tokens).

1. Set your Replicate API Token as an environment variable in your terminal where you will run the notebook:

    ```shell
    export REPLICATE_API_TOKEN=<your_replicate_api_token>
    ```

### Install Jupyter

!!! note "Use a virtual environment"
    Before installing dependencies and to avoid conflicts in your environment, it is advisable to use a [virtual environment (venv)](https://docs.python.org/3/library/venv.html).

1. Create virtual environment:

    ```shell
    python3 -m venv --upgrade-deps --clear venv
    ```

1. Activate the virtual environment by running:

    ```shell
    source venv/bin/activate
    ```

1. Install Jupyter notebook in the virtual environment:

    ```shell
    python3 -m pip install --require-virtualenv notebook ipywidgets
    ```

    For more information, see the [Jupyter installation instructions](https://jupyter.org/install)

1. To open a notebook in Jupyter (in the active virtual environment), run:

    ```shell
    jupyter notebook <notebook-file-path>
    ```

## Running the Granite Notebooks Remotely (Colab)

Running the lab notebooks remotely using [Google Colab](https://colab.research.google.com) requires the following steps:

- [Colab Prerequisites](#colab-prerequisites)
- [Serving the Granite AI Models for Colab](#serving-the-granite-ai-models-for-colab)

### Colab Prerequisites

- [Google Colab](https://colab.research.google.com) requires a Google account that you're logged into

### Serving the Granite AI Models for Colab

<!-- Which timeseries labs need to be served by an AI model runtime? -->

[Lab 1: Energy Demand Forecasting Basic Inference](../lab-1/README.md), [Lab 2: Energy Demand Forecasting Preprocessing and Performance Evaluation](../lab-2/README.md), [Lab 3: Energy Demand Forecasting Few-shot Fine-tuning](../lab-3/README.md), [Lab 4: Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation](../lab-4/README.md), [Lab 5: Getting Started with Watson X AI SDK](../lab-5/README.md), and [Lab 6: Retail Forecasting using M5 Sales Data Few-shot, Fine-tuning, Evaluation, and Visualization](../lab-6/README.md), require Granite models to be served by an AI model runtime so that the models can be invoked or called.

#### Replicate AI Cloud Platform for Colab

[Replicate](https://replicate.com/) is a cloud platform that will host and serve AI models for you.

1. Create a [Replicate](https://replicate.com/) account. You will need a [GitHub](https://github.com/) account to do this.

1. Add credit to your Replicate Account (optional). To remove a barrier to entry to try the Granite Code models on the Replicate platform, use [this link](https://replicate.com/invites/a8717bfe-2f3d-4a52-88ed-1356231cdf03) to add a small amount of credit to your Replicate account.

1. Create a Replicate [API Token](https://replicate.com/account/api-tokens).

1. Add your Replicate API Token to the Colab Secrets manager to securely store it. Open [Google Colab](https://colab.research.google.com) and click on the 🔑 Secrets tab in the left panel. Click "New Secret" and enter `REPLICATE_API_TOKEN` as the key, and paste your token into the value field. Toggle the button on the left to allow notebook access to the secret.
