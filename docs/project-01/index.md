# Problem 1 - Received on 03/04/2019

## Problem asked by Google.

!!! note "Question"
    Given a list of numbers and a number k, return whether any two numbers from the list add up to k.

    For example, given [10, 15, 3, 7] and k of 17, return true since 10 + 7 is 17.

    Bonus: Can you do this in one pass?

??? hint "Answer"
    ``` javascript

    let n1 = [10, 15, 3, 7]
    let k = 17

    document.querySelector("#app").innerHTML =
    
    n1.filter((nm, i) => n1
        .map(n2 => (k === n2 + nm) 
        ? "TRUE" : null).join("")
    ).length > 0

    ```

!!! note "View result"

    <iframe style="width: 100%; height: 200px; border: none" src="https://dcp-project-jwknz.netlify.com/project-01/"></iframe>


<a class="btn btn-primary text-white" href="https://github.com/jwknz/dcp.jwk.nz/blob/master/projects/project-01/index.html" target="_blank">View Answer on Github</a>
