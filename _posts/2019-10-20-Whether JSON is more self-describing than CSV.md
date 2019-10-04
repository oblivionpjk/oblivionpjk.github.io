---
title: Whether JSON is more self-describing than CSV
tags: self-describing, json, csv
categories: theory
---

# question
Briefly (in no more than 250 words) and using suitable examples, explain what it means for an external representation to be self-describing, and whether we can say that JSON is more self-describing that CSVs.

# my opinion
In my opinion, if a data model is self-describing, it can obtain the corresponding internal representation from the external representation. This means, a self-describing data model should not only include data but also contain a description which describe the logical and physical structure of the data.

For example: an external representation is "Alice", "wfxian@263.net", "divadpeng". a self-describing data model could tell us "Alice" is name, "wfxian@263.net" is email and "divadpeng" is id, which means we don't have to confused about the name and id and we can convert this external representation to an internal representation: rs("Alice") = "jiangtianpeng", rs("Emial") = "wfxian@263.net", rs("Id") = "divadpeng". Of course, Self-describing includes not only these, but also restrictions on format, input, content, etc.

Speaking of the self-describing of csv and json, since the internal format corresponding to an external CSV/JSON description depends crucially on the CSV/JSON Schema that is used for validation, I think it's inappropriate to say that JSON is more self-describing than CSV. If some pathological schemas do not describe the data well，they may have poor effects on validation and lead to poor self-describing of data models. However, in normal cases, CSV is not easily guessable and requires background knowledge. For instance, we don't know the field names in CSV, but in json, we can easily get the field names corresponding to each attribute. From this point of view, it can be considered that JSON is more self-describing than CSVs. 


# references
1. Jérôme Siméon, & Wadler, P. . (2003). The essence of xml. Acm Sigplan Notices, 38(1), 1-13.
