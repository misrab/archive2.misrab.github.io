---
title: Quotient Groups
layout: blog
image: /images/groups/4.png
date: 2015-02-26
excerpt: |
  Armed with some terminology, we now explore some more 
  interesting concepts in group theory
---


# Quotient Groups

_Posted on February 26th, 2015_

## Introduction





Let's recap what we've been doing so far. We have these things called "groups", with 
an associative operation \circ defined between elements, identities and 
inverses. Addition on real numbers is a group. Division on integers is not, since $1/2 \notin \mathbf{Z}$.

We then looks at maps between groups written $ f: G \rightarrow G' $. **Homomorphism**, 
where $f(a) \cdot f(b) = f(a) \cdot f(b)$ seemed interesting in the way they preserve some 
sort of structure between groups. Isomorphisms present seemingly disparate groups as one.

Let's see if we can break these maps into more detail.

## Kernels, Images and Centers

The collection of elements 'reached' in $G'$ by applying $f$ to elements in $G$ is called the image of f:

![image of map]()

The elements in $G$ that get mapped to the identity in $G'$ are the kernel of $f$. I like ot think of these as items in $G$ that get 'smashed' down to $e'#:

![kernel]()

Finally, the center of a _group_ are those elements that commute with other elements in the group.

# Normal Subgroups

In our previous post we saw that a subgroup $K \subset G$ is just a subset of $G$ with group properties. What's more interesting is a **normal** subgroup, where for any $k \in K$, $g k g^{-1} \in K$ as well, for $g \in G$.

Note that what's special here is that $g$ is in $G$, not necessarily $K$. In other words, you can surround an element in $K$ by an element in $G$ and its inverse, and stay within $K$ itself - that's what's cool. This property applies to kernels of a homomorphism, which we'll see now.


# Kernel of a Homomorphism

Consider the kernel of a homomorphism $ \phi: G \rightarrow G' $. In other words, consider 
$ \ker(\phi) = \\{ g \in G : \phi(g) = e' \\} $. It turns out that kernels are subgroups of $G$, but a _homomorphic_ kernel is also a _normal_ subgroup. The proof is straighforward.

Consider $b \in ker(\phi)$ and $a \in G$. We want to show that $ker(\phi) \subset G$ is closed as a normal subgroup. In other words, that $a b a^{-1} \in ker(\phi)$...in _other_ words, that $\phi(a b a^{-1}) = e'$. We use the homomorphism property:

$$
\begin{align}
	\phi(a b a^{-1})& = \phi(a) \cdot \phi(b) \cdot \phi(a^{-1}) \\
	& = \phi(a) \cdot e' \cdot \phi(a^{-1}) \\
	& = \phi(a a^{-1}) \\
	& = \phi(e) = e'
\end{align}
$$

So indeed $a b a^{-1} \in ker(\phi)$. This is a useful point to remember: _the kernel of a homomorphism is a normal subgroup_. We'll see later that the converse is true: every normal subgroup can be seen as the kernel of some homomorphism!


## Equivalence & Cosets

// - mention superimportant. mention left, right
// - partitions and counting!
// - prime order groups

Let's recall some simple modular arithmetic. Say we are operating in _modulo_ 5. Then
$$0 = 0 \pmod 5, 1 = 1 \pmod 5...4 = 4 \pmod5, 5 = 0 \pmod 5, 6 = 1 \pmod 5...$$
We can then do additions such as $9 + 5 = 14 = 4 \pmod 5$. Notice the _cyclicality_ - that should send some sparks flying in your brain (think cyclic groups)!

This leads to the notion of **equivalence classes**, which is just a generalisation of equality. For any two elements $a, b$ (in some set), we say $a \sim b$ ("$a$ relates to $b$") if the relation $~$ has the following properties:

1. $a \sim a$ for any $a$ (reflexivity)
2. $a \sim b$ implies $b  \sim  a$ (symmetry)
3. $a \sim b$ and $b \sim c$ implies $a \sim c$ (transitivity)

These are properties we'd like for a notion of equality. In our modular example, we could say $3 \sim 8$ since $3 = 8 \pmod 5$. In this specific context, we sometimes say "$a$ is congruent to $b$ mod 5" and write $a \cong b \pmod 5$.


## Cosets & Cyclic Groups

// - nZ is cyclic. (re)show that nZ defines all cyclic groups 
// of order n.
// - show that aZ's form _all_ cosets of Z through Euclidean alg
//   i.e. so we know we're not missing any parts of Z


## Modular Arithmetic

// - relate to cosets for intuition. draw attention to + vs \circ etc..

## Quotient Groups

