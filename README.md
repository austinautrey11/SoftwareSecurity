# SoftwareSecurity
Work from CS305 Software Security

Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

- The client that we worked with was Artemis Financial. Artemis Finanical is a financial consulting company that develops individual financial plans involving savings, retirements, investments, and insurance for their customers. Artemis would like to implement the most current security for their application. In turn, they have tasked me with adding a file verification step to their web application to confirm secure communications. They have specifically asked me to add this data verification step through the form of a checksum.

What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

- I feel like I did a great job of producing a proper checksum for this company. I did this by creating a keystore, and then adding the keystore to the application. I then refactored the code to include the properties of the keystore, switching from http to https protocol, and then adding an encryption algorithm cipher through the use of a checksum. I feel it is very important to code securely to help protect information. When information is not properly secure, then the risk of data breaches go up tremendously. In this example, secure coding will help protect both the customer's private information, and the company. Software security helps bring value to a company by giving the company piece of mind from breaches, and allowing them to keep their customers safe.

What about the process of working through the vulnerability assessment did you find challenging or helpful?

-  The most difficult part of working through the vulnerabilty assessment for me had to be trying to eliminate and discover false positives. I knew that if the CVVS score was under 7 that the vulnerability had a high chance of being a false positive. However, when it came to discovering which were used or not, this was extremley challenging. All of the vulnerabilties are listed as maven dependencies in the application. This led me to not being able to determine whether or not if they were being used in the application or not. I struggled with this on both this assignment and the previous assighnment. If you could shine some light on that for future learning for me, now that the course is over that would be greatly appreciated.

How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?

- In order to add layers of security, I practiced secure coding, generated a certificate, added it's keystore to the application, refactored the code to produce a checksum, and used the dependency check. In the future I feel like I will be using dependency checks a lot. This is one tool I will carry forward with me. I now just need to learn how to properly identify false positives.

How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?

- I ensured the code was functional and secure by switching from http to https. I then ran the code through a verify, compile, and finally spring boot run to ensure the code was functional. In order to check and see if I introduced new vulnerabilities, once I supressed vulnerabilities I would rerun the code to produce a new dependency check. I would then go back through the check to see if anything new was introduced, and whether or not it could be a false positive.

What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?

- The coding practice of generating and implementing a certificate will be very valuable to me in the future. I also will continue to access the vulnerability assessment diagram as well as the Java security algorithms, and NIST website.

Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?

- Two things that I would feel confident to show to an employer would be the ability to generate a certificate, and implement it in my code through the use of a keystore. The second ability I would like to showcase is the ability to produce a checksum including an algorithm cipher. I could also showcase my ability to examine a dependency check, but feel as if I need more experience learning how to correctly identify false positives.
