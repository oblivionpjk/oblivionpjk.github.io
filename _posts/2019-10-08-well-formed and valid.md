---
title: well-formed and valid
tags: xml,well-formed,valid
categories: theory
---

# question
Briefly (in no more than 250 words), explain an application where we have a situation that does not require input documents to be valid (for example against a RelaxNG schema, etc.) but instead merely well-formed. Explain as well how a (RelaxNG) schema might still be useful in this situation. 

# my opinion
Well-formed means that a textual object meets the W3C requirements for being XML. Valid means that well-formed XML meets additional requirements given by a specified schema(such as XSD, RELAX NG, Schematron, etc).
Suppose such a scene, we need to deal with a document. What we should do is to analyse the address information in the document and collect them. However this document contains a lot of information including name, age, address, phone and email. So, we only care about address in formation and the other information which validate against a specified schema is useless for us. In this situation, the document just need to be well-formed and need not validate aganist a specific schema. In addition, a schema is still useful in this situation, because, we can identify those relevant parts (addresses) in the document througn validating against a schema. 
In other situation such as find arithmetic expression in XHTML document, wo also don't require input documents to be valid but just well-formed. 

# reference
