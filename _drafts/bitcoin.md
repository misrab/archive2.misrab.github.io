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

1. Authenticity of transactions and balances
2. Privacy: the ledger is public
3. Sequentiality in time: which transaction came first?

Let's explore these techniques.

### Transaction Authenticity

Earlier, we mentionned that Alice could pay Bob 5 BTC by announing it on the network, thereby signalling all nodes to update the ledger. To prevent anyone from pretending to be Alice, this is done cryptographically.

The announcement is the "message". Alice posseses a personal, secret "private key", which she uses alongside the message to create a "signature". In other words, $ signature = f(private key, message) $.

But how do other nodes use this to determine authenticity? It turns out that Alice can also have a "public key" (which of course everybody knows). Nodes can verify the broadcast message through a seperate function $ v(signature, message, public key) $ that will essentially return true or false. If false, it would mean the correct private key was not used to generate the signature, and the message is thereby invalid. Note that a good consequence of this is that the message can't be maliciously or otherwise altered as it passes accross the network: that would invalidate it. The mathematics used is rooted in [elliptic curve cryptography](http://en.wikipedia.org/wiki/Elliptic_curve_cryptography).

Since everybody has a public key, we use that as recipient address as well. In other words, when Alice is sending money to Bob, she actually sends it to his public key. This is simply reuse: no cryptography is being done here.

### The Actual Ledger

Now that we're getting the hang of transactions, let's remove the oversimplification from the ledger. In reality, account balances are not stored at all. How then can we be sure Alice has sufficient funds to send Bob 5 BTC? When she seeks to spend the 5 BTC, she must reference previous transactions where she _received_ bitcoins, for a total of 5 BTC.

In other words, a transaction message is comprised of inputs and outputs. All inputs must be fully spent, so if Alice wished to send 10 BTC to Bob, using inputs amounting to 12 BTC, she would send herself 2 BTC in the outputs:

![input output]({{ site.url }}/images/bitcoin/3.png)

Hence ownership of Bitcoin is passed along in a change, where the validity of each transaction depends on previous transactions. What does this mean? It means before transacting in Bitcoin, one has to download the history of all transactions that ever took place, and sequentially verify them through signatures as discussed earlier. This is the cost of a decentralised network. It usually takes about a day, and only has to be done in aggregate once: it can then be done incrementally, which takes much, much less time.

In addition to validating each transaction through signatures, each node checks for double-spending: the same input _cannot_ be used in two separate transactions.

In summary, the ledger is a giant list of transactions. Possessing Bitcoin means having transactions where your public key is an output address, and where those outputs haven't been used as inputs for another transaction yet.

### Double Spending and Sequentiality




## Conclusion

## Acknowledgements

Two great resources I first used to understand Bitcoin were [this video](https://www.youtube.com/watch?v=Lx9zgZCMqXE) and [the original paper](https://bitcoin.org/bitcoin.pdf), and the organisation of my explanation likely deeply reflects that.