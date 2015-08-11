---
title: Understanding Complexity
layout: blog
excerpt: |
  What makes a system complex? How can we study complexity in order 
  to be more effective in any common project?
---


# Understanding Complexity


## Introduction

I think we all have an intuitive notion of complexity. We encounter it in the things we learn, the projects we work on alone or in teams, and even in our physical surroundings. I've found that simplicity and organisation can be the defining factor for progress. Complexity can be a laborious swamp that inhibits great things happening.

Complexity is ubiquitous in the truest sense. Hence understanding at least part of the dynamics at play seems very worthwhile to me. At the very least the impact on one's own effectiveness could be great; on the other hand, it could transform large organisations and the world we live in.

Perhaps we'll only scratch the surface here, but I do hope to develop an understanding of complexity that yields tangible results, even if only on an individual level (but hopefully much more). This post was inspired by my experience at work, as well as the problems I've faced when working on my own side-projects.


This can sometimes be 
subjective: a seemingly messy desk could be organised to one person but not to another. 
This suggests something more fundamental than 

## Brainstorm

Before trying to be too technical or precise, I thought it would be helpful to just brainstorm some ideas I find related to the notion of "complexity". I've tried to group them in ways I find meaningful. You may or may not agree! Try and think of other ways of looking at complexity, and keep them in mind and you read the rest of the post. I'll try and tie the ones that I've idenitified in.


![brainstorm]({{ site.url }}/images/complexity/brainstorm.svg)



## Making it More Precise

### Number of parts

It seems intuitive to model systems generally as a set of parts interacting. This can be 
viewed as a graph with vertices/nodes and edges. I think the intuitiveness of graphs makes them dangerous: one shouldn't take them for granted (as with anything)! We have to make a decision on granularity. On one extreme, we could of course just call the entire system one single node. On the other hand, in a team project where nodes are members, we could split up a member into phases of the day, on into the person's sub-projects.

So what's a reasonable way to determine the granularity to use on a graph for analysing complexity?

![granularity]({{ site.url }}/images/complexity/granularity.svg)


