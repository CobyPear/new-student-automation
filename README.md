# New Student Assignment to Spreadsheet Automation

Use this script to automatically add new student information (class code, graduation date, student name, and student email) directly to the Student Roster spreadsheet.

#### NOTE

This script only works with a Gmail account

## How To Use

1. Copy the source code from here (you'll want all three files. Code.gs, messages.html, and parsed.html): https://script.google.com/d/1TikNuUokzR7OAcGlgNdCVTjbq-67gN__feigHFbJwaxO6ApDRCS6DLqE/edit?splash=yes
2. go to script.google.com
3. click the New Project button ![image-20201107105248274](.\assets\image-20201107105248274.png)
4. Copy the files into your new project.
   1. The only parameters you need to change are line 58 in Code.gs. Here you will put the URL to your spreadsheet.
   2. You may change the last argument on line 8. This will be the number of emails that will be searched (default 4)
5. Deploy the project as a web app and accept the OAuth. ![image-20201107105544704](\assets\image-20201107105544704.png)
6. Back on the project page, click the hamburger menu>Triggers ![image-20201107105742607](.\assets\image-20201107105742607.png)
7. Add a trigger that runs the `processNewStudentEmails` function. You may choose whatever time interval you'd like, here is the recommended default:![image-20201107105916188](.\assets\image-20201107105916188.png)
8. Click save and you should see new students directly added to your spreadsheet!

## Future Development

- scrape Github Username and Time Difference as well
- convert into extension so user does not have to create own project

## Acknowledgements

Thanks Parsanth Janardanan, writer of the guide I used to build this (https://blog.gsmart.in/parse-and-extract-data-from-gmail-to-google-sheets/)

Thanks to John Blackwell for help with the RegExp and Queen Shabazz for checking in