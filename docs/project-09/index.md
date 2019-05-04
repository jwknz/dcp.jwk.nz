# Problem 9 - Received on 11/04/2019

## Problem asked by Airbnb.

### Difficulty Level: Hard

!!! note "Question"
    Given a list of integers, write a function that returns the largest sum of non-adjacent numbers. Numbers can be 0 or negative.

    For example, [2, 4, 6, 2, 5] should return 13, since we pick 2, 6, and 5. [5, 1, 1, 5] should return 10, since we pick 5 and 5.


??? hint "Answer"

    ```
      let givenNumbers = [2, 4, 6, 2, 5]
      //let givenNumbers = [5, 1, 1, 5]

      let getNonAdjacentTotal = (gn) => {

        // Create a center number if there isn't one
        (gn.length % 2 !== 0) ? gn[((gn.length + 1) / 2) - 1] : gn[gn.splice(gn.length / 2,0,0)]

        //Testing to see what the center number
        //let centerNumber = gn[Math.floor(gn.length  / 2)]

        //Add all the numbers at an even index - arrays start at 0 index
        let total = null
        gn.map((n, i) => (i % 2 === 0) ? total += n : null) 
        
        return total
      }

      document.querySelector("#app").innerHTML = getNonAdjacentTotal(givenNumbers)
    ```

!!! note "View result"

    <iframe style="width: 100%; height: 200px; border: none" src="https://dcp-project-jwknz.netlify.com/project-09/"></iframe>


<a class="btn btn-primary text-white" href="https://github.com/jwknz/dcp.jwk.nz/blob/master/projects/project-09/index.html" target="_blank">View Answer on Github</a>