# Problem 9 - Received on 11/04/2019

## Problem asked by Apple.

### Difficulty Level: Medium

!!! note "Question"
    Implement a job scheduler which takes in a function f and an integer n, and calls f after n milliseconds.


??? hint "Answer"

    ```
      let showAlert = () => {
        document.querySelector('#app').innerHTML = `Job Function!` 
      }

      let JobScheduler = (f, n) => {
        setTimeout(f, n); // called after a certain time
        //setInterval(f, n) // repeat every time n milliseconds passes
      }

      JobScheduler(showAlert, 3000)
    ```

!!! note "View result"

    <iframe style="width: 100%; height: 200px; border: none" src="https://dcp-project-jwknz.netlify.com/project-10/"></iframe>


<a class="btn btn-primary text-white" href="https://github.com/jwknz/dcp.jwk.nz/blob/master/projects/project-10/index.html" target="_blank">View Answer on Github</a>