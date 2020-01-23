---
layout: project
type: project
image: images/bank.png
title: Bank Database
permalink: projects/ics212bank
# All dates must be YYYY-MM-DD format!
date: 2019-12-12
labels:
  - C
  - C++
summary: A bank database program for ICS 212
---

<img class="ui medium rounded image" src="/images/bankterminal.png">

This bank database program, developed using C and C++ utilizes pointers to access and remove information for targeted records in the database. Each record holds an account number, a name, and an address, and the records are sorted by account numbers from largest to smallest. 

We used pointers to chain all the bank records together and successfully add, modify, or remove records to and from the list. At the exit of the program, a cleanup function ensured that all the memory in the heap was cleared. A large part of the project was the user-interface, and making it user-friendly and easy for any person to use. 

From many encounters with segmentation faults, I have since learned that I am accessing information that isn't supposed to be accessed, as our professor would put it, "accessing someone else's house," resulting in runtime errors. During the process of creating this project, I found that writing the pseudocode and working out the solution before typing the code on the computer has taught me to approach the problem in more of a cognizant manner, rather than constantly fixing the code on the computer because of a mindless attempt. 

Source: <a href="https://github.com/wjinyan/212bank"><i class="large github icon "></i>wjinyan/212bank</a>

