### QoS (Quality of service) ###

This is a Linux bash script that will set up tc to limit the outgoing bandwidth for connections to the Dogecoin2 network. It limits outbound TCP traffic with a source or destination port of 22656, but not if the destination IP is within a LAN.

This means one can have an always-on dogecoin2d instance running, and another local dogecoin2d/dogecoin2-qt instance which connects to this node and receives blocks from it.
