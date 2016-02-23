# About The Project of Firewall on SDN
Hello, I'm Rizky.  This project is written by me as part of my assignment in CS4055 - High Performance Data Networking. 
I implement Firewall on SDN.  I write some controller applications that work as Firewall and analyze incoming packets for each host. This project is also able to implement connection tracking mechanism. For this project I use mininet together with the  Ryu controller and OpenFlow framework to implement and to simulate firewall on SDN.  The applications are tested on local machine with Firewall rule-set. I use Wireshark to monitor data communication in the hosts

#Introduction
MININET 

Mininet is a network emulator which creates a network of virtual hosts, switches, controllers, and links. Mininet hosts run standard Linux network software, and its switches support OpenFlow for highly flexible custom routing and Software-Defined Networking. 

OPENFLOW 

OpenFlow Protocol(OFP) is the first, industry-specified, standardized SDN protocol which defines a way for the controller to communicate with switches.  The purpose behind it is to provide standardized speciffication for communication interfaces of Control and Infrastructure Layer devices.  It allows manipulation of the data stored on forwarding devices to refine policy-based decision for packet forwarding.

RYU 

Ryu  is a component-based SDN framework which delivers a suitable platform for SDN applications to run on the top of Ryu controller. It is an open source tool written in Python that provides well-defined APIs & packet libraries and supports all versions of OpenFlow. 
FIREWALL ON SDN CONTROLLER 
A Firewall is a network security system that is used to control the flow of ingress and egress traffic usually between a more secure local-area network (LAN) and a less secure wide-area network (WAN). The system analyses data packets for parameters like L2/L3 headers (i.e., MAC and IP address) or performs deep packet inspection (DPI) for higher layer parameters (like application type and services etc) to filter network traffic. A firewall acts as a barricade between a trusted, secure internal network and another network (e.g. the Internet) which is supposed to be not very secure or trusted 

#Installation
Virtual Box
Install	the	open-source	VirtualBox	hypervisor	https://www.virtualbox.org/wiki/Downloads

Mininet VM Image
http://www.nas.ewi.tudelft.nl/tmp/Mininet-VM.ova

Ryu	has	already	been	installed	in	the	directory	`ryu`	in	the	home	folder	of	your	VM.	You	are	encouraged	to	consult	the	additional	documentation	about	Ryu	at	http://ryu.readthedocs.org/	

#Topology
![alt tag](https://cloud.githubusercontent.com/assets/17114181/13259851/7834fe16-da59-11e5-891b-94b53b5b9d26.JPG)

This topology consists of 6 host, 3 switches, and 1 controller. h1s1 and h2s1 connect to switch1 (s1), h1s2 and h2s2 connect to switch2 (s2), and h1s3 and h2s3 connect to switch3 (s3). I create the network segmentation into 2 parts (VLAN ID=3 and VLAN ID=2). Ryu application can be run via command-line tool called ryu-manager, I use OFP version 1.3 for each switch (s1,s2,and s3).

#Refferences
Mininet website.Available: http://mininet.org/overview/ 

Ryu website http://osrg.github.io/ryu/certification.html

VM Image http://www.nas.ewi.tudelft.nl/tmp/Mininet-VM.ova 
