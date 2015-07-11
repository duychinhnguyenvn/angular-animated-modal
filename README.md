# Angular animated modal

Agular directive for [animatedModal.js](http://joaopereirawd.github.io/animatedModal.js), a jQuery plugin to create a fullscreen modal with CSS3 transitions.

## Installation
You should already have a bunch of scripts and CSS required below:
```html
<head> 
	<link rel="stylesheet" href="http://cdnjs.cloudflare.com/ajax/libs/animate.css/3.2.0/animate.min.css"> 
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script> 
	<script src="yourPath/animatedModal.min.js"></script> 
	<script src="yourPath/angular.js"></script> 
	<script src="yourPath/angular-animated-modal.js"></script> 
</head>
```
Then, inject `angular-animated-modal` in your application module:
```javascript
angular.module('myApp', ['angular-animated-modal']);
```
## Usage
In your HTML just add attribute `animated-modal` to any `a` or `button` and bind it to the `div` modal that you want by `href="#div_ID"`.
```html
<a animated-modal href="#myModal">My Modal</a>
<!--div modal-->
<div id="myModal">
	<!--THIS IS IMPORTANT! to close the modal, the class name has to match the name given on the ID  class="close-animatedModal" -->
	<div class="close-myModal"> 
		CLOSE MODAL
	</div>            
	<div class="modal-content">
		<!--Your modal content goes here-->
	</div>
</div>
```
## Demo
Please view demo at this link http://angularanimatedmodal.oqbox.com

## License
Apache License Version 2.0