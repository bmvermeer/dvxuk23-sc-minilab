# Secure Coding Lab: Building Secure Java Applications
## Devoxx UK 2023 - MiniLAB

----
## Required software
- Java 11 or higher
- Maven installed
- Decent IDE (preferably IntelliJ Community or Ultimate latest version)
- unrestricted access to your work machine
- A Github account with unrestricted access


This application is an intentional vulnerable Java Spring-Boot application with Thymeleaf.
It is use for training purposes only!

The code is and layout of the application is based on https://github.com/hieutdo/waa-coffee-shop
However it is heavily edited, updated and includes security problems by design!

Please do not use this application and workshop in any other way than intended or without consent of [Brian Vermeer](https://brianvermeer.nl).

---

## Getting started

- Fork this repository to your own GitHub account
- Check out the forked repository
```
git clone https://github.com/<your_username>/<forked-repo>.git 
```
- Sign up for a free Snyk account at https://snyk.io/signup (unless you already have one)
- Connect the forked project to your Snyk projects and leave it there.

## Run the application
- Go to the root folder of the application and run using Maven
```
mvn spring-boot:run
```
- The application fills itself with data at startup wait until you see `READY` in the console.
- You can access the application on http://localhost:8081
- By default there are two users configured you can access

| Username | Password | User type |
|----------|----------|-----------|
| Admin    | admin    | ADMIN     |
| User     | user     | CUSTOMER  |

---

# Assignments

## Assignment 1
Even without logging in, you can browse the menu and search for specific items
Set all prices of all product to 0.00 so everything is for FREE
- Use the searchbox for this and try

- [Hint 1](workshop/freeloader/hint1.md)
- [Hint 2](workshop/freeloader/hint2.md)
- [Hint 3](workshop/freeloader/hint3.md)
- [Hint 4](workshop/freeloader/hint4.md)
- [Hint 5](workshop/freeloader/hint5.md)

Fix the issue the appropriate way

- [Hint 6](workshop/freeloader/hint6.md)
- [Solution](workshop/freeloader/solution.md)

## Assignment 2
Create a link that displays the JSESSIONID

- [Hint 1](workshop/takeacookie/hint1.md)
- [Hint 2](workshop/takeacookie/hint2.md)
- [Hint 3](workshop/takeacookie/hint3.md)


Execute some JavaScript that displays the JSESSIONID when someone opens a specific product page.
This means the script will NOT be part of the URL like in part1

- [Hint 4](workshop/takeacookie/hint4.md)
- [Hint 5](workshop/takeacookie/hint5.md)
- [Hint 6](workshop/takeacookie/hint6.md)

Fix the issue the appropriate way

- [Hint 7](workshop/takeacookie/hint7.md)
- [Solution](workshop/takeacookie/solution.md)

## Assignment 3
Update your libraries to versions without vulnerabilities.

- [Hint 1](workshop/hardening/hint1.md)
- [Hint 2](workshop/hardening/hint2.md)

Ignore dependencies we cant fix.
- [Hint 3](workshop/hardening/hint3.md)

Fix as many of the code issues that are left.

Update the encryption used to store the passwords
- [Hint 4](workshop/hardening/hint4.md)
- [Hint 5](workshop/hardening/hint5.md)