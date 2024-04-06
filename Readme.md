Found an IDOR bug in the https://pro.e-box.co.in/ platform.
It bascially is an already registered user can access all the unauthoruized 
learning content without paying the specific fees for the desired course.

Steps to reproduce:
1.) Login to your Ebox account.
2.) From there simply access the learning content or reading material.
3.) Then by altering the web page index we can navigate to any of the desired page we want to , in order to get access of any learning learning content available on the platform.
Example : https://pro.e-box.co.in/attempt/206089 {By changing the number 206089 to 206555 or any other index we can access a specific learning content which should be unauthorized.} 

Insecure Direct Object Reference (IDOR) is a vulnerability that arises when attackers can access or modify objects by manipulating identifiers used in a web application's 
URLs or parameters. It occurs due to missing access control checks, which fail to verify whether a user should be allowed to access specific data.

SEVERITY : HIGH.
