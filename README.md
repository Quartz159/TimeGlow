<!DOCTYPE html>
<html>
<head>
<title>Time of Now</title>
<style>
body {
background-color: black;
color: white;
font-size: 48px;
text-align: center;
height: 100vh;
margin: 0;
}
</style>
</head>
<body>
<div id="time"></div>
<script>
function updateTime() {
const now = new Date();
document.getElementById('time').textContent = now.toLocaleTimeString();
}
setInterval(updateTime, 1000);
updateTime(); // initial call
</script>
</body>
</html>                                            <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Khaled's Time</title>
<style>
body {
background-color: black;
color: white;
font-family: 'Courier New', Courier, monospace;
display: flex;
justify-content: center;
align-items: center;
flex-direction: column;
height: 100vh;
margin: 0;
overflow: hidden;
}

#quote {
font-size: 28px;
opacity: 0;
animation: fadeIn 2.6s ease-in-out forwards;
}

#time {
font-size: 48px;
margin-top: 30px;
}

@keyframes fadeIn {
to {
opacity: 1;
}
}
</style>
</head>
<body>
<div id="quote">Time only moves forward… just like Khaled.</div>
<div id="time"></div>

<script>
function updateTime() {
const now = new Date();
document.getElementById('time').textContent = now.toLocaleTimeString();
}
setInterval(updateTime, 1000);
updateTime(); // initial call
</script>
</body>
</html>
