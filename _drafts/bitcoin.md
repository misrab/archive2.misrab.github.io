---
title: Bitcoin - How it Works, Where it's Going
layout: blog
image: /images/bitcoin/logo.png
excerpt: |
  After going through the fundamentals of Bitcoin, I 
  explain my perspective on the cryptocurrency
---


# Bitcoin: How it Works, Where it's Going

## Introduction

The term "Bitcoin" is becoming more and more widespread. However the core technical 
details of the cryptocurrency are often brushed aside, or lumped together. Bitcoin is 
in fact a decentralised payment _system_, encompassing multiple features that characterise it. In this post, I hope to identify and briefly explain these key features.

Once we've identified the overall architecture of the system, I'll try and use it to develop some views on where things are headed.


## Fundamentals

### Overview

In its essence, Bitcoin is just a **public ledger** network. Computers come together to form a network, and each computer stores the ledger. A simplified ledger could just be a table of identities and account balances:

![simple ledger]({{ site.url }}/images/bitcoin/1.svg)

To transact, Alice and Bob can pass a message to other nodes in the network saying Alice paid Bob 5 Bitcoins (BTC). All nodes on the network then update their ledgers:

![transaction]({{ site.url }}/images/bitcoin/2.svg)

This differs from traditional transactions within or between banks in that the ledger is 
completely decentralised. This means there is no single entity that can be help accountable for what goes on with the ledger. Furthermore, the ledger is completely public.

The Bitcoin system incorporates cryptographic techniques to deal with the issues that arise from such a network, namely:

- privacy
- authenticity of transactions and balances
- sequentiality in time

Let's explore these techniques.

### Payment Authenticity


## Conclusion

## Acknowledgements

Two great resources I first used to understand Bitcoin were [this video](https://www.youtube.com/watch?v=Lx9zgZCMqXE) and [the original paper](https://bitcoin.org/bitcoin.pdf), and the organisation of my explanation likely deeply reflects that.