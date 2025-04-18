---
title: Granite Timeseries Workshop Lab 3
description: Energy Demand Forecasting - Few-shot Fine-tuning
logo: images/ibm-blue-background.png
---

# Energy Demand Forecasting - Few-shot Fine-tuning

TinyTimeMixers (TTMs) are compact pre-trained models for Multivariate Time-Series Forecasting, open-sourced by IBM Research. With less than 1 Million parameters, TTM introduces the notion of the first-ever "tiny" pre-trained models for Time-Series Forecasting. TTM outperforms several popular benchmarks demanding billions of parameters in zero-shot and few-shot forecasting and can easily be fine-tuned for multi-variate forecasts.

In this lab, we move beyond zero-shot prediction to few-shot fine-tuning and prediction. We use a real-world dataset containing energy demand data from Spain.

## Prerequisites

This lab is a [Jupyter notebook](https://jupyter.org/). Please follow the instructions in [pre-work](https://ibm-granite-community.github.io/granite-timeseries-workshop/pre-work/) to run the lab.

## Lab

[![Energy Demand Forecasting - Few-shot Fine-tuning notebook](https://badgen.net/badge/icon/github?icon=github&label=View%20on "View on GitHub")]({{ config.repo_url }}/blob/{{ git.commit }}/notebooks/Few-shot_Finetuning_and_Evaluation.ipynb){:target="_blank"}
[![Energy Demand Forecasting - Few-shot Fine-tuning notebook](https://colab.research.google.com/assets/colab-badge.svg "Open In Colab")]({{ extra.colab_url }}/blob/{{ git.commit }}/notebooks/Few-shot_Finetuning_and_Evaluation.ipynb){:target="_blank"}

To run the notebook from your command line in Jupyter using the active virtual environment from the pre-work, run:

jupyter notebook notebooks/Few-shot_Finetuning_and_Evaluation.ipynb

The path of the notebook file above is relative to the granite-workshop folder from the git clone in the pre-work.

## Credits

This notebook is a modified version of the IBM Granite Community [Energy Demand Forecasting - Few-shot Fine-tuning](https://github.com/ibm-granite-community/granite-timeseries-cookbook/blob/main/recipes/Time_Series/Few-shot_Finetuning_and_Evaluation.ipynb) notebook. Refer to the [IBM Granite Community](https://github.com/ibm-granite-community) for the official notebooks.
