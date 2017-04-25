# Project 8 - Pentesting Live Targets

Time spent: 5 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation


Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

It's very troublesome to do GIF everytime, so I'm going to describe each vulnerability in detail instead

## Blue

Vulnerability #1: SQLi
If you go to salesperson and show any of the salesperson and change the query parameter id= injection.

Vulnerability #2: Session Hijacking/Fixation
PHPSESSID is always the same. As long as you can obtain it and set the cookie to it you can hijack the session.


## Green

Vulnerability #1: Username Enumeration
The text is bolded when you enter a valid username and not bolded when it's not.

Vulnerability #2: XSS
When you submit a feedback with XSS vulnerability, you can see it in the logged in feedback section.


## Red

Vulnerability #1: IDOR
When you go to public's show salesperson and change the query parameter ID to one that's not supposed to be
visible, such as 10, it works.

Vulnerability #2: CSRF
When you enter an invalid CSRF token it works also(But must have the right session and user-agent).

## Notes

None
