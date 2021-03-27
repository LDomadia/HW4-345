# HW4 Answers
"I pledge my Honor that I have abided by the Stevens Honor System." - Leena Domadia

### Summary
#### REST Client
This was by far the most difficult homework assignment I have had in this semester. I do not have any experience writing in JavaScript, so I struggled throughout this entire assignment. I don't know what `await`, `return new Promise`, `request`, `resolve`, or any of the functions that were used in this assignment do. The GitHub API documents were not helpful at all. I wish we were taught in class about all these functions and what they do behind the scenes rather than me trying to Google search, looking at StackOverflow, trying to find help but unable to find anything.
I was able to get the test.js to eventually pass, but I am still left confused if I had successfully completed the assignment.

#### REST Server
This part was easier to handle. I was initially getting syntax errors when I ran the following command:
`curl --request POST -H "Content-Type: application/json" --data '{"coffee":1,"milk":1,"sugar":1,"chocolate":1}' http://localhost:3000/share`
After doing a Google search, I was able to find this [article](https://docs.oracle.com/en/cloud/saas/marketing/eloqua-develop/Developers/GettingStarted/APIRequests/curl-formats.htm#Windows) which shows that the command given to us was in macOS and I had to change the formatting of the command to this:
`curl --request POST -H "Content-Type: application/json" --data "{\"coffee\":1,\"milk\":1,\"sugar\":1,\"chocolate\":1}" http://localhost:3000/share`
After that, I was able to get the correct outputs in Command Prompt.

### Things I Learned
* `curl` statements work on Windows in Command Prompt, not in Powershell
* The `curl` statements are different on each operating system

### REST Client
test.js passing:
![REST_Client](REST_Client.jpg)

### REST Server
command outputs:
![REST_Server](REST_Server.jpg)