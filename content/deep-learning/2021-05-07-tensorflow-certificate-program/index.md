---
title: 'Review: TensorFlow Certificate Program'
author: Imran Kocabiyik
date: '2021-05-07'
slug: tensorflow-certificate-program
categories:
  - Deep Learning
tags:
  - tensorflow
topic: Reviews
---

I just received the TensorFlow Developer Certificate.

It is a new program (announced in March 2020), and I think I am one of the early-holders of the certificate. Here are my impressions and expectations:


## Why Choosing TensorFlow Framework?
To have hands-on experience in a deep learning framework, and I have chosen TensorFlow. It is for two reasons:

In general, it is the most popular DL framework.
It is mostly used in the industry than in academia. So, it fits my profile.
Is the Certificate Worth Paying?
The exam costs $100 and takes five hours to complete.

I haven't proven it yet, but I would expect that it would be useful for demonstrating coding skills.

## The Exam Preparation
The certificate program suggests TensorFlow in Practice Specialization in Coursera. The specialization contains four courses:

Introduction to TensorFlow for Artificial Intelligence, Machine Learning, and Deep Learning
Convolutional Neural Networks in TensorFlow
Natural Language Processing in TensorFlow
Sequences, Time Series and Prediction
The specialization program assumes that you have a good understanding of deep learning because this specialization is not about theory but application.

Deep Learning with Python by François Chollet can also be a useful resource.

## Technical Requirements for Taking the Exam
You can take the exam with a PC. They consider training the models can take time, but 5 hours should be sufficient.

I purchased the exam with my MacBook because I need to upload a copy of my passport and take a photo with the webcam. However, I started the certification exam on my workstation with a GPU. In summary, GPU is not crucial, but speed doesn't hurt. 🐢 🐇

You need PyCharm for the exam. The exam plugin creates an environment for you.

## Some Suggestions
For preparing the exam:

Better to start with a blank notebook and start coding from scratch, instead of just running the cells in the given in a tutorial.
Finding new challenges you may like. For example, if you have a binary classification problem in a tutorial,  you may consider finding another problem in the real world and work on it.
Explore documentation, change the network architecture, observe how it is changing the results. If you see a new term for the first time (for example, Huber Loss function was new for me), do some quick research and check how it is working.
During the exam:

To use time efficiently, you may consider creating checkpoints (saving weights in an h5 file and initializing the weights before a new training. Note that this may not work if you change the network architecture.)
You can also use other tools if you feel more comfortable. For example, I developed the model in Jupyter Lab, and then I moved the project into PyCharm.
I hope this helps anyone who might consider taking it.

