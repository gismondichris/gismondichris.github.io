---
title: Automatic Network Drive Connection
roles:
  - Laboratory Data Manager
languages:
  - PowerShell
---

#### Summary
Accepts user credentials at login in order to reconnect
network drives on isolated network.

#### Description
The laboratory has an isolated network set up. This network 
allows access to certain locations (network drives, certain database servers, etc.)
but nothing else. This isolated network is mostly used with 
computers that are not updated because they have legacy software 
that is not guaranteed to run on new versions of the OS.

Since the computers are not on the domain, users must use local 
logins. However, the network drives require that credentials are verified 
every so many days or the network drives disconnect.

I created a PowerShell script that ran every time a user logged 
into the computer. This script would request the user's domain 
credentials and use them to reconnect the network drives. This ensured that 
the drives stayed connected.