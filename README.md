# distributed-systems---fully-connected-structure


Muilti-server system
1. server are fully connected, if a server authentication successes, then it will be automatically connected to all the other server exist in the current network.

2. server can join the network at anytime, working with current clients in the system.

3. Provide acaliability and consistency:
   - guarantees that an activity message sent by a client reaches all clients that are connected to the 
     network at the time that the message was sent
     if T is the time that the message was sent, and X is the set of clients connected to the
     network at time T, then the message should be received by all clients in the set X
   - guarantees that all activity messages sent by a client are delivered in the same order at each receiving client
   - load balance 
   - if network is partitioned and the system is break into sub-groups, the sub-groups will continue work without impacting on their activities
   - after network recovered, load re-balanced, missed messages re-send, 
