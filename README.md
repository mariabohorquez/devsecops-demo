### Disclaimer

The base code of this project comes from this repo: https://github.com/cr0hn/vulnerable-node. Credits to @ggdaniel for his work on it.

## Project

Further changes to this repository are for a security course for Universidad Argentina de la Empresa (UADE). We will test how many vulnerabilities we can catch with different tools in the CI.

## Installation

The most simple way to run the project is using docker-compose, doing this:

```bash

# git clone https://github.com/cr0hn/vulnerable-node.git vulnerable-node
# cd vulnerable-node/
# docker-compose build && docker-compose up
Building postgres_db
Step 1 : FROM library/postgres
---> 247a11721cbd
Step 2 : MAINTAINER "Daniel Garcia aka (cr0hn)" <cr0hn@cr0hn.com>
---> Using cache
---> d67c05e9e2d5
Step 3 : ADD init.sql /docker-entrypoint-initdb.d/
....
```

## Running

Once docker compose was finished, we can open a browser and type the URL: `127.0.0.1:3000` (or the IP where you deployed the project):

![Login screen](https://raw.githubusercontent.com/cr0hn/vulnerable-node/master/images/login.jpg)

To access to website you can use displayed in landing page:

- admin : admin
- roberto : asdfpiuw981

# Vulnerabilities

## Vulnerability list:

This project has the most common vulnerabilities of `OWASP Top 10 <https://www.owasp.org/index.php/Top_10_2013-Top_10>`:

- A1  - Injection
- A2  - Broken Authentication and Session Management
- A3  - Cross-Site Scripting (XSS)
- A4  - Insecure Direct Object References
- A5  - Security Misconfiguration
- A6  - Sensitive Data Exposure
- A8  - Cross-Site Request Forgery (CSRF)
- A10 - Unvalidated Redirects and Forwards

# License

This project is released under license BSD.
