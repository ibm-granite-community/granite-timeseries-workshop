---
title: Granite Timeseries Workshop Lab 6
description: Retail Sales Forecasting using the M5 dataset with Granite Time Series - Few-shot finetuning, evaluation, and visualization
logo: images/ibm-blue-background.png
---

# Retail Sales Forecasting using the M5 dataset with Granite Time Series - Few-shot finetuning, evaluation, and visualization

In this tutorial, we will explore [timeseries forecasting](https://www.ibm.com/think/insights/time-series-forecasting) using the [IBM Granite](https://ibm.com/granite) Timeseries model to predict retail sales. We will cover key techniques such as few-shot forecasting and fine-tuning. We are using [M5 datasets](https://drive.google.com/drive/folders/1D6EWdVSaOtrP1LEFh1REjI3vej6iUS_4?usp=sharing) from the official [M-Competitions repository](https://github.com/Mcompetitions/M5-methods) to forecast future sales aggregated by state. The aim of this recipe is to showcase how to use a pre-trained time series foundation model for multivariate forecasting and explores various features available with Granite Time Series Foundation Models.

This lab uses TinyTimeMixers (TTMs), which are compact pre-trained models for Multivariate Time-Series Forecasting, open-sourced by IBM Research. With less than 1 Million parameters, TTM introduces the notion of the first-ever "tiny" pre-trained models for Time-Series Forecasting. TTM outperforms several popular benchmarks demanding billions of parameters in zero-shot and few-shot forecasting and can easily be fine-tuned for multivariate forecasts.

## Prerequisites

This lab is a [Jupyter notebook](https://jupyter.org/). Please follow the instructions in [pre-work](https://ibm-granite-community.github.io/granite-timeseries-workshop/pre-work/) to run the lab.

## Lab

[![Retail Forecasting using M5 Sales Data Few-shot, Fine-tuning, Evaluation, and Visualization notebook](https://badgen.net/badge/icon/github?icon=github&label=View%20on "View on GitHub")]({{ config.repo_url }}/blob/{{ git.commit }}/notebooks/M5_retail_sales_forecasting.ipynb){:target="_blank"}
[![Retail Forecasting using M5 Sales Data Few-shot, Fine-tuning, Evaluation, and Visualization notebook](https://colab.research.google.com/assets/colab-badge.svg "Open In Colab")]({{ extra.colab_url }}/blob/{{ git.commit }}/notebooks/M5_retail_sales_forecasting.ipynb){:target="_blank"}

To run the notebook from your command line in Jupyter using the active virtual environment from the pre-work, run:

jupyter notebook notebooks/Bike_Sharing_Finetuning_with_Exogenous.ipynb

The path of the notebook file above is relative to the granite-workshop folder from the git clone in the pre-work.

## Credits

This notebook is a modified version of the IBM Granite Community [Retail Forecasting using M5 Sales Data Few-shot, Fine-tuning, Evaluation, and Visualization](https://github.com/ibm-granite-community/granite-timeseries-cookbook/blob/main/recipes/Time_Series/M5_retail_sales_forecasting.ipynb) notebook. Refer to the [IBM Granite Community](https://github.com/ibm-granite-community) for the official notebooks.
