# br
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Hacking Console</title>
<style>
body {
background-color: #000;
color: #fff;
font-family: 'Courier New', Courier, monospace;
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
margin: 0;
}

.container {
text-align: center;
padding: 20px;
width: 90%;
max-width: 600px;
}

h1 {
font-size: 2em;
margin-bottom: 20px;
text-transform: uppercase;
}

p {
font-size: 1em;
margin-bottom: 20px;
}

.button {
padding: 15px 30px;
background-color: #4CAF50;
border: none;
color: white;
font-size: 1em;
text-transform: uppercase;
cursor: pointer;
border-radius: 5px;
box-shadow: 0 5px #444;
transition: all 0.3s ease;
}

.button:hover {
background-color: #45a049;
box-shadow: 0 3px #444;
transform: translateY(2px);
}

.console {
width: 100%;
height: 300px;
background-color: #333;
color: #00FF00;
font-family: 'Lucida Console', Monaco, monospace;
font-size: 1em;
padding: 10px;
margin-top: 20px;
overflow-y: scroll;
border: 2px solid #4CAF50;
}

.console::before {
content: '>';
margin-right: 10px;
}

.input {
width: 100%;
padding: 10px;
background-color: #444;
border: none;
color: #00FF00;
font-family: 'Lucida Console', Monaco, monospace;
font-size: 1em;
margin-top: 10px;
box-sizing: border-box;
}
</style>
</head>
<body>
<div class="container">
<h1 style="color: red;">BHAgirath Console.com</h1>
<p>Welcome to the bhagirath' WEB<br>
</p>
<a href="Danger%20Warning%20Page.html"><button class="button"
onclick="startHacking()">Enter</button></a>
<div style="color: rgb(102, 0, 204);" class="console" id="console">
<p><span style="color: rgb(51, 255, 51);">enter your email/mobile nuber
<span style="color: red;">and enter&nbsp; </span>enter <br>
</span></p>
</div>
<input class="input" id="commandInput" placeholder="Enter command..."
type="text"> </div>
<script>
const consoleElement = document.getElementById('console');
const inputElement = document.getElementById('commandInput');

function startHacking() {
consoleElement.innerHTML += '<p>Starting hacking sequence...</p>';
// You can add more hacking simulation logic here
}

// Example: simulate typing in commands
inputElement.addEventListener('keyup', function(event) {
if (event.key === 'Enter') {
const command = inputElement.value;
consoleElement.innerHTML += '<p>> ' + command + '</p>';
inputElement.value = '';
// You can add more logic to process the command here
}
});
</script>
</body>
</html>
