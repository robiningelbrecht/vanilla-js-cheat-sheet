# 1. Events

```javascript
window.addEventListener('DOMContentLoaded', event => {
  /* Your DOM just loaded */
});

window.onload = event => {
  /* Your media (images, etc.) just loaded */
}

```

# 2. jQuery-like selector

```javascript
let $ = selector => document.querySelector(selector);
let $$ = selector => document.querySelectorAll(selector);

// Example:
$('.my-first-div-with-class');
$$('.all-divs-with-class');

```
# 3. Async calls

```javascript
let make = function(payload) { return { method: 'post',
    headers: { 'Accept': 'application/json', 'Content-Type': 'application/json' },
    body: JSON.stringify(payload) };
}

fetch("https://www.twitter.com/followers.json", make({token:token})).then( (response) => response.text().then(msg => {
    console.log(msg); // Text message returned from the server
}));  

```                                      
    
