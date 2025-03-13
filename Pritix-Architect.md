# PritiX  - Proof of Concept for Learning Dictionaries 
>This assignment is part of the Xebia XMS Hiring process. You should have received companion documents that explains the details of the procedure and an overview of the company PritiX.

![PritiX Logo](/images/pritix.png)

## The Assignment
As Xebia we are asked to help PritiX in their endeavour. This repository contains the requirements for the Proof of Concept. 

PritiX wants to be able to quickly go to market with their new application and incrementally add features once the products gains traction. They value quality a lot and are looking for means to keep a high standard and quality level for their work. Testing vigorously and running the application reliably is an important part of their vision of modern software development. They want to go to market as soon as possible with their new application. This new application needs to be the example of how you should build applications for all other teams in PritiX. 

## Your Task
In a Proof of Concept, you need to show how to build a this application. Because there is limited time, you should pick and choose what you build, based on your expertise and based on what is most convincing to the customer to proof the value of Xebia. 

PritiX expects that we implement the application as outlined below in the chapter "The Application" and show them what technology they should choose and how they should construct the software following Cloud, Data,Software craftsmanship and DevOps principles you find most predominantly important. 

In the presentation you present the following
1. The Proof of Concept application according to your vision, so it can be used as an example how well-organized DevOps teams should build applications. It needs to contain the things you feel are crucial in building quality software, meet the requirements, and show your vision on architecture and continuous delivery.
2. Architectural Decision Records (ADR) to describe your decisions so you can explain them when asked.

## The application
The PritiX CEO wants to get to the market as soon as possible, to get money from investors. The CEO has a good relationship with the CEO of a big Social Media Platform, and they agreed that this new application can be featured on the homepage experience. This will put some tremendous pressure on the scalability of the application build and also the challenge of providing a solution that needs to run 24x7 with no maintenance downtime.

## Requirements
The envisioned application will help people learn words from a foreign language. For example, a Dutch girl in primary school needs to learn English words. The application will take practice tests in which the student must answer multiple choice or spelling questions on a set of words from a dictionary. Below you find User Stories for the Proof of Concept application. 

It is equally important to setup the relevant infrastructure and Deployment pipelines. No User stories have been created for this.

### :memo: US01 - Login to the application

The application is started for the first time. The student registers an account with a user name (email address) and password. After registration the student logs in and is shown a list of dictionaries. There is a sample dictionary present. 

### :memo: US02 - Create a new dictionary
The student creates a new dictionary and adds some words to it in 2 different languages

### :memo: US03 - Start a practice test
A choice is given for the type of test. There are three types of tests:
  1. Type along: type the translated word as displayed.
  2. Multiple choice: choose the right translated word from a list of 4 possibilities
  3. Translate: Translate the word by typing it

The test consists of an amount of questions that need to be answered. After completing the test the student is given the results. Closing the results returns the student to the dictionary list.

A test consists of a random ordered questions for the available words. The total number of words is configurable for a test.

### :memo: US04 - Continue to take practice tests

The student starts the application again and uses her account to log into the learning system. One of the dictionaries that was created in an earlier session is opened. It shows previous test results.

### :memo: US05 - The user can manage one or more dictionaries of words.
A dictionary is characterized by two languages: a primary language with a translation in another language. It contains at least 5 words with their translations. Words can be single words or expressions.

Here is an example of a dictionary:

| **Dutch** | **English** |
| --- | --- |
| Groente | Vegetable |
| Biefstuk | Steak |
| Zak chips | Bag of crisps |
| Kool | Cabbage |


## Checklist
For the Proof of Concept Presentation make sure you show what you thinbk is relevant and shows of your expertise. Whether this is the software, the (cloud) infrastructure, the automation or the pipelines, make sure you can show some "real" code. 

> Be realistic with the limited amount of time. This part is important as we want to assess your hands-on skills. It is also a starting point for the technical discussion of architecture, technology and development practices.

‼️As stated before, do reach out if and when you have any questions. Don't assume. Ask!
