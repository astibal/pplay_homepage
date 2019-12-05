Title: Welcome to pplay homepage!
Date: 2019-12-04 17:30
Category: intro
save_as: index.html

# TL;DR  

**still on python2 -- python3 version is on the way**

* `sudo pip install pplay`
* slightly outdated .deb -- [download section](https://bitbucket.org/astibal/pplay/downloads/) 



# Introduction

some time ago I've been in the need of reproducing some issue with DLP, while I was provided with pcap when DLP was not involved in the traffic flow and everything worked.
I was trying to utilize netcat, tcpreplay and other tools. All were very good possibly for their usage, but this was not what I wanted to have.  

> "I wanted a tool to simply replay the payload of the connection"

I quickly realized there is surprisingly and literally **nothing** I can use as I wanted.

# What **IS** pplay

PPlay is tool to replay/resend application data (ie content of TCP or UDP stream) from suplied single connection from pcap, or smcap.  
Its primary role is to resend already seen (and captured) data over the wire, but doesn't care if segments are smaller, or IP addresses are different.

# What pplay **IS NOT**

PPlay is *not* stress test tool. It can be run simultaneously, sure. But its performance is not aimed to be super tuned, there are waiting times at certain
places in the code.

PPlay is *not* capture analyzer. It can however save your capture in python module, you can then acess captured L7 data from python class.

# Support #
For comments, feedback or new feature discussion feel free to drop a message to **pplay-users@googlegroups.com** mailing list.  

