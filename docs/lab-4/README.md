---
title: Granite Timeseries Workshop Lab 4
description: Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation
logo: images/ibm-blue-background.png
---

# Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation

TinyTimeMixers (TTMs) are compact pre-trained models for Multivariate Time-Series Forecasting, open-sourced by IBM Research. With less than 1 Million parameters, TTM introduces the notion of the first-ever "tiny" pre-trained models for Time-Series Forecasting. TTM outperforms several popular benchmarks demanding billions of parameters in zero-shot and few-shot forecasting and can easily be fine-tuned for multivariate forecasts.

In this lab, we cover zero-shot forecasting, as well as fine-tuning. This example makes use of the [Kaggle bike sharing dataset](https://www.kaggle.com/datasets/lakshmi25npathi/bike-sharing-dataset) which contains bikes rental demand with weather and seasonal information.

## Prerequisites

This lab is a [Jupyter notebook](https://jupyter.org/). Please follow the instructions in [pre-work](https://ibm-granite-community.github.io/granite-timeseries-workshop/pre-work/) to run the lab.

## Lab

[![Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation notebook](https://badgen.net/badge/icon/github?icon=github&label=View%20on "View on GitHub")]({{ config.repo_url }}/blob/{{ git.commit }}/notebooks/Bike_Sharing_Finetuning_with_Exogenous.ipynb){:target="_blank"}
[![Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation notebook](https://colab.research.google.com/assets/colab-badge.svg "Open In Colab")]({{ extra.colab_url }}/blob/{{ git.commit }}/notebooks/Bike_Sharing_Finetuning_with_Exogenous.ipynb){:target="_blank"}

To run the notebook from your command line in Jupyter using the active virtual environment from the pre-work, run:

jupyter notebook notebooks/Bike_Sharing_Finetuning_with_Exogenous.ipynb

The path of the notebook file above is relative to the granite-workshop folder from the git clone in the pre-work.

## Credits

This notebook is a modified version of the IBM Granite Community [Bike Sharing Forecasting Zero-shot, Fine-tuning, and Performance Evaluation](https://github.com/ibm-granite-community/granite-timeseries-cookbook/blob/main/recipes/Time_Series/Bike_Sharing_Finetuning_with_Exogenous.ipynb) notebook. Refer to the [IBM Granite Community](https://github.com/ibm-granite-community) for the official notebooks.
