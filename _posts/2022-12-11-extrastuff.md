---
toc: true
layout: post
description: Extra Research Related to Sections 12-13
categories: [markdown]
title: Extra Research Related to Sections 12-13
---

In sections 12-13, we learned a lot about *procedure calls*. 

After doing some research, I found that there are also a few different types of procedure calls, both using *lists* of *parameters*. These types of procedure calls can be more applicable to the workings of the operating systems that we use on our devices everyday, especially Windows. Below, I'll give a brief overview of what I read about. 

**Type 1: Local Procedure Calls**:

To simplify this concept as much as possible, local procedure calls are utilized by ports on our system. Each port on our system is assigned to a different program. In this context, procedure calls are used by each port to essentially *call* each other and communicate. For example, if a port number is already taken up for a particular program, it communicates that with the other programs to make sure that that port is no longer usable elsewhere.

Another local procedure call machination comes through *file mapping*. This is mostly related to file sharing, where files are being shared across applications/processes. Procedure calls are very necessary in this case, as each process needs to call the other in order to effectively receive the file/multiple files that are being shared.

**Type 2: Remote Procedure Calls**: 

Remote Procedure Calls are especially useful on Windows machines. On Windows, Remote Desktop is an application that allows for one system to connect to another system in order to transfer files, share settings, etc. 

Remote procedure calls allow for this systems communication to take place. From each system calling each other (client to server), the client waits for a response from the server, and then the necessary data is unpacked once a response is received.


Overall, we can see that the concept of algorithmic procedure calls stretches far beyond the constraints of Python programming, and is a very interesting and essential programming principle.
