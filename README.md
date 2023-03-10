# Testing Strategies

## Table of Contents

- [White box testing](#white-box-testing)
- [Unit Testing](#unit-testing)
- [Integration Testing](#integration-testing)
- [Functional Testing](#functional-testing)
- [Regression Testing](#regression-testing)
- [Performance Testing](#performanceptesting)
- [Security Testing](#security-testing)

### White box testing

Tests the internal code structure and logic of the software.

### Unit Testing

Tests individual units or components of the software to ensure they are functioning as intended.

### Integration Testing

Tests the integration of different components of the software to ensure they work together as a system.

### Functional Testing

Tests the functional requirements of the software to ensure they are met.

### Regression Testing

Tests the software after changes or modifications have been made to ensure the changes have not introduced new defects.

### Performance Testing

Tests the software to determine its performance characteristics such as speed, scalability, and stability.

### Security Testing

Tests the software to identify vulnerabilities and ensure it meets security requirements.

## Software Testing Objectives

- The process of investigating and checking a program to find whether there is an error or not and does it fulfill the requirements or not is called testing.
- When the number of errors found during the testing is high, it indicates that the testing was good and is a sign of good test case.
- Finding an unknown error that wasn’t discovered yet is a sign of a successful and a good test case.

The main objective of software testing is to design the tests in such a way that it systematically finds different types of errors without taking much time and effort so that less time is required for the development of the software.

![testing](https://media.geeksforgeeks.org/wp-content/uploads/20200605230034/Untitled226-1.png)

The overall strategy for testing software includes:

- <b>Before testing starts, it’s necessary to identify and specify the requirements of the product in a quantifiable manner.</b> Different characteristics quality of the software is there such as maintainability that means the ability to update and modify, the probability that means to find and estimate any risk, and usability that means how it can easily be used by the customers or end-users. All these characteristic qualities should be specified in a particular order to obtain clear test results without any error.

- <b>Specifying the objectives of testing in a clear and detailed manner. </b> Several objectives of testing are there such as effectiveness that means how effectively the software can achieve the target, any failure that means inability to fulfill the requirements and perform functions, and the cost of defects or errors that mean the cost required to fix the error. All these objectives should be clearly mentioned in the test plan.

- <b>For the software, identifying the user’s category and developing a profile for each user. </b>Use cases describe the interactions and communication among different classes of users and the system to achieve the target. So as to identify the actual requirement of the users and then testing the actual use of the product.

- <b>Developing a test plan to give value and focus on rapid-cycle testing. </b>Rapid Cycle Testing is a type of test that improves quality by identifying and measuring the any changes that need to be required for improving the process of software. Therefore, a test plan is an important and effective document that helps the tester to perform rapid cycle testing.

- <b>Robust software is developed that is designed to test itself.</b> The software should be capable of detecting or identifying different classes of errors. Moreover, software design should allow automated and regression testing which tests the software to find out if there is any adverse or side effect on the features of software due to any change in code or program.

- <b>Before testing, using effective formal reviews as a filter. </b> Formal technical reviews is technique to identify the errors that are not discovered yet. The effective technical reviews conducted before testing reduces a significant amount of testing efforts and time duration required for testing software so that the overall development time of software is reduced.

- <b>Conduct formal technical reviews to evaluate the nature, quality or ability of the test strategy and test cases. </b> The formal technical review helps in detecting any unfilled gap in the testing approach. Hence, it is necessary to evaluate the ability and quality of the test strategy and test cases by technical reviewers to improve the quality of software.

- <b>For the testing process, developing a approach for the continuous development. </b> As a part of a statistical process control approach, a test strategy that is already measured should be used for software testing to measure and control the quality during the development of software.

# Everything you need to know about Visual Regression Testing

## Introduction

Visual Regression Testing has come a long way and it’s growing increasingly popular. And if you want to implement it in your project, what tools do you choose? Fear not, for in this article we will give you a comprehensive overview of all there is to know about Visual Regression Testing.

### What is Automated Visual Regression testing?

Visual testing is about checking for unintended changes to an application’s look and feel.

At a high level, automated visual regression testing follows the following steps:

- Step 1: Open a browser
- Step 2: Simulate user interaction on the app
- Step 3: Take screenshots of the app
- Step 4: Compare screenshots with the stored baseline image
- Step 5: Present comparison results to dev/tester

Examples of things visual regression testing tests include checking for an app’s background colour, element positions, content overflows and animation.

### What makes visual testing difficult to automate？

Steps 1–3 above can be achieved quite easily with many browser testing tools such as [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/) or [Cypress](https://www.cypress.io/)

The challenge comes in Step 4 — screenshot comparison.

It’s easy to compare two images pixel by pixel but the trouble is that browsers don’t always render every pixel the same. Minute differences could occur if the page is rendered with different monitors, or different graphics cards, using different browser versions, or a different OS etc. This means that if we perform an exact 1:1 pixel comparison, two screenshots that look identical to humans could fail because they’ve been rendered with completely different pixels. For example:

![compare](https://miro.medium.com/v2/resize:fit:1294/format:webp/1*FSSY6R17ViANsdcar7pZEA.png)
