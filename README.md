# reliableBroadcast
An effort to implement a peer-to-peer solution to the Byzantine General's Problem

One of the major problems of Peer to Peer networking is the Byzantine's General Problem.  Given that certain nodes in the network could be malicious, how does one prevent them from impacting the service.

In theory, if I can make two assumptions, the problem is easily solved:

* Assumption of Reliability: Every broadcast goes to all nodes.  No one node can stop a broadcast from going to all nodes in the network.
* Assumption of Distinguishability:  Every broadcast can be identified as either trustworthy or untrustworthy based on the hash signature.

If every broadcast is reliable, then a valid message cannot be stopped.  If every trustworthy broadcast can be distinguished, then only valid instructions will be followed.

The goal of this project is implement a message protocol such that is reliable and distinguishable over a peer to peer network where any node on the internet is able to join and open to fooling the system.

