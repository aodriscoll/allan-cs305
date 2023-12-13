# allan-cs305
SNHU CS-305 Software Security

``` text
 _____  _   _  _   _  _   _   _____  _____        _____  _____  _____ 
/  ___|| \ | || | | || | | | /  __ \/  ___|      |____ ||  _  ||  ___|
\ `--. |  \| || |_| || | | | | /  \/\ `--.  ______   / /| |/' ||___ \ 
 `--. \| . ` ||  _  || | | | | |     `--. \|______|  \ \|  /| |    \ \
/\__/ /| |\  || | | || |_| | | \__/\/\__/ /      .___/ /\ |_/ //\__/ /
\____/ \_| \_/\_| |_/ \___/   \____/\____/       \____/  \___/ \____/ 
```

|              |     |
| ------------ | --- |
| Institution  |  Southern New Hampshire University   |
| Course       | [CS-305-H7001 Software Security 23EW2](https://learn.snhu.edu/d2l/home/1426327 "CS-305-H7001 Software Security 23EW2")    |
| Instructor   |  Ross Foultz, DCS ([rfoultz@snhu.edu](mailto:rfoultz@snhu.edu))   |
| Course Dates |  10/23/2023 - 12/17/2023   |
| Status       |  Active/Online   |

## 8-1 Journal: Portfolio Submission

### Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

In this assignment I played the role of a software developer for an engineering firm called Global Rain. Global Rain provides experties for companies who want to build custom software solutions. In particual, they focus on building security into all of their client's applications. As an employee of Global Rain, I was assigned to a team working on a project for Artemis Finanical. Artemis Financial is a consulting firm that helps indivivuals build personalized plans to meet their future financial needs. The primary goals for the project were to:

- Analyze the current system using both static dependency scanning and manual code reviews to identify possible security vunerabilities.
- Research security issues to determine their impact on the system and filter out false positives.
- Provide recommendations on how to mitigate any security vulnerabilities or risks that were discovered.
- Analyze and recommend secure encryption ciphers and hashing algorithsm.
- Refactor code to implement secure communications between the browser-based client and the application server.
- Implement a mechanism to verify data integrity using a secure hashing algorithm.
- Address other security issues found in the code to imporove the overall security of the application.

### What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

Researching the vulnerability list produced by the OWASP dependency checker was a time consuming process. However I feel that I did a good job in analyzing each issue and coming up with a mitigation plan to reduce the overall risk to the application. Writing secure code is not always front and center in a developers mind when they are building new features. However, it's important because it shows that you care about the product and the end users. It's also much easier to build security in from beginning than it is to refactor the code after it's already written. Writing secure code reduces risk to the business and allows them to focus on what they do best, running their application.

### What part of the vulnerability assessment was challenging or helpful to you?

The most challenging part of the process was trying to understand how certain vulnerabilites could impact the application. In many cases the vulnerabilites are in open-source or third party libraries that you are not familiar with. You really just have to either upgrade the library to a newer version or try to make an educated guess on the potential impact. In many cases I found that it's easier to just avoid the problem by upgrading the vulnerable libraries instead of trying to resolve the problem in some other way. This might not always be possible, but is preferable in many cases.

### How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

### How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

### What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

### Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?