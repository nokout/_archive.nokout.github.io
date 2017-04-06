---
layout: post
title: Blockchain
categories: null
---

## Introduction

The following is a modified version of a brief I wrote for Dept Of Human Services (Commonwealth of Australia) about blockchain. I am sharing this to provide descriptions of what I think are the key concepts. I am by no means an expert on the subject but it should provide a reasonable basis understanding blockchain and its utility.

### Contents:
 - [Whats in a blockchain?](#whats-in-a-blockchain)
 - [Whats it for?](#whats-it-for)
 - [When is a thing Blockchain](#when-is-a-thing-blockchain)
 - [Performance](#performance)
 - [Using it](#using-it)
 - [Failures and Risks](#failures-and-risks)
 - [The likely future](#the-likely-future)
 - [Key Blockchain Technical Components](#key-blockchain-technical-components)
 - [Distributed Ledger](#distributed-ledger)
 - [Transaction Signing](#transaction-signing)
 - [Transaction Ordering](#transaction-ordering)
 - [Transaction Schemas and Smart Contracts](#transaction-schemas-and-smart-contracts)
 - [Transaction Confirmation](#transaction-confirmation)
 - [References and Sources](#references-and-sources)


## Whats in a blockchain?

The term blockchain comes from the following elements:

- Block - Things that happens are recorded in "Blocks" of transactions (or operations)
- Chain - The blocks are recorded in chronological order as a "chain" of events

At an implementation level blockchain reuses many existing advanced computer science concepts and adds to this the "big-deal" innovation which is an implementation for "distributed consensus". This is the key component which makes blockchain truly innovative.

## Whats it for?

There are several analogies that are useful to describe blockchain but the most prevalent is the general ledger concept from accounting practices. This is apt because at its core, blockchain is about managing the "transaction" of "assets" between "accounts" (however what a transaction, asset and account are in this context is more flexible than the well-known norms). Given this, it is not a surprise that the elements of blockchain were first laid out in the implementation of the virtual currency [Bitcoin](https://bitcoin.org/bitcoin.pdf).

A software based general ledger is nothing new though, it was one of the early areas addressed by computers. The excitement around blockchain is that it enables the additional feature of the general ledger being shared and distributed. This means that there is no central controlling entity so "[It provides a way to verify the order in which entries are made to a ledger, without any centralized authority](https://www.constellationr.com/blog-news/blockchain-almost-everything-you-read-wrong)".

This means business processes which traditionally required a trusted third party such as stock markets, clearing houses or contract settlements can now be potentially reengineered without that trusted third party.

## When is a thing Blockchain

Even though there is no globally accepted definition for blockchain, the following characterisations are fairly consistent across various authoritative discussions regarding blockchain.

If a technical approach does not meet these characteristics it is debatable if it meets current norms for the definition of blockchain.


**Shared and Fully Distributed >>**
Blockchain supports shared and distributed applications because the blockchain is dispersed over the network of interconnected computers of all participants with no central control or authority.

**Egalitarian >>**
The egalitarian aspect of blockchain makes it so that entities participating the in the blockchain are treated equally at a technical level. This is probably the least critical characteristic and is weakened in some applications of blockchain, but it is present in some fashion for all the implementations researched.

**Append Only >>**
The way blockchain is implemented means that it is strictly append-only. The only way information can be contributed to a blockchain is by adding it to the end.

**Provides Consensus >>**
Providing consensus is a key role of the blockchain. This ensures that all participants in the blockchain are in agreement about the state of it. The mechanism to reach consensus varies.

**Immutable & Final >>**
Once the participants in a blockchain network reach consensus about the blockchain state, there is no mechanism to retrospectively alter it.

**Provides Provenance >>**
The combination of the above also means that a blockchain implementation provides provenance for all transactions on the chain.


#### _...However_
As with many popular and developing technical concepts it is difficult to maintain hard boundaries around its definition as constant related creations, modifications, extensions and adaptations continue. It is also important to note that the blockchain term is starting to gain value as a marketing term and this may contribute to increased ambiguity in the definition.

## Performance
It is also important to consider the performance constraints of blockchain based solution. It is highly likely that where some of th blockchain characteristics are not required (e.g. if a truly distribute solution is not needed), more performant solutions will be availabl through existing technologies.

The reasons for this are discussed further in the Technical sections of this document.

## Using it
When considering blockchain the principle ["not everything possible is also is practical, and possibly not even desirable"](https://www2.deloitte.com/content/dam/Deloitte/au/Images/infographics/au-deloitte-technology-bitcoin-blockchain-distributed-ledgers-180416.pdf) is very appropriate and reminds us that it is important to consider the characteristics of blockchain in order to assess use cases.

A clear candidate for a blockchain solution will:
 - have an inherent and powerful need for fully distributed  processing,
 - want to treat all actors in the system the same,
 - have strong support from the user group,
 - probably want to understand provenance,
 - be tolerant of all prior decisions and transactions being  exposed to and permanent for all participants, and
 - does not require fast response times or high throughput.

Use cases outside of the above may still be worth consideration but more scrutiny should be applied.

Some interesting and informative example use cases:
- [Bitcoin - an innovative payment network and a new kind of money](https://bitcoin.org/en/)
- [Tracking Diamonds as an asset on the blockchain to detect blood diamonds](https://www.ft.com/content/f2b0b2ee-9012-11e4-a0e5-00144feabdc0)
- [Settling intra-bank payments](http://www.coindesk.com/australia-commonwealth-bank-ripple-experiment/)
- [Voting in politics](https://www.cryptocoinsnews.com/blockchain-voting-used-by-danish-political-party/)
- [Digital identity and e-residency](https://e-estonia.com/e-residents/about/)
- [Finance Notary](http://ausdigital.org/specs/ausdigital-nry/1.0/)

## Failures and Risks

While it does not appear that any systemic technical failures have been identified in the blockchain approach, its application does not remove all existing risks and also adds some new risks. Here are some examples of major failures using blockchain technology:

 - The Ethereum "The DAO hack" exploited how some transactions were coded in one application on the Ethereum blockchain platform. While some currency was brought back under control, the final outcome is still unclear and about USD \$5M is at risk. There is an interesting account of the saga [here](http://www.coindesk.com/ethereum-dao-hacker-getting-away-classic/).
 - There has also been major losses of bitcoin simply because the owner lost their key information which is required to participate in the blockchain. In a [single example](https://news.bitcoin.com/guy-lost-bitcoin-computer-upgrade/) USD $67K was lost.
 - The major Bitcoin exchange Mt Gox went backrupt and \$460 million [dollars disappeared](https://www.wired.com/2014/03/bitcoin-exchange/)

So while blockchain provides the mechanisms to be highly secure and distributed, other factors – including human - are still involved and can be exploited. The other very important point is to consider what happens if things go wrong because blockchain is strongly resistant to an appeal to authority for rectification.

Applications of Blockchain are also still very immature and there is little standardisation or support from existing software packages. This is particularly pertinent risk when attempting to integrate blockchain solutions into existing systems.

There is also a risk with regard to how much a process can be disrupted with blockchain while not falling foul of regulatory requirements which are commonly based on the existence of an authoritative entity. This is especially the case for financial and law applications which are otherwise highly suited to the blockchain approach.

## The likely future
The future for blockchain is not easily assessed. There is a spectrum of projects underway across the world which range from highly speculative but massively disruptive, to applications which are more specific and conformist to current norms.

Examples of the highly disruptive end of the spectrum are [Ethereum](https://ethereum.org/) and [IPFS](https://ipfs.io/) which aim to fundamentally change the way the web works.

In the more speculative arenas there is a high level of inertia working against those changes which is likely to mean that they will not immediately displace existing solutions. It is also likely that elements of these disruptive applications will be co-opted by established players while largely maintaining the status quo.

# Key Blockchain Technical Components
The following sections look closer at some of the key technical components of blockchain as they are currently understood. While not essential to understand appropriate usage of blockchain they do connect some of the more technical terminology used with the key concepts for assessing blockchain usage.

## Distributed Ledger
Mechanisms for maintaining distributed databases vary widely and can involve partitioning data into subsets which are managed separately, replication which maintains multiple copies in different places, and many other complex considerations.

The blockchain requirement for equal collaboration of each node in order to achieve transaction ordering (discussed in a following section) means many of these approaches are not possible. So in blockchain a copy of the ledger is "potentially" on all nodes and is able to be automatically created on all nodes.

Maintaining all these copies is hard and complex, this is made somewhat easier with the append-only nature of blockchain which is inherent in the provenance and immutable characteristics of blockchain.

While the approach to distribution by blockchain is fairly straightforward, it is not very performant. The cost of maintaining the storage of the blockchain by all participants is high and is a contributor to the comparably low performance of blockchain.

## Transaction Signing
All transactions are signed using existing [public key encryption](https://en.wikipedia.org/wiki/Public-key_cryptography) processes. This signature is appended to all transactions and guarantees which user created the transaction and that it has not been modified after creation. Other blockchain users can verify these aspects. This component uses the same public key encryption processes which are used to secure (https) webpage traffic but does not require central issuing authorities.

This guarantees that each transaction was produced by who it is purported to be and that it has not been modified by some other actor.

## Transaction Ordering
The hard problem solved by bitcoin (the original blockchain implementation) is the double spending problem. This problem occurs when a system fails to prevent a user from "spending" - or more generally, transacting – on the same entity multiple times. The common analogy is that if a person writes two cheques for the same amount, but only has sufficient funds for one of these cheques to be paid; the first to be processed by a bank will be paid, and the second will be rejected.

In this analogy the banks decide which cheque will be paid, but because transactions on the blockchain have no intermediating third party like the bank, another solution is needed.

The ordering of transactions, within each confirmed block determines the outcome of any attempt to double spend. Guaranteeing that this ordering hasn't been manipulated is achieved through a consensus algorithm. The job of the consensus algorithm is to provide a mathematically provable mechanism to agree on the ordering of transactions.

In Bitcoin and many other algorithms - including Ethereum - the basis of this is a race to provide a "proof of work". A proof of work is a mathematical problem which is hard to solve but easy to confirm. This is used to "balance" the network and keep the probability of a bad actor being able to influence the network practically impossible. Refer to _Appendix A - Bitcoin Proof Of Work To Build Consensus_ for more information on bitcoins technical application of this.

In HyperLedger and ripple this is achieved through variations on the Practical Byzantine Fault Tolerance (PBFT) algorithm which requires that a quorum of nodes provide identical answers to an algorithm. This contrasts with the bitcoin approach because instead of the confirmation being a race between the nodes, each node contributes their answer which is accepted once a quorum is reached.

There are various pros and cons for each approach but it can be said that - thus far - the process of maintaining a distributed mathematically provable consensus has a substantial computational cost.

Development is also happening around "proof of stake" alternatives to proofs of work and PBFT but no evidence of an accepted solution supporting this approach could be identified at the time of writing. In this approach the principle is that each user would have a weighted stake instead of the flat distribution of stake in other mechanisms.

## Transaction Schemas and Smart Contracts
Within a blockchain application all the participating nodes must agree on the rules in advance by establishing the schema of supported transactions. In some applications this is a global set of rules, while in other applications (designed to support general applications on blockchains) it might vary across the network but is always agreed by the network participants.

This is where the concept of smart contracts can be applied. Smart contracts allow a user in the blockchain network to author a script which specifies the rules for all the transactions which are covered by that smart contract.

In allowing users to define these rules it also allows the creation of distinctions between user groups, somewhat reducing the egalitarian characteristic of the application. However this is up to each implementation and is not provided by the blockchain technology itself.

## Transaction Confirmation
Blockchain implementations also provide an ability to confirm transactions without having to have a copy of the entire blockchain content. The nodes which only implement this aspect, can only confirm a transaction has been accepted and confirmed into the blockchain. This document refers to these as "light nodes" but are actuality referred to by different names in different applications.

While a light node does not have all the transaction information it still maintains the headers of the blockchain. These headers contains a field called the "[merkle root](https://hsi.dhsstaff.dhs.gov.au/Pages/default.aspx)", the merkle root represents the final outcome of building a "[merkle tree](https://en.wikipedia.org/wiki/Merkle_tree)".

The merkle root allows a full node to provide sufficient information to a light node for it to prove that a transaction has been accepted and confirmed by the network.

The merkle tree is a structure built from the set of transactions in a block. It is built through repeatedly combining the results of hashing each transaction until the entire set of transactions is represented by a single hash which can only be generated by that exact set of ordered transactions. The nature of this structure drastically reduces the amount of information that has to be passed from the full node to the light node to perform transaction validation.

The merkle tree is used by a light node by processing:
 - the _transaction_ which it is trying to confirm,
 - the _block header_ containing the merkle root which is available from the blockchain network,
 - The _missing parts_ of the merkle tree which is provided by a _trusted_ full node.

This processing compares the result of recalculating the merkle tree using the _transaction_ of interest and the _missing parts_ and confirming that the results match the known _block header_. If they match then it is proven that this transaction was confirmed in the related block.

It is important to note that this partially relies on a _trusted_ full node whereas in all other blockchain processes nodes are assumed to be untrustworthy.

While this technical concept is not intrinsic to the operation of most blockchain networks it enables the light nodes feature which is highly suited to low power nodes and "wallet" applications. This concept has also been adapted in powerful ways for some of highly disruptive applications like IPFS.

# The Bitcoin Proof Of Work To Build Consensus

The bitcoin proof of work is a task undertaken to cryptographically hash the contents of a block, plus the hash of the previous block, plus an unspecified number. When the output of that function meets a certain criteria it is taken to be solved (e.g. The first 4 characters must be zero). A solution to the proof of work is included in the rules for the bitcoin network treating a block as valid.

Because hash results vary massively with very small inputs to the point of appearing to be random, solving this is computationally expensive.

The following table shows an example of this where the block of transactions is represented by a single string. You can see that changing only the "unspecified number" drastically changes the resulting hash in an unpredictable way. A proof of work is considered solved when this process is continued until the hash value meets the blockchain proof of work rules - like having to start with a certain number of zeros as in bitcoin.

| String | Hash  |
|--------|-------|
| [“This is an example block of transactions”, 0] | aeb46ab65625c3c1e577bf6f2733f082712c332b3406e4b06b84326fd7bb7d6e
| [“This is an example block of transactions”, 1] | 69cf7aa89e06b10de9b5a6255b775fb0ccadf4e4053452daa2f42c763e3b2b28
| [“This is an example block of transactions”, 2] | 56548b81bc9e08ae6309f451ff23c25337426fc51e85013fc34579c7638f9b71
| [“This is an example block of transactions”, 3] | cb5358f99a461b299b6ff499f170dab6614ec68ebcc89adde91f8c49e05ee9fe


While solving the proof of work problem is computationally expensive checking the solution is cheap.

The network determines block validity as a group when proposed transactions are published to the ledger. Members of the network attempt to validate a set of transactions into a proposed block. The member who completes this task first is rewarded with a bitcoin payment. This reward ensures that sufficient nodes are incentivised to try and be the one to confirm a block – keeping the network running.

However, in order to prevent malicious nodes from publishing invalid blocks to claim the payment or manipulate the blockchain in their favour, the proof of work must also be completed. This way, each node is competing against all the other nodes in a race to be the one who confirms a block and the cost to swing the odds in favour of being the one to confirm a block (and therefore get the chance to corrupt the blockchain) is massively cost ineffective, therefore protecting the blockchain.

While this solves the double spend problem without an intermediary it happens at massive computational cost and without any tangible outcome for the processing effort.

**Note:** Ethereum also uses a proof of work but uses a different algorithm to SHA256 called ETHASH. While the algorithm is different the function is the same. <https://github.com/ethereum/wiki/wiki/Ethash>

## References and Sources

The following sources were considered in developing this information.

Supporting Information:
 - <https://www2.deloitte.com/content/dam/Deloitte/au/Images/infographics/au-deloitte-technology-bitcoin-blockchain-distributed-ledgers-180416.pdf>
 - Blockchain will prove to be a risky route for payment services - Gartner (ID: G00310735)
 - Experiment with blockchains for data management innovation - Gartner (ID: G00314377)
 - <http://cryptorials.io/glossary/lightweight-wallet/>
 - <http://www.coindesk.com/australia-commonwealth-bank-ripple-experiment/>
 - <http://www.thegeniusworks.com/2016/02/blockchain-from-geeky-bitcoin-technology-to-a-revolution-in-everyday-processes/>
 - <http://www.waterstechnology.com/inside-reference-data/opinion/2455662/golden-copy-the-blockchain-is-just-a-database>
 - <https://bitcoin.org/bitcoin.pdf>
 - <https://bitcoin.org/en/>
 - <https://bitcoin.org/en/glossary/merkle-root>
 - <https://console.ng.bluemix.net/docs/services/blockchain/etn_pbft.html>
 - <https://e-estonia.com/e-residents/about/>
 - <https://en.wikipedia.org/wiki/Merkle_tree>
 - <https://en.wikipedia.org/wiki/Public-key_cryptography>
 - <https://ethereum.org/>
 - <https://gendal.me/2014/10/26/a-simple-explanation-of-bitcoin-sidechains/>
 - <https://ipfs.io/>
 - <https://medium.com/@keilian/in-blockchain-we-trust-452c1ac5b37a#.gaj8e81r0>
 - <https://news.bitcoin.com/guy-lost-bitcoin-computer-upgrade/>
 - <https://www.constellationr.com/blog-news/blockchain-almost-everything-you-read-wrong>
 - <https://www.constellationr.com/blog-news/blockchain-almost-everything-you-read-wrong>
 - <https://www.cryptocoinsnews.com/blockchain-voting-used-by-danish-political-party/>
 - <https://www.ft.com/content/f2b0b2ee-9012-11e4-a0e5-00144feabdc0>
 - <https://www.wired.com/2014/03/bitcoin-exchange/>
 - <https://www2.deloitte.com/content/dam/Deloitte/au/Images/infographics/au-deloitte-technology-bitcoin-blockchain-distributed-ledgers-180416.pdf>
 - Tookit – Overview of blockchain use cases – Gartner (ID: G00302283)
 - [Ausdigital Contract Notorisation](http://ausdigital.org/specs/ausdigital-nry/1.0/)
