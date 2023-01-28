The gossip package implements a reliable probabilistic eager broadcast protocol that enables 
the exchange of asynchronous messages within a distributed system without the need for
a centralized message broker.

The protocol uses UDP to reduce the network overhead. However, this imposes a limitation
on message size, which must be small enough to fit within a single UDP datagram, usually 
no larger than 1500 bytes (typical network MTU size).