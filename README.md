# nex-forms_SQL-Injection CVE-2023-2114
https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-2114

https://wpscan.com/vulnerability/3d8ab3a5-1bf8-4216-91fa-e89541e5c43d

Quick Review about the SQL-Injection in the NEX-Forms Plugin for WordPress

## Uploaded exploit
Note that this uploaded exploit code isnt for this particular vulnerability... But this is an example how you could make an exploit for this issue.

## Vulnerable Versions
From Version 8.3 (Maybe earlier too) till version 8.4

## The SQL-Injection itself
The SQL-Injection is placed in the authenticated area from NEX-Forms. When you edit a form and want to safe it, your client sends a post-request to the server with some parameters.

One of those parameters is called 'table' which is vulnerable. There was no sanitizing or filtering.

## Screenshots
![request](https://user-images.githubusercontent.com/91736634/230071803-edb449a3-0d99-4574-9858-00444c3b36cc.PNG)
![save-button](https://user-images.githubusercontent.com/91736634/230071810-9b08bd2b-23fa-4625-af21-27d717c95e76.PNG)
![sql_error](https://user-images.githubusercontent.com/91736634/230071811-8bf5be21-4043-4a90-936f-03c5cada5a6c.PNG)
![database](https://user-images.githubusercontent.com/91736634/230071813-2d4ef627-085b-4611-86ff-db1cff665516.PNG)
