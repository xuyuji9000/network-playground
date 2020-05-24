Why sliding window protocol?

The time it takes for ACK signal to be received may represent a significant amount of time compared to the time needed to send the packet. In this case the overall throughput may be much lower than theoretically possible.
To address this, sliding window protocol allow a selected number of packets, the window, to be sent without havint to wait for an ACK. Each packet receive a sequence number, and the ACKs send back the number. The protocol keeps track of which packets have been ACKed, and when they are received, sends more packets. In this way, the window slides along the stream of packets making up the transfer.

