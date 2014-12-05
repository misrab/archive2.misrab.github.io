---
title: Does Unsupervised Learning Exist?
layout: blog
---

# An Introduction to Hidden Markov Models

Does Unsupervised Learning Exist?

## Introduction

// explain sup vs unsup

// thesis

If data is truly unlabeled, forever, then there is little more 
we can do than describe what we see. This is a cluster, this is the 
variance, etc.

If we're going beyond pure description, to some sort of task like prediction, 
then we can define a loss function i.e. how well are we doing. In that sense, the 
scenario is actually as follows: we start with truly unsupervised data, but then 
upon carrying out our desired task, we have a measure of how well we're doing. 
The more of this task we carry out, the more information we have about our success _given_ 
our loss function. **Hence one can think of the task as providing soft labels over the 
data**.

In the traditional supervised setting we have firstly information about each _point_, 
and secondly _deterministic_ information (i.e. presumably certain labels on each point). 
In the relaxed supervised setting I am proposing, we have possibly pointwise information, but more generally aggregate information through aggregate loss (i.e. how well we've been 
doing our task so far over the data, or on new points). Secondly the loss function may be 
a soft version of "right and wrong" labelling.

This is all very high level as I'm still formulating the concept. Here we'll try and 
do some preliminary investigation, and see how much we can formalize (at least for the moment).