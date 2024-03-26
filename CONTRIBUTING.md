# Open Source Community Contribution: 

## Part 1:  Assess External Communitie Contribution :  

### About the project :  Validator



The [Validator](https://github.com/validatorjs/validator.js) library is a JavaScript validation library commonly used in web development to validate various types of data, such as strings, numbers, dates, and more. It provides a simple and flexible way to validate input data and enforce validation rules.



 ### **Summary of issues:**


I stumbled upon an issue that I believe could serve as a valuable opportunity for learning and contributing to an open-source project. This particular issue appears to align well with my interests and expertise, making it an ideal candidate for my involvement.

So the issue was in the date validation function: the date is validated when the date is clearly not valid. You can put hyphen in the beginning of a date and it is treated as the right format.


Expected behavior
"-2012" not valid

Actual behavior
"-2012" valid




### Contribution

* I've created a fork of the original code. You can access my fork through this link.

* Following that, I established a dev branch from the fork to address the issue at hand.

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


### Reflection

My contribution to the Validator library reflects my commitment to fostering collaborative development within the open-source community. By actively engaging with the project, I not only addressed a specific issue but also gained valuable insights into code review, testing, and collaboration practices. Moving forward, I look forward to continuing my involvement in open-source projects, further honing my skills and making meaningful contributions to the community.







## Part 2:  pattern Library Contribution :  

