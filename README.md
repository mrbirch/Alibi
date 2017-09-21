# Alibi Project
* The Alibi Project is for research purposes only and should be viewed as a theoretical design.
The author does not condone or promote any non legal activity

Design Overview

The projects aim is to track Mac addresses via geo location with timestamps.

It achieves this via widespread deployment of Kismet Drone nodes.

Data (time/loc/addr)is fed back into a central MongoDB repository where Alibi_Route is tracked on OpenMap.

Addresses that have repeated same geolocations at 3am local time will be assigned an Alibi_Home attribute.

To opt out (have your mac address removed from the dataset) you will need to run a Kismet Slave on you node.

To retrieve data from the datasets you must run a Kismet Drone on your node.

Currently there are Drone packages for Android and Debian.

All communication is via TCP443

Design Goals
