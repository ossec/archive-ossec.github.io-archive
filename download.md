---
layout: page
title: Download
permalink: /download/
---

# Downloads

## Source Code Packages 

* Latest Development Snapshots
    * Server/Agent: [https://github.com/ossec/ossec-hids]()
    * Web UI: [https://github.com/ossec/ossec-wui]()
    * Documentation: [https://github.com/ossec/ossec-docs]()
* Latest Stable Release (2.8.1) 
    * [Release Notes](https://github.com/ossec/ossec-hids/releases/tag/2.8.1) 
    * Server/Agent 2.8.1 - Linux/BSD: [ossec-2.8.1.tar.gz](https://github.com/ossec/ossec-hids/archive/2.8.1.tar.gz)
        * [CheckSum](/checksum/ossec-hids-2.8.1-checksum.txt)
    * Agent 2.8 – Windows: [ossec-agent-win32-2.8.exe](https://github.com/ossec/ossec-hids/releases/download/v2.8.0/ossec-agent-win32-2.8.exe)
        * [CheckSum](/checksum/ossec-agent-win32-2.8-checksum.txt)
    * Server Virtual Appliance 2.8.1: [ossec-vm-2.8.1.ova](http://www.ossec.net/files/ossec-vm-2.8.1.ova)
        * [CheckSum](checksum/ossec-vm-2.8.1-checksum.txt)

## RPMs for RHEL, CentOS, Fedora and others

Available in the [Atomicorp](http://www.atomicorp.com/) [repository](http://www5.atomicorp.com/channels/ossec/).

* CentOS
    * el5: [i386](http://www5.atomicorp.com/channels/ossec/centos/5/i386/RPMS/)
    * el5: [x86_64](http://www5.atomicorp.com/channels/ossec/centos/5/x86_64/RPMS/)
    * el6: [i386](http://www5.atomicorp.com/channels/ossec/centos/6/i386/RPMS/)
    * el6: [x86_64](http://www5.atomicorp.com/channels/ossec/centos/6/x86_64/RPMS/)
* Fedora
    * 20: [i386](http://www5.atomicorp.com/channels/ossec/fedora/20/i386/RPMS/)
    * 20: [x86_64](http://www5.atomicorp.com/channels/ossec/fedora/20/x84_64/RPMS/)
    * 19: [i386](http://www5.atomicorp.com/channels/ossec/fedora/19/i386/RPMS/)
    * 19: [x86_64](http://www5.atomicorp.com/channels/ossec/fedora/19/x84_64/RPMS/)
    * all: [6-20](http://www5.atomicorp.com/channels/ossec/fedora/)


## DEBs for Debian Wheezy, Jessie and Sid

Available in the [AlienVault](http://alienvault.com/) [repository](http://ossec.alienvault.com/repos/apt/debian/pool/main/o/)

* OSSEC Server
    * [Wheezy, Jessie, Sid](http://ossec.alienvault.com/repos/apt/debian/pool/main/o/ossec-hids/)
* OSSEC Agent
    * [Wheezy, Jessie, Sid](http://ossec.alienvault.com/repos/apt/debian/pool/main/o/ossec-hids-agent/)

## RPM Installation

To install with yum do the following:

    # wget -q -O – https://www.atomicorp.com/installers/atomic | sh
    # yum install ossec-hids ossec-hids-server (or ossec-hids-client for the agent)



## DEB Installation

To install with apt-get do the following:

    # wget -O – http://ossec.alienvault.com/repos/apt/conf/ossec-key.gpg.key | apt-key add –
    # echo “deb http://ossec.alienvault.com/repos/apt/debian wheezy main” >> /etc/apt/sources.list
    (change wheezy for your Debian distribution)
    # apt-get update
    # apt-get install ossec-hids  (or ossec-hids-agent)

## PGP key

Before you install any package from our project, we recommend that you
verify it using our PGP key. Follow these two steps if you are not used
to using gpg. You first need to import our public key:

    ossec-test# wget http://www.ossec.net/files/OSSEC-PGP-KEY.asc
    ossec-test# gpg –import OSSEC-PGP-KEY.asc

And then verify each file against its signature:

    ossec-test# gpg –verify file.sig file 

You should get the following result:

    gpg: Signature made Tue 19 Jul 2011 03:13:58 PM BRT using RSA key ID A3901351
    gpg: Good signature from “Daniel B. Cid ”
    Primary key fingerprint: 6F11 9E06 487A AF17 C84C E48A 456B 17CF A390 1351

_Note that the key expiration date was changed lately. If you get an
warning saying “gpg: Note: This key has expired!”, make sure to update
the key and run the “import” command again (as specified above)._


## Contribute back!

If you find ossec useful and would like to contribute back to the
community, please contact us. We have a lot of work to do and any help
is appreciated.




