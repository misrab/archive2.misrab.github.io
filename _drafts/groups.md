---
title: Abstract Groups
layout: blog
image: /images/prob1/3.png
date: 2014-11-02
excerpt: |
  Groups are a fundamental, fascinating mathematical object. 
  Everybody should be exposed to their study
---


# Abstract Groups

_Posted on November 11th, 2014_


## Introduction

Groups, and what follows from them, are really cool. Had I known earlier, I 
would have seriously started studying group theory a long time ago.

What makes abstract algebra so interesting, to me at least? I think it's the balance between generality and structure. The foundation 
is very simple (and thus general), yet it leads to extremely 
interesting ways of thinking about specific problems. If for no other reason, it's 
worth a look to enhance one's mental flexibility.

'Nuff said, let's dive in.

## On Generalisation

I want to make a quick point on the concept of generalisation. 
How does it occur and what is its use? 
My personal experience is that one first grapples with very specific problems. In this case one might be working with matrices, and seperately permutations. Generalisation occurs when one starts to notice _patterns_ accross disparate fields. For instance, "hmmm, when I multiply this matrix by others nothing changes. That's like the permutation where each element goes to itself!".

<center><em>The $3x3$ identify matrix, and the identity permutation</em></center>

$$
\begin{pmatrix} 
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1  
\end{pmatrix} 
$$

<center>
	<img style="text-align: center;" src="/images/groups/1.svg" />
</center>

What then is the advantage of connecting seemingly disparate fields? On one hand, one might be able to solve multiple problems the same way, just as we do with basic algebra: 
the solution to $ 3x + 1 = 4 $ is $ x = 1 $, whether we're talking about apples or spaceships. Another advantage, not to be understated, is getting a better mental grasp of the subject: understanding bounds on structure. By that I mean what are the minimal properties required for certain conclusions, and how far can these conclusions extend.

"Specific problems to general perspective. Simple solutions and better mental grasp". Got it!

## Groups

Let's start to be precise. A group is formally:

- A set $G$ with a binary operation $\circ\$
- The operation is associative: $ a \circ (b \circ c) = (a \circ b) \circ c$
- There is an identity element $e$
- Each element $a$ has a unique inverse $a^{-1}$ such that $ a \circ a^{-1} = e $

If the operation further commutes i.e. $a \circ b = b \circ a$ for all $a, b$, we 
say the group is Abelian. Many interesting groups will not be.

Let's look at some examples. The most typical would be the real numbers $\mathbb{R}$ under 
usual addition. When then have $e = 0$ and $a^{-1} = -a$. For common operations we'll use symbols like $+$ or $*$ instead of $\circ$, but it is _really_ important to always be aware that we are really talking about an abstract operation. This will be crucial so as not to get confused when generalising.

We already touched upon permutations of $n$ elements, also known as the **symmetric group** $S_n$. Aside from the identity permutation


## Cyclic Groups

## Subgroups

## Maps

## Morphisms

## Kernel, Image and Center

## Quotient Groups

Now is when things start to get really exciting.

## Conclusion

## Ackowledgements

A huge thanks to anyone contributing to open-source in general, 'tis the best 
way forward. In this specific case, thanks to Harvard's online 
[Abstract Algebra course](http://www.extension.harvard.edu/open-learning-initiative/abstract-algebra).