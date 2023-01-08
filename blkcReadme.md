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



