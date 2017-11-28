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

I have built a mobile drone instructable here https://www.instructables.com/member/mrbirch/instructables/

All communication is via TCP443

Design Goals

Technology has become personal and we carry at least one device with us all the time. Very few people do not have a permanent personal device continually advertising it's MAC address. Mac addresses in general do not change. We all need to sleep for at least 4 hours a day and usually charge our personal devices during that time, we generally do not turn them off while doing that.
1. Our personal devices (ones we travel with) are usually stationary for four hours a day and during that time we are also recharging (sleeping)
2. We should be able to track measure and report on that activity on a global scale.
3. Based on the data we will have a trail of activity that states while I cannot prove that I was not in one location at a particular time, I can prove that I was in a different location at that same time. Proving my Alibi
