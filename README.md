\# Amazon EFS Shared Storage for Content Management Club



\## Project Overview



This project implements a shared cloud storage solution for a Content Management Club using Amazon Elastic File System (Amazon EFS).



Two Amazon EC2 instances are connected to the same EFS file system, allowing both servers to access the same documents, images, and videos.



\## Problem Statement



A Content Management Club needs centralized storage where files can be stored and accessed by multiple servers.



Using separate local storage on different servers can make file sharing and collaboration difficult.



\## Proposed Solution



Amazon EFS is used as shared storage between two Amazon EC2 instances.



```text

Server 1 ─────┐

&#x20;             │

&#x20;             ▼

&#x20;         Amazon EFS



&#x20;             │

&#x20;             ▲

&#x20;             │

Server 2 ─────┘

