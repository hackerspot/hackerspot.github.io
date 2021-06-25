---
title: Owasp Top 10 Security Vulnerabilities - 2017
description: Top vulnerabilities identified by OWASP top 10 in 2017
tags:
 - web-security
---

# OWASP Top 10 Security Vulnerabilities - 2017

The OWASP Top 10 is an awareness document created by OWASP team. This is a standart for developers and web application security. It represents a broad consensus about the most critical security risks to web applications. Companies and organisations use this document as a reference and adopt to their infrastructure. Interviewers asks many questions about this topic. So in this page we explain OWASP Top 10 vulnerabilities, vulnerable code examples and protection mechanisms.

## 1. Injection

Injections are dangerous attacks to any web application. In this attack, the attacker basically sends malicious data, in order to make the application process it and do something it is not supposed to do. Injection flaws are very prevalent, particularly in legacy code. The core reason being the input data is not validated, filtered or sanitized by the application. This could then get processed by an interpreter as part of a command or query which in turn gets manipulated to execute what the attacker wants, deviating from the original flow.

Some other possibel reasons about injection attacks:
- Using dynamic queries directly in the interpreter.
- Using non-parameterized calls without implementing context-aware escaping (auto-escaping in short) directly in the interpreter. Read more about escaping all user-supplied input here.
- Hostile data being used within object-relational mapping (ORM) search parameters to extract additional, sensitive records.
- Hostile data being used or concatenated directly, such that the SQL or command contains both structure and hostile data in dynamic queries, commands, or stored procedures.

### Injection Attack Types

- <b>SQL Injection:</b> SQL injection is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database. It generally allows an attacker to view data that they are not normally able to retrieve. This might include data belonging to other users, or any other data that the application itself is able to access. In many cases, an attacker can modify or delete this data, causing persistent changes to the application's content or behavior. In some situations, an attacker can escalate an SQL injection attack to compromise the underlying server or other back-end infrastructure, or perform a denial-of-service attack.
- <b>NoSQL Injection:</b> NoSQL injection vulnerabilities allow attackers to inject code into commands for databases that don’t use SQL queries, such as MongoDB. NoSQL injection attacks can be especially dangerous because code is injected and executed on the server in the language of the web application, potentially allowing arbitrary code execution. 
- <b>Command Injection:</b> Command injection is a cyber attack that involves executing arbitrary commands on a host operating system (OS). Typically, the threat actor injects the commands by exploiting an application vulnerability, such as insufficient input validation. For example, a threat actor can use insecure transmissions of user data, such as cookies and forms, to inject a command into the system shell on a web server. The attacker can then leverage the privileges of the vulnerable application to compromise the server.
- <b>Template Injection: </b>
- <b>LDAP Injection:</b>
- <b>XSS(arbitrary script injection):</b>
- <b>Email header injection:</b>
- <b>XPATH injection:</b>
- <b>Host Header injection:</b>

- [https://owasp.org/www-project-top-ten/2017/A1_2017-Injection](https://owasp.org/www-project-top-ten/2017/A1_2017-Injection)
- [https://deepsource.io/blog/owasp-top-ten-injection/](https://deepsource.io/blog/owasp-top-ten-injection/)
- [https://www.siemba.io/post/owasp-top-10-injection-attacks](https://www.siemba.io/post/owasp-top-10-injection-attacks)

## 2. Broken Authentication

## 3. Sensitive Data Exposure 