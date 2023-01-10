Distributed consensus - in bitcoin
>at any given point;
- all nodes have a sequence of blocks of txns they have reached consensus on
- each node has a set of outstanding txns its heard about

>its hard to achieve
- latency (no standard global time)
- malicious activity
- genuine node crash
>Byzantine generals problem
>Fischer-Lynch-Paterson(deterministic nodes): consensus impossible with a single faulty code
>Paxos

Results says more about the model than about the problem
The models were developed to study systems like distributed databases
..
>> Reach consensus without identity
- in each round, random node is picked, and this node proposes the next block in chain
- other nodes implicitly accept/reject this block
-- by either extending it.
-- or ignoring it and extending chain from earlier block

Every block contains hash of the block it extends
image.png
Double spend probability: this decreases exponentially with # of confirmations
Most common heruuistic: 6 confirmations;

Incentives & Proof of work:
block reward: 

Double Spending attack:

Types of Consensus Protocols:
Proof-of-work:
Proof-of-Staking: forgers stake their tokens and has probability to be block validator
Delegated Proof-of-stake: Instead of probability cryptocurrency holders are able to cast votes apportioned 
Proof-of-Authority: Arguably more centralized again, PoA has predetermined block validators. New blocks on a blockchain are only created when the validators are in majority. The protocol is similar to PoS. The validators are publicly known and accountable for determining their role and eligibility for PoS validation. A newer blockchain, Elysian, uses PoA as well as some Ethereum testnets, or test blockchains.
Types of Blockchain  attacks:
`Sybil attack:   Proof-of-work has protected froom this attack
Routing attack: In a routing attack, a hacker intercepts data as its sent to an ISP. Once they're in, a hacker can split the network into partitions.`

