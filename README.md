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

In this assignment, I played the role of a software developer for an engineering firm called Global Rain. Global Rain provides expertise for companies who want to build custom software solutions. In particular, they focus on building security into all of their client's applications. As an employee of Global Rain, I was assigned to a team working on a project for Artemis Financial. Artemis Financial is a consulting firm that helps individuals build personalized plans to meet their future financial needs. The primary goals for the project were to:

- Analyze the current system using both static dependency scanning and manual code reviews to identify possible security vulnerabilities.
- Research security issues to determine their impact on the system and filter out false positives.
- Provide recommendations on how to mitigate any security vulnerabilities or risks that were discovered.
- Analyze and recommend secure encryption ciphers and hashing algorithms.
- Refactor code to implement secure communications between the browser-based client and the application server.
- Implement a mechanism to verify data integrity using a secure hashing algorithm.
- Address other security issues found in the code to improve the overall security of the application.

### What did you do very well when you found your client's software security vulnerabilities? Why is it important to code securely? What value does software security add to a company's overall wellbeing?

Researching the vulnerability list produced by the OWASP dependency checker was a time-consuming process. However, I feel that I did a good job in analyzing each issue and coming up with a mitigation plan to reduce the overall risk to the application. Writing secure code is not always front and center in a developer's mind when they are building new features. However, it's important because it shows that you care about the product and the end users. It's also much easier to build security from the beginning than it is to refactor the code after it's already written. Writing secure code reduces risk to the business and allows them to focus on what they do best: running their application.

### What part of the vulnerability assessment was challenging or helpful to you?

The most challenging part of the process was trying to understand how certain vulnerabilities could impact the application. In many cases, the vulnerabilities are in open-source or third-party libraries that you are not familiar with. You really just have to either upgrade the library to a newer version or try to make an educated guess on the potential impact. In many cases, I found that it's easier just to avoid the problem by upgrading the vulnerable libraries instead of trying to resolve the problem in some other way. This might not always be possible but is preferable in many cases.

### How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

I increased layers of security in the application in several different ways. The starting point was to understand the client's goals and security needs. This initial analysis was followed by a vulnerability scan and manual testing. All of this was compiled into a [Vulnerability Assessment Report](Allan_ODriscoll_CS_305_Project_One_20231111.docx) along with a mitigation plan (O'Driscoll, 2023a). It's important to understand the starting point so that you can measure your progress. After this initial research, I started the implementation. This included the creation and installation of an SSL certificate to enable secure communications between the client and server, implementing code to validate data using a checksum, and addressing security vulnerabilities that were discovered earlier in the exercise. This process was documented in a [Practices for Secure Software Report](Allan_ODriscoll_CS_305_7_1_Project_Two_20231210.docx) (O'Driscoll, 2023b).

In the future, I will continue to use a similar process. Specifically, I would use tools like the OWASP Dependency Checker along with websites such as the National Vulnerability Database to analyze issues (OWASP, n.d.; NIST, n.d.). I would ensure that dependencies stay up to date as much as possible and would also follow recommendations such as the Oracle Secure Coding Guidelines for Java SE (Oracle, n.d.). These tools are provided free of charge and allow developers to leverage the work done by the open-source community to keep their software secure.

### How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?

Besides security scans provided by tools such as the OWASP Dependency Checker, I performed manual code reviews that were guided by the Vulnerability Assessment Process Flow Diagram (SNHU, n.d.). This diagram helped to maintain a focused approach to reviewing the application's security architecture and code base. After refactoring the code, I performed manual testing and executed a secondary dependency check to ensure that no new vulnerabilities had been introduced. I corrected several issues that I found and also reviewed the remaining issues to identify false positives. This process worked well and resulted in a secure application that met the client's needs.

### What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

A number of tools were introduced in this class that would be helpful for future school or work assignments. These are:

- The OWASP Dependency Checker. This tool helps automate static scanning for vulnerabilities found in open-source and third-party libraries.
- The National Vulnerability Database. This tool provides a comprehensive database of software vulnerabilities with links to websites providing additional analysis, reproduction procedures, and remediation steps.
- The Oracle Secure Coding Guidelines for Java SE. This tool provides a detailed list of secure coding practices that can be used to eliminate vulnerabilities and limit risk.
- The Vulnerability Assessment Process Flow Diagram. This tool provides a guided process to analyze an application's security architecture and perform code reviews.
- The Java Keytool Utility. This tool includes the functionaly to create and manage SSL certificates to establish secure communication channels for websites.
- The Tink Cryptography Library. This tool includes APIs for programatic encryption and decryption within an application (Tink, 2023).

### Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?

The two projects completed in this class ([one](Allan_ODriscoll_CS_305_Project_One_20231111.docx), [two](Allan_ODriscoll_CS_305_7_1_Project_Two_20231210.docx)) will be useful in showcasing skills for future employers. They show the end-to-end security analysis performed on an application, including remediation of known vulnerabilities and refactoring to enhance security. The ability to document this entire process from beginning to end demonstrates a developer's attention to detail and provides a reference for future projects. These documents provide concrete evidence of the skills developed in this class.

## References

NIST. (n.d.). *National Vulnerability Database.* NVD. https://nvd.nist.gov/

O’Driscoll, A. J. (2023a). *Artemis Financial Vulnerability Assessment Report.* GitHub. https://github.com/aodriscoll/allan-cs305/blob/main/Allan_ODriscoll_CS_305_Project_One_20231111.docx 

O’Driscoll, A. J. (2023b). *Practices for Secure Software Report.* GitHub. https://github.com/aodriscoll/allan-cs305/blob/main/Allan_ODriscoll_CS_305_7_1_Project_Two_20231210.docx

Oracle. (n.d.). *Keytool.* Keytool. https://docs.oracle.com/javase/8/docs/technotes/tools/unix/keytool.html 

Oracle. (2023, May). *Secure Coding Guidelines for Java SE.* Secure coding guidelines for java SE. https://www.oracle.com/java/technologies/javase/seccodeguide.html 

OWASP. (n.d.). *Owasp dependency-check.* OWASP Dependency-Check | OWASP Foundation. https://owasp.org/www-project-dependency-check/

SNHU. (n.d.). *Vulnerability Assessment Process Flow.* CS-305-H7001 Software Security 23EW2. https://learn.snhu.edu/content/enforced/1426327-CS-305-H7001-OL-TRAD-UG.23EW2/course_documents/CS%20305%20Vulnerability%20Assessment%20Process%20Flow%20Diagram.pdf?ou=1332052%2c1426327

Tink. (2023). *What is Tink? | tink | google for developers.* Google. https://developers.google.com/tink/what-is