# 2.4 - SQL Injection

## SQL Injection

### Topics

> 1. Introduction to SQL Injection
> 2. Finding SQL Injection
> 3. Exploiting In-Band SQL Injection
> 4. Exploiting Error-Based SQL Injection
> 5. Exploiting Blind SQL Injection
> 6. SQLMap
> 7. Mitigation Strategies
> 8. From SQLi to Server Takeover

<details>

<summary>SQLi</summary>

**SQL Injection (SQLi)** is an attack method that exploits the injection of SQL commands into a web application's SQL queries. A successful SQLi attack allows a malicious hacker to access and manipulate the backend database of a web application.

Web applications, ranging from complex systems to Content Management Systems (CMSs) and simple personal web pages, often utilize databases like MySQL, SQL Server, Oracle, PostgreSQL, and others to store data, user credentials, or statistics. Structured Query Language (SQL) is employed by entities such as system operators, programmers, applications, and web applications to interact with databases.

SQL, a powerful interpreted language, is used to extract and manipulate data from databases. Web applications embed SQL commands, known as queries, in their server-side code, with connectors serving as middleware between the web application and the database.

Before delving into attack techniques, understanding some SQL basics is essential. This includes knowledge of SQL statement syntax, query execution, union operations, the DISTINCT and ALL operators, and how comments function.

</details>

### Web Basics

* ​[Web Application Basics](https://attackdefense.com/listing?labtype=webapp-web-app-basics\&subtype=webapp-web-app-basics-getting-started)​
* ​[Web Apps Tools of Trade](https://attackdefense.com/listing?labtype=webapp-tools-of-trade\&subtype=webapp-tools-of-trade-getting-started)

{% content-ref url="https://app.gitbook.com/s/iS3hadq7jVFgSa8k5wRA/practical-ethical-hacker-notes/main-contents/14-hacking-web-apps" %}
[14 - Hacking Web Apps](https://app.gitbook.com/s/iS3hadq7jVFgSa8k5wRA/practical-ethical-hacker-notes/main-contents/14-hacking-web-apps)
{% endcontent-ref %}

{% content-ref url="https://app.gitbook.com/s/iS3hadq7jVFgSa8k5wRA/practical-ethical-hacker-notes/main-contents/15-sql-injection" %}
[15 - SQL Injection](https://app.gitbook.com/s/iS3hadq7jVFgSa8k5wRA/practical-ethical-hacker-notes/main-contents/15-sql-injection)
{% endcontent-ref %}

### Practise

🔬 There are many vulnerable testing web apps like:

* ​[Juice Shop - Kali Install](https://www.kali.org/tools/juice-shop/)​
* ​[DVWA - Kali Install](https://www.kali.org/tools/dvwa/)​
* ​[bWAPP](http://www.itsecgames.com/)​
* ​[Mutillidae II](https://github.com/webpwnized/mutillidae)

<details>

<summary>DVWA</summary>

**The Damn Vulnerable Web Application (DVWA)** is a web application built with PHP and MySQL intentionally designed to be susceptible to security vulnerabilities. Its primary purpose is to serve as a resource for security professionals to assess their skills and tools within a legal context. Additionally, it aids web developers in gaining a deeper understanding of the processes involved in securing web applications and facilitates learning about web application security for both students and teachers in a controlled classroom setting.

DVWA is designed to provide a platform for practicing various common web vulnerabilities at different difficulty levels, all presented through a simple and user-friendly interface. It's important to note that there are deliberate both documented and undocumented vulnerabilities within the software, encouraging users to explore and identify as many issues as possible.

</details>

{% embed url="https://github.com/digininja/DVWA" %}
DVWA
{% endembed %}

#### DVWA - My Writeups

{% content-ref url="https://app.gitbook.com/s/rRWtuMw6xkkeDjZfkcWC/dvwa" %}
[DVWA](https://app.gitbook.com/s/rRWtuMw6xkkeDjZfkcWC/dvwa)
{% endcontent-ref %}

#### Theory and Lab platform

{% embed url="https://portswigger.net/web-security/all-labs" %}
Web Burp Suite Security Academy
{% endembed %}

> #### ❗ Disclaimer
>
> * **Never use tools and techniques on real IP addresses, hosts or networks without proper authorization!**
