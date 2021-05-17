# 1. JQuery-like selector.

```javascript
let $ = selector => document.querySelector(selector);
let $$ = selector => document.querySelectorAll(selector);

// Example:
$('.my-first-div-with-class');
$$('.all-divs-with-class');

```
