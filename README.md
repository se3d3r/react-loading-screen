## Display a loading screen while your complex React App initialises.
**ipl-progress-indicator** is an element in index.html that consists of a loading bar and a logo.

<img width="1440" alt="Loading Screen" src="https://user-images.githubusercontent.com/99820278/163048466-fe45f0bc-9ac4-4553-adf7-7480a592a3e5.png">

Once your react app is initialised, you can remove the loading screen with a nice transistion via:
```
const ele = document.getElementById('ipl-progress-indicator')
if(ele){
        // fade out
        ele.classList.add('available')
        setTimeout(() => {
          // remove from DOM
          ele.outerHTML = ''
        }, 2000)
 }
 ```
