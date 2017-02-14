---
layout: post
title: "Operating System Fingerprinting and Nmap"
description: "The various techniques and methods in and around OS fingerprinting"
comments: true
keywords: "fingerprint, fingerprinting, os fingerprinting"
---

> Currently a work in progress.

# What is fingerprinting?


# Operating System (OS) fingerprinting

Via conducting an ``nmap`` scan using the ``-O`` parameter, one can conduct OS fingerprinting through inspecting the packets received from the target.  More details about [nmap here](https://www.nmap.org).

Such differentiations can be different implementations of the TCP/IP stack (TTL value defaults) and TCP window size.

Example command:

```
nmap -Pn -O IP_ADDRESS
```

The ``-Pn`` has been added since I know that the target is up but it may be blocking the ping probe.

An example output is below of conducting an OS fingerprint exercise:

```
$ nmap -Pn -O IP_ADDRESS_HERE

Starting Nmap 7.25BETA2 ( https://nmap.org ) at 2017-02-10 17:03 EST
Nmap scan report for MYSITE.COM (IP_ADDRESS_HERE)
Host is up (0.0020s latency).

All 1000 scanned ports on MYSITE.COM (IP_ADDRESS_HERE) are filtered

Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port

Device type: WAP|general purpose|specialized

Running: DETAILS_HERE
OS CPE: OS_CPE_DETAILS_HERE

OS details: OS_DETAILS_HERE

OS detection performed. Please report any incorrect results at https://nmap.org/submit/ .

Nmap done: 1 IP address (1 host up) scanned in 253.29 seconds

```

Also note that by default, nmap scans 1000 ports which is mentioned in the report above.  


> Your mileage may vary.  This content is constantly under development and may change at any time.
