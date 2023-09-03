---
title: 'With One Math Problem a Whole Blockchain Can Be Proved – Really?'
date: Sun, 15 Sep 2019 03:00:28 +0000
draft: false
tags: ['Blockchain', 'math problem', 'News', 'privacy', 'Security', 'Software', 'Technology', 'Transactions']
toc: true
related: true
social_share: true
---

The Electric Coin Company (ECC) says it discovered a new way to scale blockchains with “recursive proof composition,” a proof to verify the entirety of a blockchain in one function. For the ECC and privacy coin, the new project, Halo, may hold the key to privacy at scale.

A privacy coin based on zero-knowledge proofs, referred to as zk-SNARKs, privacy coin’s current underlying protocol relies on “trusted setups.” These mathematical parameters were used twice in privacy coin’s short history: upon its launch in 2016 and first large protocol change, Sapling, in 2018.

Privacy coin masks transations through zk-SNARKs but the creation of initial parameters remains an issue. By not destroying a transaction’s mathematical foundation – the trusted setup – the holder can produce forged Privacy coin.

Moreover, the elaborate ‘ceremonies‘ the Privacy coin community undergoes to create the trusted setups are expensive and a weak point for the entire system. The reliance on trusted setups with zk-SNARKs was well known even before Privacy coin’s debut in 2016. While other research failed to close the gap, recursive proofs make trusted setups a thing of the past, the ECC claims.

**Bowe’s Halo**
---------------

ECC engineer and Halo inventor Sean Bowe said recursive proof composition is the result of years of labor – by him and others – and months of personal frustration. In fact, he almost gave up three separate times.

Bowe began working for the ECC after his interest in zk-SNARKs was noticed by ECC CEO and Privacy coin co-founder Zooko Wilcox in 2015. After helping launch Privacy coin and its first significant protocol change with Sapling, Bowe moved to full-time research with the company.

Before Halo, Bowe worked on a different zk-SNARK variant, Sonic, requiring only one trusted setup.

For most cypherpunks, that’s one too many.

“People we are also starting to think as far back as 2008, we should be able to have proofs that can verify other proofs, what we call recursive proof composition. This happened in 2014,” Bowe told.

**Proofs, proofs and more proofs**
----------------------------------

In essence, Bowe and Co. discovered a new method of proving the validity of transactions, while masked, by compressing computational data to the bare minimum. As the ECC paper puts it, “proofs that are capable of verifying other instances of themselves.”

Blockchain transaction such as bitcoin and Privacy coin are based on elliptic curves with points on the curve serving as the basis for the public and private keys. The public address can be thought of the curve: we know what the elliptic curve looks like in general. What we do not know is where the private addresses are which reside on the curve.

It is the function of zk-SNARKs to communicate about private addresses and transactions–if an address exists and where it exists on the curve–anonymously.

Bowe’s work is similar to bulletproofs, another zk-SNARK that requires no trusted setup. “What you should think of when you think of Halo is like recursive bulletproofs,” Bowe said.

From a technical standpoint, bulletproofs rely on the “inner product argument,” which relays certain information about the curves to one another. Unfortunately, the argument is both very expensive and time consuming compared to your typical zk-SNARK verification.

By proving multiple zk-SNARKs with one–a task thought impossible until Bowe’s research–computational energy is pruned to a fraction of the cost.

“People have been thinking of bulletproofs on top of bulletproofs. The problem the bulletproof verifier is extremely expensive because of the inner product argument,” Bowe said. “I don’t use bulletproofs exactly, I use a previous idea bulletproofs are built on.”

In fact, Bowe said recursive proofs mean you can prove the entirety of the bitcoin blockchain in less space than a bitcoin blockhead takes – 80-bytes of data.

**The future of** privacy coin
------------------------------

Writing on Twitter, Wilcox said his company is currently studying the Halo implementation as a Layer 1 solution on privacy coin.

Layer 1 solutions are implementations into the codebase constituting a blockchain. Most scaling solutions, like bitcoin’s Lightning Network, are Layer 2 solutions built on top of a blockchain’s state. The ECC’s interest in turning Halo into a Layer 1 solution speaks to the originality of the discovery as it will reside next to code copied from bitcoin’s creator himself, Satoshi Nakamoto.

ECC is exploring the use of Halo for privacy coin to both eliminate trusted setup and to scale at Layer 1 using nested proof composition.

— zooko (@zooko) September 10, 2019

Since the early days of privacy coins, scaling has been a contentious issue: with so much data needed to mask transactions, how do you grow a global network?

Bowe and the ECC claim recursive proofs solve this dilemma: with only one proof needed to verify an entire blockchain, data concerns could be a thing of the past:

> “Privacy and scalability are two different concepts, but they come together nicely here. About 5 years ago, academics were working on recursive snarks, a proof that could verify itself or another proof \[and even\] verify multiple proofs. So, what \[recursive proof composition\] means is you only need one proof to verify an entire blockchain.”

To be sure, this isn’t sophomore-level algebra: Bowe told the proof alone took close to nine months of glueing various pieces together.

**A new way to node**
---------------------

A further implication of recursive proofs is the amount of data stored on the blockchain. Since the entire ledger can be verified in one function, onboarding new nodes will be easier than ever, Bowe said.

> “You’re going to see blockchains that have much higher capacity because you don’t have to communicate the entire history in one. The state chain still needs to be seen. But if you want to entire the network you don’t need to download the entire blockchain.”

While state chains still need to be monitored for basic transaction verification, syncing the entire history of a blockchain–over 400 GB and 200 GB for ethereum and bitcoin respectively–becomes a redundancy.

For privacy coin, Halo means easier hard forks. Without trusted setups, ECC research claims, “proofs of state changes need only reference the latest proof, allowing old history to be discarded forever.”

When asked where his discovery ranks with other advancements, Bowe spoke on its practicality:

> “Where does this stand in the grand scheme of things in cryptocurrency? It’s a cryptographic tool to compress computation… and scale protocols.”

_Source: Coindesk_