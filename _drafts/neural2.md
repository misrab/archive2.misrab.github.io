---
title: Neural Networks (2) - Basics
layout: blog
excerpt: |
  In the second part of this series, I look at the fundamental 
  concept of variation
---


# Neural Networks - Basics

## Introduction

In our last post we spoke about the general context of neural networks,
namely machine learning algorithms. The problem being solved is one of abstracting
rule definitions in solving a problem away from the programmer.

We also noted that neural networks might stand out in their ability to identify 
useful feature transformations automatically, which would serve this overarching
purpose.

Here I'll describe the fundamentals of neural network architecture, and why 
this architecture might be useful.

## Universality

Let start by examining what a neural network can theoretically do. Remember, the problem at hand is to take "some" input, and say something useful about it. We might want to 
group some inputs together, for example. In the extreme, most fine-grained case, we might 
want to distinguish between _every_ possible input. All other problems are a subset of this extreme case. So let's see if a neural network can do this.

We can translate information into binary format. For example we could say that "red" is 
$0010$ and blue is $0001$. More compactly we could use $0$ and $1$. [Information Theory](http://en.wikipedia.org/wiki/Information_theory) is a fascinating field. Let's call the digits of a given input $x_0, x_1, x_2...$. In the first "red" example, we have $x_0=0, x_1=1...$. A neural network is comprised of nodes (I avoid terminology like "neurons" as much as I can, since I consider the problem of connecting this architecture to the human brain a whole other area of research). These nodes are organised into an input layer, an output layer, and one or more hidden layers. Let's consider one hidden layer first:

![one layer]({{ site.url }}/images/neural2/1.svg)

The approach is as follows. If we want to distinguish every possible input, we need an output node for each possible input, to say "yes" if we got that input. Ask yourself, do we have enough output neurons above, if each input node is a bit?

The answer is no: there are $2 \times 2 \times 2 = 8$ possible combinations of three bits, so in reality we'll need $8$ output neurons in the above example, so let's pretend that we do. Next, what do the connections represent? These can be any function we like. We could go so far as to manually set all connections to return $0$. For instance if $f_{i,j}$ is the function from input node $x_i$ to hidden layer node $h_j$, we could set them all to $0$. More interestingly, we could set them to the indicator function $\mathbb{1} (i=j)$. In other words, $h_i$ just checks to see if $x_i$ is $1$. The output layer then combines these for all possible inputes. For example $o_0$ could be the indicator that the first bit is $1$ and all others are $0$.

Put briefly, neural networks are universal computation machines on the input, at least in theory (we've said nothing of efficiency).

## Non-linearity & Learning

It makes sense to parametrise the connecting functions, rather than specify each one individually. The idea is that we can "learn" the parameters that accomplish a given objective function best.


## Notation




## Conclusion

## Acknowledgements

This series of posts is heavily inspired by the writings of 
[Michael Nielsen](http://neuralnetworksanddeeplearning.com/), 
[Richard Socher](http://www.socher.org/index.php/Main/HomePage), and 
[Christopher Olah](http://colah.github.io/), to whom much credit is due. Some of the 
statistical intuition is also influenced by [Trevor Hastie and Rob Tibshirani](http://www.r-bloggers.com/in-depth-introduction-to-machine-learning-in-15-hours-of-expert-videos/).