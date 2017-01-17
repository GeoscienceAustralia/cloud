---
title: Code Security
layout: page
permalink: code_security_sub.html
---

### OWASP Top 10

The [OWASP Top 10](https://www.owasp.org/index.php/OWASP_Top_Ten_Cheat_Sheet) is a list of the most critical web application flaws. Checking your code against the Top 10 is a great first step to ensuring your application is secure.

### CWE Top 25

Similarly to OWASP's list, the [CWE Top 25](http://cwe.mitre.org/top25/index.html#Listing) is a list of the most widespread and critical errors that can lead to software vulnerabilities.

### Code review

Getting peers to review code can be another effective method of ensuring application security. It also helps to ensure code is comprehensible, well-documented, and understood by the whole team before going into production.

Some considerations to consider when conducting code reviews:

*Application Security* – This reminds developers to handle buffer overruns, mask or remove any internal resource references, and verifying server-side validity checks to coincide with client-side ones. Often overlooked security items such as session information, transaction controls, developer back-doors, and hard-coded passwords are questioned.

*Error Handling* – This area is looked at to help ensure safe and user-friendly end-user experiences by questioning function caller notifications, assertions, and exception handling. It’s also important not to give too much information in errors, so that is examined as well. Performance – Since this is always a concern, our checklist identifies some key areas that need to be reviewed, such as recursive functions, duplicated objects, system call blocks, and busy waits.

*Resource Leaks* – Resource leaks can cause and contribute to performance issues, so this could include questions regarding the freeing of allocated memory and objects, and tracking reference counts.

*Comments* - Well commented code will be easier to operate and maintain in the long run.

*Coding Conventions* - Adherence to coding standards/style/conventions (add link or references) helps to ensure consistency and readability and thus improve maintainability.
