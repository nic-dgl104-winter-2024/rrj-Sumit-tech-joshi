# Open Source Community Contribution: 

## Part 1:  Assess External Communitie Contribution :  

### About the project :  Validator



The [Validator](https://github.com/validatorjs/validator.js) library is a JavaScript validation library commonly used in web development to validate various types of data, such as strings, numbers, dates, and more. It provides a simple and flexible way to validate input data and enforce validation rules.



 ### Summary of the selected issue:


I stumbled upon an issue that I believe could serve as a valuable opportunity for learning and contributing to an open-source project. This particular issue appears to align well with my interests and expertise, making it an ideal candidate for my involvement.

So the issue was in the date validation function: the date is validated when the date is clearly not valid. You can put hyphen in the beginning of a date and it is treated as the right format.


Expected behavior
"-2012" not valid

Actual behavior
"-2012" valid




### Contribution

* I've created a [fork](https://github.com/Sumit-tech-joshi/validator.js) of the original code. You can access my fork through this link.

* Following that, I established a dev [branch](https://github.com/Sumit-tech-joshi/validator.js/tree/dev-date-issue) from the fork to address the issue at hand.

* I conducted a thorough review of the code implementation to understand how the validation operates within the project.

* Upon testing the issue alongside its test cases, I successfully pinpointed the root cause.

* Subsequently, I introduced the necessary code to rectify the issue and ensured its effectiveness by including the appropriate test cases in the .test file.

* To resolve the problem, I implemented a validator pre-fix check on the year.

```javascript
// Check if the year starts with a hyphen
    if (fullYear.startsWith('-')) {
      return false; // Hyphen before year is not allowed
    }
``` 
* Created [pull request](https://github.com/validatorjs/validator.js/pull/2381 for the same
)  

### Detailed discussion of code review and outcomes

* Got comments on PR by [repository owner](https://github.com/WikiRik) for adding test cases. [Link for the comment](https://github.com/validatorjs/validator.js/pull/2381#pullrequestreview-1956457214)

* Also got comment from [Mitsuhiro Kadota](https://github.com/michiwo1) for same test cases.

* Added require test cases for the date and updated the PR [#2381](https://github.com/validatorjs/validator.js/pull/2381)
.

* Received a comment on the PR regarding the addition of the new date function in the test case. After conducting research on the JavaScript (Date function)[https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date], I added a comment on the PR with my findings.



### Reflection

My contribution to the Validator library reflects my commitment to fostering collaborative development within the open-source community. By actively engaging with the project, I not only addressed a specific issue but also gained valuable insights into code review, testing, and collaboration practices. Moving forward, I look forward to continuing my involvement in open-source projects, further honing my skills and making meaningful contributions to the community.


### References

[JavaScript Date function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)


---
---

## Part 2:  pattern Library Contribution :  

### About the Selcted issue on the pattern Library:

I have chosen to document the contrast between functional patterns and object-oriented programming (OOP) because, based on my previous experience with JavaScript, I believe delving into pattern implementation for both paradigms will greatly benefit programmers in understanding and selecting design patterns.

I believe that by providing a comprehensive exploration of functional patterns and OOP, programmers will gain valuable insights into the intricacies of each approach. This understanding will make it easier for them to make informed decisions when choosing the appropriate design patterns for their projects.

## Contribution

Actions I've taken with respect to Pattern Library Issues:

* Added a comment on issue [#27](https://github.com/nic-dgl104-winter-2024/pattern-library/issues/27) to be assigned for doing research on Contrast functional patterns vs. OOP design patterns in README.md

* Worked on the issue [#27](https://github.com/nic-dgl104-winter-2024/pattern-library/issues/27), wrote the fidings on implementation of the Singleton pattern and made a pull request to merge my forked repository with the main pattern library repository

* Finished work on the issue and created PR [#59](https://github.com/nic-dgl104-winter-2024/pattern-library/pull/59) for the same.

* Got comments on PR #59 and reviewed them.

* Attempted to remove conflicts on the PR, leading to the need to rebase the branch and resulting in automatic closure of the PR. As a result, a new PR [#73](https://github.com/nic-dgl104-winter-2024/pattern-library/pull/73) was created.

* After conflict resolution, a comment was received on the PR [#73](https://github.com/nic-dgl104-winter-2024/pattern-library/pull/73) suggesting a change in the structure of the comparison.

* All comments on the PR [#73](https://github.com/nic-dgl104-winter-2024/pattern-library/pull/73) have been addressed, and another review is requested.



## Reflections

In this task, I engaged in exploring the contrast between functional patterns and object-oriented programming (OOP) design patterns in JavaScript. Initially, I expressed interest in the subject and was assigned the responsibility to conduct research and contribute to the project. My focus centered on implementing the Singleton pattern, which involved understanding its principles and intricacies within the JavaScript context. Subsequently, I submitted a pull request (PR [#59](https://github.com/nic-dgl104-winter-2024/pattern-library/pull/59)) to integrate my findings into the main pattern library repository.

However, the process wasn't without challenges; I encountered conflicts during the review phase, necessitating the creation of a new PR [#73](https://github.com/nic-dgl104-winter-2024/pattern-library/pull/73) to address these issues. Despite this setback, I remained receptive to feedback and diligently addressed comments and suggestions to refine the contribution.

This task provided valuable insights into collaborative software development practices, emphasizing effective communication, adaptability, and attention to detail. Moreover, it underscored the significance of comprehending different programming paradigms and patterns, highlighting their diverse approaches to problem-solving and the importance of selecting the most suitable approach for a given context. Overall, this experience reinforced the importance of persistence and flexibility in navigating challenges and achieving successful outcomes in collaborative projects.

## References

[Javascript string function: startWith()](https://www.w3schools.com/jsref/jsref_startswith.asp#:~:text=The%20startsWith()%20method%20returns,()%20method%20is%20case%20sensitive.)

[Writing test cases in Javascript](https://www.lambdatest.com/learning-hub/javascript-unit-testing) 



## Discussion of next steps
For the next steps, I have started working on another issue in the same repository for solving email validation [issue](https://github.com/validatorjs/validator.js/issues/2360). However, few of the test cases failed, so I need to debug and resolve them on the same pull request after testing. Apart from this, I will take on more issues from the [validator library](https://github.com/validatorjs/validator.js/issues). I find it really interesting as the issues are easy to understand but require a lot of research, especially since they mainly focus on core JavaScript. This will help me strengthen my JavaScript skills.
