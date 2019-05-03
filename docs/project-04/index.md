# Problem 4 - Received on 06/04/2019

## Problem asked by Stripe.

### Difficulty Level: Hard

!!! note "Question"
    Given an array of integers, find the first missing positive integer in linear time and constant space. In other words, find the lowest positive integer that does not exist in the array. The array can contain duplicates and negative numbers as well.  
      
    For example, the input [3, 4, -1, 1] should give 2. The input [1, 2, 0] should give 3.

??? hint "Answer"

    ```
    let numbers = [3, 4, -1, 1] // also in the question is [1, 2, 0]

    numbers.sort()

    let positiveNumbers = numbers.filter(n => n > 0)
    
    let firstMissingPositiveNumber = 
      positiveNumbers.filter((cn, ci) => cn + 1 !== positiveNumbers[ci + 1])[0] + 1

    document.querySelector("#app").innerHTML = firstMissingPositiveNumber
    ```

!!! note "View result"

    <iframe style="width: 100%; height: 200px; border: none" src="https://dcp-project-jwknz.netlify.com/project-04/"></iframe>


<a class="btn btn-primary text-white" href="https://github.com/jwknz/dcp.jwk.nz/blob/master/projects/project-04/index.html" target="_blank">View Answer on Github</a>