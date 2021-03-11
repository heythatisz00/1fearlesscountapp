Part 1: Developing Phase
This web application is developed using JavaScript, HTML.

The steps invloved using this app are given as below:

Step 1: Install Node.js
	Node.js is open source server enviroment that creates server for web hosting.
Step 2: Create app.js 
	Create a file named app.js that contains "hostname", "port", and server. 
 	Following three commands are used in this process:
	--const hostname = '127.0.0.1';
	--const port = 3000;
	--const server = http.createServer((req, res)
Step 3:Create index.html:
	The index.html file is developed that contains the button which increases its value on click. 
 	The following tags are used while developing this perticular process:
 	--<div class="form-group"><button class="btn btn-info" id="magic-button" onclick="counter()">Hit</button></div>
Step 4:JavaScript code integrated with https://countapi.xyz/: 
	For implementation of functionality of button JavaScript code is emplyed 
 	that urge html button to increase its vlaue by 1 when clicked. The certain part of code is given as below:
 	<script>
	function counter(){
		$.getJSON("https://api.countapi.xyz/hit/mysite.com/visits", function(response) {
		    $("#counter").text(response.value);
		});
	}
	</script>.



Part 2:Execution of the app:
	To execute this app you need to follow following simple steps:
Step 1: Once you installed node.js and have created app.js file, 
	run app.js file in commant prompt using command - node app.js. Make sure you in in a directory where app.js is saved.
Step 2: Viste http://localhost:3000 on your browser (preferbaly Chrome) where you will see the html element button.
	click the button and experence the the value is being increaed by 1 upon each click.