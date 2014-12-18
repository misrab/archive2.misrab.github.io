---
title: Neural Networks - Basics
layout: blog
excerpt: |
  In the second part of this series, I look at the fundamental 
  concept of variation
---


# Neural Networks - Basics

## Introduction

Writing explicit programs to accomplish sophisticated tasks can quickly become 
intractable. For example, it may be evident how to tell a computer to change screen 
color based on which user is logged in: this is definite. Writing a definite program to 
recognize pigeons in a photo is not obvious. The core issue is that it is difficult to 
determine what set of rules is optimal, and even if we knew them it would be a lot of work 
to hard code them all.

Machine learning is then a further level of abstraction: we hard code the **process of 
learning** more generally, and hope the algorithm identifies a good set of rules in [classification](http://en.wikipedia.org/wiki/Statistical_classification) or [regression](http://en.wikipedia.org/wiki/Regression_analysis), based on labelled data (supervised learning), unlabelled data (unsupervised learning), or a mixture of both.

Neural networks are a class of these learning algorithms. Let's look into why we 
might care about them at all, given some other possible techniques.

## Context

As we said, we want some sort of algorithm that's good at learning rules from data. 
Probability is a good framework for this since data is seldom black or white: pigeons 
have a whole range of sizes, but some sizes are more intuitively likely than others.

## Architecture

- include nonlinearity here

## Layers

## Gradient Problems


## Conclusion

## Acknowledgements

This series of posts is heavily inspired by the writings of 
[Michael Nielsen](http://neuralnetworksanddeeplearning.com/), 
[Richard Socher](http://www.socher.org/index.php/Main/HomePage), and 
[Christopher Olah](http://colah.github.io/), which I highly recommend.