Popsicle JS
===========

Popsicle JS fires the following custom events:
* onefingertap
* swipeleft
* swiperight
* swipeup
* swipedown
* twofingertap
* threefingertap
* fourfingertap

### Download Popsicle JS
[Download Popsicle JS Version 1.0](https://raw.githubusercontent.com/codyhess/popsiclejs/master/popsicle.js)

### Import Popsicle JS
```html
<script src="/path/to/popsicle.js"></script>
```

### Create a popsicle (raw) and bind an event.
```javascript
var popsicle;
var myElement;

document.addEventListener('DOMContentLoaded', function() {
  popsicle = new Popsicle(); // popsicle binds to body by default
  myElement = document.getElementById('myElement');
  myElement.addEventListener('twofingertap', function(event) {
    alert('Two Finger Tap on ' + event.target);
  });
});

```

### Create a Popsicle (jQuery)
```javascript
var popsicle;
var $myElement;

$(document).ready(function() {
  popsicle = new Popsicle(); // popsicle binds to body by default
  $myElement = $('#myElement');
  $myElement.on('twofingertap', function(event) {
    alert('Two Finger Tap on ' + event.target);
  });
});
```
