---
title: well-formed and valid
tags: xml,well-formed,valid
categories: theory
---

# question
Briefly (in no more than 250 words), explain an application where we have a situation that does not require input documents to be valid (for example against a RelaxNG schema, etc.) but instead merely well-formed. Explain as well how a (RelaxNG) schema might still be useful in this situation. 

# my opinion
Well-formed means that a textual object meets the W3C requirements for being XML. Valid means that well-formed XML meets additional requirements given by a specified schema(such as XSD, RELAX NG, Schematron, etc).
In my opinion, validating against a specific schema is not a necessary process. a document can be valid w.r.t a specific schema(such as RelaxNG schema) even if it has not been validated through schema.this means as long as the document satisfies all constraints in schema, it is valid and not need to validate against a specific schema. 
Suppose such a situation, we need to deal with a document. What we should do is to analyse the address information in the document and collect them. However this document contains a lot of information including name, age, address, phone and email. So, we only care about address information and the other information is useless for us. In this situation, we can recognize those address information in the document and these relevant parts satisfied schema constaints. So the document just need to be well-formed and do not need to validate aganist a specific schema. In addition, a schema is still useful in this situation, because, we can test whether those relevant parts (addresses) in the document is valid  through validating against a schema. 
In other situation such as finding arithmetic expression in XML document, if we are able to ignore irrelated things, we also don't require input documents to be valid but just well-formed. 

# reference
