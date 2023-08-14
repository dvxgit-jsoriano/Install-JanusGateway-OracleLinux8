# Install-JanusGateway-OracleLinux8
This is a guide on how to install Janus Gateway on an Oracle Linux 8.7

## What is Janus Gateway
**Janus Gateway** is a **WebRTC Server** developed by Meetecho conceived to be a general purpose one. As such, it doesn't provide any functionality per se other than implementing the means to set up a WebRTC media communication with a browser, exchanging JSON messages with it, and relaying RTP/RTCP and messages between browsers and the server-side application logic they're attached to. Any specific feature/application is provided by server side plugins, that browsers can then contact via Janus to take advantage of the functionality they provide. Example of such plugins can be implementations of applications like echo tests, conference bridges, media recorders, SIP gateways and the like.

## Pre-Requisite
- [Oracle Linux 8.7](https://yum.oracle.com/oracle-linux-isos.html)
- [Janus Gateway](https://janus.conf.meetecho.com/)

NOTE: This guide will not teach you how to install Oracle Linux. Assuming you already know how to install the Oracle Linux 8. Below are the steps you can follow to install Janus Gateway.

## How to Install Janus Gateway
1. Install the epel release:

    ```
    dnf install epel-release
    ```


Notice that you may have to `yum install epel-release` as well if you're attempting an installation on a CentOS machine instead.