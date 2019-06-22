+++
title = "Scale Laravel Application"
outputs = ["Reveal"]
+++

#### **Enable Laravel Application for high growth**

{{% note %}}
1m

* Who am I?
* How many of are you using laravel?
* How many of are you facing downtime and scaling issue?
{{% /note %}}

---
### **Scaling types?**

{{% note %}}
4m

* Explain scaling 

{{% /note %}}

---
### **Vertical Scaling**


{{% note %}}
10m

* Explain Vertical Scaling
  * It's easy to upgrade server
  * Almost no changes in application
  * But not a good option for really a large application
{{% /note %}}

---
### **Horizonal Scaling**

{{% note %}}
13m

* Explain Horizontal Scaling
  * Distribution of load among different server  
  * It's complex
  * We will deep dive in Horizonal Scaling as it's the only way to handle very large application.
{{% /note %}}

---
### **Changes in our laravel application** 
Our application can't scale horizontally without changes

{{% note %}}
14m


{{% /note %}}

---
### Use SCM

* Git/SVN or any type of SCM tool must be used 

{{% note %}}
15m
When we are building a large application, there will be many people who are supposed to work together. We can enforce to use SCM from very beginning of the project.
{{% /note %}}

---
### Latest Depedency

Try to use composer.json for depedencies and lock your depedency file(.lock) so you can ensure that which version of package is working with you.

{{% note %}}
15m

{{% /note %}}

---
### Don't use local files driver

By Default, laravel uses files for session, cache storage. That should be changed to i.e database, redis etc.

{{% note %}}
18m

{{% /note %}}

---
### Use event based work flow

Don't handle complex scenario synchronosly, queue up with SQS (i.e email, event handling etc)

{{% note %}}
23m
Explain scenario of creating account in one system can trigger so many other things, sending email, entry in other systems etc.
{{% /note %}}

---
### Environment based config

We can create separate .env file as per environment.

{{% note %}}
28m

* Each environment should have their own personal configuration file, so system should pick based on their environment.

{{% /note %}}

---
### Test Case Coverage

Try to cover most of your code in testing. It helps when adding new features

{{% note %}}
30m

* Explain why test cases is important in large application.
* End-to-end testing is desirable but not necessary.

{{% /note %}}

---
### Code style

Whole team should adopt any particular style for writing code along with auto format. (i.e PHP_CodeSniffer, php-cs-fixer)

{{% note %}}
34m

* Use tools for enforcing style in your code so you don't have messy code.

{{% /note %}}

---
### CI/CD Setup

Continuous Integrations and Deployment.

{{% note %}}
38m

* Explain strategy of how does it CI/CD works.

{{% /note %}}

---
### Thanks!

Shailesh Davara ([@sdavara](https://twitter.com/sdavara))

[improwised.com](https://www.improwised.com)
