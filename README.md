# CS-305
Files for SNHU CS-305

## Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?
Artemis Financial is a financial services company that wanted to update their current web applications to meet the most current standards for funcitonality and security. In particular, they wanted to make sure that data sent to and from their servers was both encrypted, and cryptographically verifiable.

## What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?
For the cryptographic hash function that would be used to verify the integrity of data, I chose one of the strongest and most advanced cipher algorithms currently available, SHA3-256. I also created the code that would carry out the hashing function on any given input data and display the generated checksum. My code was clean and efficient and the functionality that it provides will help the company keep data secure.

## What part of the vulnerability assessment was challenging or helpful to you?
The OWASP Dependency Check was the most helpful tool that I used during this project. It provides an amazingly thorough list of vulnerabilities present in dependencies used in system, such as the Spring Framework. In addition to showing existing vulnerabilities, the tool could also be used as new code was added to be sure that no new vulnerabilities had been inadvertently introduced into the system.

## How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
Adding the ability to produce an SHA3-256 checksum for any data being transmitted gives Artemis Financial the the ability to ensure that all data received is exactly as it was sent with no changes or manipulation of any kind in the middle. The company can now tell if data has been tampered with instantly.

I would use the OWASP Dependency check tool along with other tools such as the JUnit testing framework to look for vulnerabilities and make plans for removing any that are found.

## How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
I executed and tested the refactored code to make sure that it worked as expected and did not leak any kind of information if there was any kind of invalid input or other error. To be sure that I didn't accidentally add any new security vulnerabilities I first ran the OWASP Dependency tool on the original code and then ran it again after my refactoring. I then compared the results of the two reports to make sure there were no new problems found.


## What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
In addition to the dependency check tool, I found various websites with some examples of implementing different types of encryption techniques to be very helpful. I find that learning to research things correctly and efficiently is the biggest help of all. I needed to look up various details to make sure I was implementing my hash function correctly as well as creating the web server security certificate the right way.

## Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
I would show potential employers my refactored and functional code for implementing the hash cipher algorithm. I think that in addition to being functional, the code is well written and easy to understand. I believe that writing good code is not the same as writing functional code. Code needs to be efficient and easy to understand if you're going to be working as part of a team, which is how virtually every developer will be working.
