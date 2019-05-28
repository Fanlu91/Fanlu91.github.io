---
title: Machine learning basics 01
date: 2019-05-22 18:58:05
tags: 
- machine learning
---

## Machine learning examples:
- Database mining 
- Applications can't program by hand
  autonomous helicopter, handwriting recognition, NLP, computer vision.
- Self-customizing programs
  product recommendation
- Understand human learning 
  brain, real AI

## What is machine learning

By Arthur Samuel 1959. Machine learning: Field of study that gives computer the ability to learn without being explicitly programmed.
By Tom Mitchell 1998. A computer program is said to learn from **experience E** with respect to some **task T** and some **performance measure P**, if its performance on T, as measured by P, **improves** with experience E. 

Example: playing checkers.

E = the experience of playing many games of checkers
T = the task of playing checkers.
P = the probability that the program will win the next game.

## Types of machine learning algorithms
- Supervised learning, we are going to teach the computer
  The term Supervised Learning refers to the fact that we gave the algorithm a data set in which the, called, "right answers" were given.
  - classification problem，trying to map input variables into discrete categories（discrete value 离散值）
  - regression problem，predict results within a continuous output（scalar value 标量值）
- Unsupervised learning, let the computer learn by itself
  Unsupervised learning allows us to approach problems with little or no idea what our results should look like. We can derive structure from data where we don't necessarily know the effect of the variables.
  - Clustering, automatically group
  - Non-clustering, Cocktail Party Algorithm", allows you to find structure in a chaotic environment.
  
- Other, reinforcement learning / recommender systems