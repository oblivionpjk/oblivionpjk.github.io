---
title: Why JSON is more self-describing than CSV
tags: self-describing, json, csv
categories: theory
---

# question
Briefly (in no more than 250 words) and using suitable examples, explain what it means for an external representation to be self-describing, and whether we can say that JSON is more self-describing that CSVs.

# my opinion
In my opinion,if an external representation is self-describing, it can obtain the corresponding internal representation from it-self. This means, an self-describing external representation should not only include data but also contain a structure describing itself, It includes a set of system catalog tables, which describe the logical and physical structure of the data; a configuration file, which contains the parameter values associated with the database; and a recovery log, which records ongoing transactions and transactions that can be archived."(IBM)
For example:
an external representation is "Alice", "wfxian@263.net", "divadpeng". a self-describing external representation could tell us "Alice" is name, "wfxian@263.net" is email and "divadpeng" is id, which means we don't have to confused about the name and id and we can convert this external representation to an internal representation :rs("Alice")="jiangtianpeng",rs("Emial")="wfxian@263.net",rs("Id")="divadpeng"



# references
