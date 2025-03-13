# Xpirit Cloud Development Assessment

## Introduction

This assignment is part of the Xpirit assessment procedure for hiring new employees. You should have received a companion document that explains and details the procedure. Please ask for it if you did not.

In this cloud development assignment you will get an outline of a customer case that is interested in our services. It should not take you more than about 5-10 hours to complete depending on your pace. The assignment is intentionally open-ended to allow you to choose your own path and make your own choices. When in doubt, feel free to contact us and discuss.

## The assignment

You are asked to make acquaintance to a fictitious company BakerBuddy. BakerBuddy traditionally makes software for baker shops for inventory and bread recipe management.

![](images/mae-mu-Ehtxtp9Ykvo-unsplash.jpg)

_Photo by_ [_Mae Mu_](https://unsplash.com/@picoftasty?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) _on_ [_Unsplash_](https://unsplash.com/s/photos/sourdough-bread?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

Sourdough bread making at home has become massively popular over the past year. There is a large online community sharing recipes and photos on Instagram and other social media. BakerBuddy wants to provide an online platform for the sourdough community to facilitate creating and sharing recipes, and for bakers to keep a log of their bakes.

You have been given the assignment of designing an architecture and implementing an MVP for this platform.

## Your task

BakerBuddy aims to provide an API - or set of API's - that the sourdough community can use to consume in their own apps. The platform must be able to serve many users. They need to be able to create and share recipes. Recipes will be searchable for everyone and can be used by anyone.

For each loaf they make, bakers like to keep a _loaf log_. A loaf log keeps track of the recipe they used and records all the steps and modifications they make in the process. This helps them assess the quality of their bread and adjust their process on their next bake. Loaf logs are private for each user and will not be shared.

The high-level domain model looks as follows:

![](images/diagram.png#gh-light-mode-only)
![](images/diagram-dark.png#gh-dark-mode-only)

As a cloud developer, you have been tasked to come up with an architecture and sample (MVP) implementation of this sourdough community platform. You do not have to provide a front-end application, solely focus on a solid and highly scalable back end.

For BakerBuddy, this is all a big experiment, so it is crucial that the platform has very low operational cost from the start.

## User stories

Below are a few user stories that would be implemented in apps on top of the BakerBuddy platform. The platform should support this. _ **Note: feature completeness less important than a sound architecture, so select a few that you feel are feasible within the timeframe of the assignment.** _

### US01 – Create a recipe

As a baker, I want to create a new recipe and add it to my library so that I can use it to bake a new loaf of bread.

The baker creates a new entry, which is given a name, and a description (e.g. some instructions that are specific to the recipe), and a list of ingredients with their respective weights. The app will calculate the [baker's percentages](https://en.wikipedia.org/wiki/Baker_percentage) and [hydration level](https://truesourdough.com/sourdough-hydration-explained-what-why-how-when/), based on the proportions of the ingredients.

The recipe is saved for later use and will also be accessible for other users on the platform (sharing is caring).

### US02 – Like a recipe

As a baker, I want to 'like' a recipe that looks good to me, so that it becomes more popular, and I can find it back later when I want to bake a loaf from it.

This is achieved by recording a 'like' on a recipe. The number of likes is an indication of its popularity. The 'like' also serves as a bookmark so that the baker has the recipe available in their own library.

### US03 – Start a loaf log

As a baker, I want to start making a new loaf from a recipe, so that I can keep a record of it.

The baker selects a recipe from their own library - or from the public list after searching it – and starts a new loaf log. The loaf log captures each step of the process over time. It is based on a recipe, but the baker must always be able to tweak the weight proportions a bit, e.g. a little bit more water or salt. This must also be recorded in the loaf log.

### US04 – Record a step

As a baker, I want to record a step in the loaf log whenever I perform it, so that the process is recorded, and I can look back at it later on.

During the sourdough baking process, the baker performs several steps. Some examples are: mix dry ingredients, add water, add starter, start autolyse, knead, stretch & fold, shape, bake. Since time is an important factor, recording the timestamp with the action is important.

### USBONUS – Surprise us!

Looking at these four use cases, is there another cool feature you can think of and you want to show off? Surprise us! 😊

## Checklist

Make sure that you address the following aspects in your solution:

- **Technical solution architecture**
Come up with a technical solution architecture of this platform: what components make up your solution? How would you host this solution in the Azure cloud? How do you handle authentication, and how do you manage storage?
- **Minimum viable product**
 Implement a minimum viable product that demonstrates your solution architecture. We are most interested to see how you structure your code internally. This is more important to us than feature completeness.
- **DevOps**
 Setup an automated build and delivery pipeline(s) for your product. Also think about other aspects of the DevOps cycle that might be relevant.

> Do reach out if there are any questions. Don't assume. Ask!


![](images/jeremy-yap-h3tP-D2eABI-unsplash.jpg)

_Photo by_ [_Jeremy Yap_](https://unsplash.com/@jeremyyappy?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) _on_ [_Unsplash_](https://unsplash.com/s/photos/baker?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
