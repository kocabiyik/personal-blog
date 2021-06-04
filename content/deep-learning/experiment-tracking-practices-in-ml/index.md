---
title: Experiment Tracking Practices in ML
author: ''
date: '2021-06-03'
slug: experiment-tracking-practices-in-ml
categories:
  - Machine Learning
tags: []
topic: 'MLOps'
---

If you build machine learning model for practical applications, it would be a good 
strategy to try different strategies until you get a **good enough** model. 
One of the most  useful practice is tracking your experiments.  

## Why Keeping a Experiment Records?

You may need to:  
- reproduce a similar model.  
- remember the hyperparameters you set.  
- analyze different experiments.  
- etc.  

## What to record?

It is the data about the training process.  

- **Hyperpameters** like Learning Rate, Batch Size, Number of Epochs, Optimizer, ...  
- **Metrics** like MSE, IOU, F1 Score etc.
It is a good practice to record them for both train and validation datasets.  
- **Training Data Source**  
- **Code Version**  

## How to Record?

### Manual Recording
An easy but a bad solution.

### Logging in the Training Process
My solution was this:   

- Keep all the metadata I care about in a python dictionary, and export it as a YAML file during the training process.
- Inspect the experiments because YAML file format is human readable.  
- YAML files can also be used programmatically. For example, if I pass `--continue_train` argument to my entrypoint (example: `python3 train.py --continue_train`), it looks up the file location of the best model (the one with the highest validation metric) by using the YAML file and initializes weights of the model accordingly.  

### A Dedicated Tool

I am now trying experiment tracking tools and my first impression is good.  

Pros:
- Easy integration  
- Easy sharing with team members  
- Built-in dashboards, easy monitoring  
- Live monitoring  
- and more  