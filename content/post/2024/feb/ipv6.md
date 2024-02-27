+++
title = 'nullidle debugging'
date = 2024-02-09T07:15:54-07:00
draft = false
image = '/img/posts/ipv6.png'
description = 'What are your thoughts on IPv6?'
+++

# Introduction

It is astonishing that a protocol released in 1983 still powers a vast majority of our internet based technology. The TCP/IP protocol ha been actively used and scaled to what our modern internet is today, over 41 years later!  Until recently, almost every single connection made between any device on the internet has been trasmitted using TCP/IP version 4. IPv6 was developed in response to the predicted exhaustion of the IPv4 address space. It was reported RIPE NCC was fully depleted of IPv4 addresses on November 25th, 2019. 

# NAT

While IPv4 address space is mostly consumed, connection of additional devices has been possible thanks to network address translation. NAT allows a network of non-public devices operating on private address space to communicate with the public internet by routing traffic of local devices through the NAT device. In terms of device security, this is a huge benefit in keeping your devices safe as it provides an additional layer of isolation between the internet and local devices. If someone is trying to connect to a device residing behind a NAT device, that connection will only succeed if rules exist to direct traffic to that device. The target device would need to be either set as a DMZ or port forwarding rules would need to exist to successfully connect to that device. 

With up to 4.3 billion connected devices on the public internet on IPv4 alone, there are countless malicious actors scanning the public internet at any given time for open ports and vulnerable software. If a port is open, it is capable of accepting a connection. Depending on the software accecpting the connection, it may be vulnerable to exploit. If that vulerability is successfully explited, that malicious actor could gain access to the device. 

Without the address space limitations in IPv6, the need to operate multiple devices behind a NAT doesn't exist. A unique address can be assigned to every single device using the version six protocol. While IPv6 adoption has been slow for most devices operating in homes, mobile technology is the largest adopter of IPv6.

## What does this mean?

While the rest of the world is protected by a NAT using IPv4 address, anyone with the IPv6 address of your mobile device can make a direct connection to the device. The connection is only possible if there is something listening for connections on an open port of the device, but without a NAT a direct connection is possible. This is HUGE in terms of goverment survellence, if they wish to monitor the activities of an individual they only need to exploit the device. Without any layer of security between the device and public internet, a direct connection can be established allowing them to access your day to day phone activities. For most of us this access details our entire lives. This is why adoption of IPv6 scares the living shit out of me, without NAT, it allow a direct connection to any device with an IPv6 address. 
