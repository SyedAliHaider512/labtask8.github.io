<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portfolio</title>
<style>
body {
font-family: 'Comic Sans MS', sans-serif;
margin: 0;
padding: 0;
overflow-x: hidden;
}

header {
background-color: #111;
color: #fff;
text-align: center;
padding: 2em 0;
}

section {
height: 50vh;
display: list;
align-items: center;
justify-content: center;
text-align: center;
}

section:nth-child(odd) {
background: linear-gradient(45deg, #fc5c7d, #6a82fb);
}

section:nth-child(even) {
background: linear-gradient(45deg, #a18cd1, #fbc2eb);
}
h2 {
font-size: 3em;
margin-bottom: 30px;
color: #fff;
}

p {
font-size: 1.2em;
color: #fff;
}

nav {
position: center;
top: 0;
left: 0;
height: 100%;
background-color: #333;
padding-top: 20px;
}

nav a {
display: list;
padding: 20px;
color: #fff;
text-decoration: none;
transition: background-color 0.3s;
}
nav a:hover {
background-color: #555;
}

.download-btn {
padding: 20px 30px;
background-color: #333;
color: #fff;
border: none;
cursor: pointer;
font-size: 1.2em;
}

.tooltip {
position: relative;
display: inline-block;
cursor: pointer;
}

.tooltip .tooltiptext {
visibility: hidden;
width: 120px;
background-color: #333;
color: #fff;
text-align: center;
border-radius: 6px;
padding: 5px;
position: absolute;
z-index: 1;
bottom: 125%;
left: 50%;
margin-left: -60px;
opacity: 0;
transition: opacity 0.3s;
}

.tooltip:hover .tooltiptext {
visibility: visible;
opacity: 1;
}
</style>
</head>
<body>

<nav>
<a href="#about">About</a>
<a href="#services">Services</a>
<a href="#contact">Contact</a>
</nav>

<header>
<h1>Air University</h1>
<p>Kamra Campus</p>
</header>

<section id="about">
<h2>About Me</h2>
<p>I'm a Product Designer.</p>
</section>

<section id="services">
<h2>Services</h2>
<div class="tooltip">
<span class="tooltiptext">Web Designing</span>
<p>Web designing &nbsp;</p>
</div>

<div class="tooltip">
<span class="tooltiptext">Branding</span>
<p>Branding &nbsp;</p>
</div>

<div class="tooltip">
<span class="tooltiptext">Photography</span>
<p>Photography</p>
</div>
</section>

<section id="contact">
<h2>Contact</h2>
<p>Email: 235080@aack.au.edu.pk</p>
<p>Phone: 03034567890</p>
</section>

<section>
<button class="download-btn" id="downloadBtn">Download Resume</button>
</section>
<body>
<button id="downloadBtn">Download PDF</button>
<script>
document.getElementById("downloadBtn").addEventListener("click", function() {
var pdfUrl = "https://drive.google.com/file/d/1eOlRiVEri3cFu6ezQ_Q-TIwXHf647pT3/view?usp=drive_link";
var link = document.createElement('a');
link.href = pdfUrl;
link.download = "downloaded_file.pdf";
link.target = "_blank";
link.click();
});
</script>
</body>
</html>
