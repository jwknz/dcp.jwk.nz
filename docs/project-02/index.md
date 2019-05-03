# Problem 1 - Received on 03/04/2019

## Problem asked by Uber.

!!! note "Question"
    Given an array of integers, return a new array such that each element at index i of the new array is the product of all the numbers in the original array except the one at i.

    For example, if our input was [1, 2, 3, 4, 5], the expected output would be [120, 60, 40, 30, 24]. If our input was [3, 2, 1], the expected output would be [2, 3, 6].

    Follow-up: what if you can't use division?

??? hint "Answer"

    ```
    let numbers = [3, 2, 1]
    let removeIndex = []
    let answers = []
    numbers.map(nm => {
        removeIndex.push(numbers.filter(n => {
            return (nm !== n)
        }))
    })
    answers.push(removeIndex.map(x => {
        let t = 1;
        x.map(y => t *= y)
        return t
    }))
    document.querySelector("#app").innerHTML = answers
    ```

!!! note "View result"

    <iframe style="width: 100%; height: 200px; border: none" src="https://dcp-project-jwknz.netlify.com/project-02/"></iframe>


<a class="btn btn-primary text-white" href="https://github.com/jwknz/dcp.jwk.nz/blob/master/projects/project-02/index.html" target="_blank">View Answer on Github</a>