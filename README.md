# firewall-on-sdn
I implement Firewall on SDN.  I write some controller applications that work as Firewall and analyze incoming packets for each host. This project is also able to implement connection tracking mechanism. For this project I use mininet together with the  Ryu controller and OpenFlow framework to implement and to simulate firewall on SDN.  The applications are tested on local machine with Firewall rule-set. I use Wireshark to monitor data communication in the hosts

1.1 MININET 
Mininet is a network emulator which creates a network of virtual hosts, switches, controllers, and links. Mininet hosts run standard Linux network software, and its switches support OpenFlow for highly flexible custom routing and Software-Defined Networking. 

1.2 OPENFLOW 
OpenFlow Protocol(OFP) is the first, industry-specified, standardized SDN protocol which defines a way for the controller to communicate with switches.  The purpose behind it is to provide standardized speciffication for communication interfaces of Control and Infrastructure Layer devices.  It allows manipulation of the data stored on forwarding devices to refine policy-based decision for packet forwarding.

1.3 RYU 
Ryu  is a component-based SDN framework which delivers a suitable platform for SDN applications to run on the top of Ryu controller. It is an open source tool written in Python that provides well-defined APIs & packet libraries and supports all versions of OpenFlow. 

1.4 FIREWALL ON SDN CONTROLLER 
A Firewall is a network security system that is used to control the flow of ingress and egress traffic usually between a more secure local-area network (LAN) and a less secure wide-area network (WAN). The system analyses data packets for parameters like L2/L3 headers (i.e., MAC and IP address) or performs deep packet inspection (DPI) for higher layer parameters (like application type and services etc) to filter network traffic. A firewall acts as a barricade between a trusted, secure internal network and another network (e.g. the Internet) which is supposed to be not very secure or trusted [4] 
