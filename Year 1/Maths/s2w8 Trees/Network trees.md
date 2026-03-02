Created: Oct 08 2025
Class: [[Trees]] 
- - -
# Standard internet protocol routing
clients talk to servers
routers select paths for packets to travel from origin to destination
each router has routing table which stores the paths the packets should take

# Peer to peer
All peers are equal. Every computer plays role of client and server
P2P network is an overlay network above IP infrastructure
Each peer stores list of neighbours
Messages sent hop-by-hop from one peer to the next

## Kademlia Trees
![[Pasted image 20251008105556.png]]
Used to path find to message destination
Creates log size routing table. Size = $log(n)$
Every peer is reachable in path length $log(n)$

Represents connections as tree
Peers represented as binary
Neighbours are determined by peers with binaries that only differ by 1 bit

### Bit flipping algorithm
Send packet to neighbour with shortest path length to target
Kinda like a word ladder
Repeat for new node until target node is reached

in other words
Take origin binary,
flip 1st bit from the right that is different from target
Since flipping 1 bit at a time, each subsequent peer is guaranteed to be a neighbour of the previous one
Repeat until you have reached target
$$For \space 110 \rightarrow 001$$
$$110 \rightarrow 010\rightarrow 000 \rightarrow 001$$