www.w3schools.com

https://www.csszengarden.com/

https://www.codecademy.com/

Loo oma konto... teha läbi: Learn HTML ja Learn CSS. Tulemuste link saata Heiki Terras'ele.

[02.12.2022.zip](https://github.com/AlvinKask/Veebirakenduste-alused/files/10141165/02.12.2022.zip)

[04.02.23.zip](https://github.com/AlvinKask/Veebirakenduste-alused/files/10608267/04.02.23.zip)


[kavand-3.pdf](https://github.com/AlvinKask/Arvutivorkude-alused/files/9930621/kavand-3.pdf)

# 1 - Algus
```
<html>
<head>
<meta charset="UTF-8">
<title>UTF-8 Encoding</title>
</head>
<body>
<h1>Õudne</h1>
</body>
</html>
```

# 2 - Värvid
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Internal style rules</title>
<style type="text/css" media="screen">
h1	{ color : blue; background : yellow }
h2	{ color : white; background : green }
p	{ color : red }
</style>
</head>
<body>
<h1 style="color:blue;background:yellow">Heading styled by CSS</h1>
<h2 style="color:white;background:green">Sub-heading styled by CSS</h2>
<p>Paragraph styled by CSS</p>
</body>
</html>
```

# 3 - Hierarhia
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Evaluating Importance</title>
<link rel="stylesheet" type="text/css" href="importance.css">
</head>
<body>
<h2>Element style</h2>
<h2 id="heading-2">Identity style</h2>
<h2 class="headers">Class style</h2>
</body>
</html>
```

# 4 - Box
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Content Box Model</title>
<link rel="stylesheet" type="text/css" href="box.css">
</head>
<body>
<p>Content Box</p>
<p class="pad">Content Box - Padded</p>
<p class="pad bdr">Content Box - Padded + Border</p>
<p class="pad bdr mgn">Content Box - Padded + Border + Margin</p>
/* Kasutab classi puhul .css failis leiduvaid parameetreid */
</body>
</html>
```

### 4 - box.css
```
p	{ background : yellow; width : 20em }
p.pad	{ padding : 1em }
p.bdr	{ border : 0.5em red solid }
p.mgn	{ margin : 2em }
```

# 5 - Taust 1
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Background</title>
<link rel="stylesheet" type="text/css" href="background.css"
</head>
<body>
<p> <span>Repeat - Default</span></p>
<p id="x"><span>Repeat-X</span></p>
<p id="y"><span>Repeat-Y</span></p>
<p id="no"><span>No Repeat</span></p>
</body>
</html>
```

### 5 - background.css
![tile](https://user-images.githubusercontent.com/115221752/199756486-98a255b4-32f0-44bc-a8ac-9092f3506728.png)

```
span	{ background : yellow; margin : 0 0 0 10em }
p	{ background : url(tile.png) fuchsia repeat ; height : 3.5em }
p#x	{ background-repeat : repeat-x }
p#y	{ background-repeat : repeat-y }
p#no	{ background-repeat : no-repeat }
```

# 6 - Taust 2
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Background</title>
<link rel="stylesheet" type="text/css" href="background2.css"
</head>
<body>
<div id="box-1"> </div>
<div id="box-2"> </div>
<div id="box-3"> </div>
</body>
</html>
```

### 6 - background2.css
![flower](https://user-images.githubusercontent.com/115221752/199756536-9c0a08c1-57c4-4067-9329-ecc2aeb7c829.png)

```
div { float : left ; margin : 10px ; height : 120px ; width : 120px ; border: 5px solid black ; background : url(flower.png) ; }
div#box-1	{ background-size : 100% 100% }
div#box-2	{ background-size : 50% 50% }
div#box-3	{ background-size : 200% 200% }
```

# 7 - Kodulehe alge
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Columns</title>
<link rel="stylesheet" type="text/css" href="columns.css">
</head>
<body>
<div id="wrapper">
	<div id="hdr">Header Panel<br><img src="tile.png" width="250"
	height="25" alt="Box"></div>
	
	<div id="nav">Navigation Panel<br>&bull;Link<br>&bull;Link</div>

	<div id="ads">Supplement Panel<br><img src="tile.png" width="75"
	height="100" alt="Box"></div>
	
	<div id="txt">Content Panel<br><img src="tile.png" width="150"
	height="300" alt="Box"></div>
</div>
<div id="ftr">Footer Panel</div>
</body>
</html>
```

### 7 - columns.css
```
* { margin: 0; padding : 0 ; text-align : center }

html,body { height: 100%; }

#wrapper
{
	min-height: 100%;
	height: auto !important;
	height: 100%;
	margin: 0 auto -30px;
}

#hdr { height: 60px; background : aqua}
#ftr { height: 30px; background : aqua;}
#nav { float : left; width : 100px ; background : yellow }
#ads { float : right; width : 100px ; background : fuchsia }
#txt { margin: 0 100px; background : lime }
```

# 8 - Kuubikud
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Columns</title>
<style type="text/css">
.wrapper {
	background-color: #A0D953;
	height: 300px;
	width: 300px;
	margin-right: auto;
	margin-left: auto;
	position: absolute;
}
.sinine{
	background-color: #4177C0;
	height: 100px;
	width: 100px;
}
.valge{
	background-color: #FDFDFD;
	height: 100px;
	width: 100px;
	margin-top: -100px;
	margin-left: 200px;
}
.must{
	background-color: #2B2B2B;
	height: 100px;
	width: 100px;
	margin-top: 0px;
	margin-left: 100px;
}
.punane{
	background-color: #E5373A;
	float: left;
	height: 50px;
	width: 50px;
	margin-top: -75px;
	margin-left: 125px;
}
.oranz{
	background-color: #FC9819;
	height: 30px;
	width: 100%;
}
</style>
</head>

<body>
<div class="wrapper">
	<div class="sinine"></div>
	<div class="valge"></div>
	<div class="must"></div>
	<div class="punane"></div>
	<div class="oranz"></div>
	
</div>

</body>
</html>
```

# 9 - nav_bar_horizontal_piltideta
```
<!DOCTYPE html >
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
<title>CosmoFarmer</title>
<style type="text/css">
	
/* BASIC */
body {
	font: 62.5% Verdana, Arial, Helvetica, sans-serif;
	margin: 0;
	padding: 20px;
}


/* NAVIGATION */
ul#mainNav {
	border-left: 1px dashed #999999;
	margin: 0;
	padding: 0;
	list-style: none;
	float: left;
}

#mainNav li {
	float: left;
	width: 12em;
}

#mainNav a {
	text-decoration: none;
	color: #000000;
	font-size: 1.1em;
	text-transform: uppercase;
	border: 1px dashed #999999;
	border-left: none;
	display: block;
	padding: 7px 5px 7px 30px;
	background: #E7E7E7;
}

#mainNav a:hover {
	background: #B2F511;
	font-weight: bold;
}

/* special formatting for home page link */
a#homeLink {
	background: #E7E7E7;
}

/* styles for the "you are here" buttons */
#home #mainNav a#homeLink,
#feature #mainNav a#featureLink {
	background: #FFFFFF;
	padding-right: 15px;
	padding-left: 30px;
	font-weight: bold;
}

#home #mainNav a#homeLink:hover,
#feature #mainNav a#featureLink:hover {
	color: #B2F511;
}

</style>
</head>
<body id="feature">
  <ul id="mainNav">
    <li><a href="http://www.delfi.ee" id="homeLink">Home</a></li>
    <li><a href="04.11.22.html" id="featureLink">Features</a></li>
    <li><a href="#" id="expertLink">Experts</a></li>
    <li><a href="#" id="quizLink">Quiz</a></li>
    <li><a href="#" id="projectLink">Projects</a></li>
    <li><a href="#" id="horoscopeLink">Horoscopes</a></li>
  </ul>

</body>
</html>
```

# 10 - Varjutamine & ümarad nurgad & liikumine
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Box-Shadow</title>
<link rel="stylesheet" type="text/css" href="box-shadow.css"
</head>
<body>
	<div id="box-1"> </div>
	<div id="box-2"> </div>
	<div id="box-3"> </div>
</body>
</html>
```

### 10 - box-shadow.css
```
div { float : left ; margin : 10px ; height : 120px ; width : 120px ; border: 1px solid black }
div#box-1 { border-radius : 40px ; box-shadow : 5px 5px 10px gray }
div#box-2 { border-top-left-radius : 50px ; border-bottom-right-radius : 50px ;box-shadow : 10px 10px 10px lime inset }
div#box-3 { border-radius : 165px ; box-shadow : 0 0 10px 10px aqua }

div#box-1:active { border-radius : 40px ; box-shadow : 5px 5px 10px gray ; transform : rotate( 45deg) }
div#box-2:hover	{ border-top-left-radius : 50px ; border-bottom-right-radius : 50px ;box-shadow : 10px 10px 10px lime inset; transform : scale( 0.5) }
div#box-3:active { border-radius : 25px ; box-shadow : 0 0 10px 10px aqua ; transform : rotateZ(180deg) }
```

# 11 - Highlighting
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Highlighting content</title>
<link rel="stylesheet" type="text/css" href="highlight.css"
</head>
<body>
	<p> In what was once Texcoco lake, birthplace of <span>pre-Hispanic civilizations</span>, lies the <span lang = "es">Ciudad de los Palacios</span> (City of Places) that is today, Mexico City.</p>
	
	<p>Mexico City offers visitors a great many different interesting sites to visit, from <span>pre-Columbian Mexico</span> to modern and <span>cosmopolitan 21st century Mexico</span>.</p>
</body>
</html>
```

### 11 - highlight.css
```
p:first-letter { font-size : 200% ; color : red }
p:first-line { background-color : yellow }
*:lang(es) { background-color : lime }
span:first-child { background-color : aqua }
```

# 12 - paiknemine
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Background Position</title>
<link rel="stylesheet" type="text/css" href="paiknemine.css">
</head>
<body>
<p>Content Box</p>
<p><span>Top Left - Default</span></p>
<p id="p1"><span>Bottom Left</span></p>
<p id="p2"><span>20% 50%</span></p>
</body>
</html>
```

### 12 - paiknemine.css
```
span { background : yellow ; margin 0 0 0 10em }
p { background: url(tile.png) fuchsia no-repeat ; height : 3.5em }
p#p1 { background-position : bottom left }
p#p2 { background-position : 20% 50% }
body { background: url(tile.png) no-repeat bottom right fixed }
```

### 13 - Checkbox
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Checkbox Example</title>
</head>
<body>
<form method="GET" action="http:localhost/echo.pl">
<p>Yes, I would like to receive details
<input type="checkbox" name="Ask For" value="Details" checked>
</p>
<fieldset>
<legend>Activities of Interest...</legend>
Sailing <input type="checkbox" name="Do" value="Sail"><br>
Walking <input type="checkbox" name="Do" value="Walk"><br>
Driving <input type="checkbox" name="Do" value="Drive"><br>
Skiing <input type="checkbox" name="Do" value="Ski"><br>
Jogging <input type="checkbox" name="Do" value="Jog"><br>
</fieldset>
<p>
<input type="submit" value="Submit form">
</p>
</form>
</body>
</html>
```

### 14 - Radio
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Radio Button Example</title>
</head>
<body>
<form method="GET" action="http:localhost/echo.pl">
<p>Choose only one answer...</p>
<fieldset>
<legend>What kind of language is HTML?</legend>
Scripting <input type="radio" name="Definition" value="Scripting"><br>
Markup <input type="radio" name="Definition" value="Markup"><br>
Programming <input type="radio" name="Definition" value="Programming" checked>
</fieldset>
<p>
<input type="submit" value="Submit form">
</p>
</form>
</body>
</html>
```

### 15 - Dropdown
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Dropdown</title>
</head>
<body>
<form method="GET" action="http:localhost/echo.pl">
<select name="HTML List Type Selector One" size="4">
<optgroup label="List Type">
<option value="UL">Unordered List</option>
<option value="OL" selected>Ordered List</option>
<option value="DL">Definition List</option>
</optgroup>
</select>
<input type="submit" value="Submit form">
</p>
</form>
</body>
</html>
```

### 16 - Text input
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Text input</title>
</head>
<body>
<form method="GET" action="http:localhost/echo.pl">
<dl>
<dt> User Name:</dt>
<dd><input type="text" name="Name"> </dd>
<dt> Password:</dt>
<dd><input type="password" name="Password"> </dd>
<dt> City:</dt>
<dd><input type="text" name="City" value="Dallas"> </dd>
<dt> Area:</dt>
<dd><input type="text" name="Area" value="Downtown" disabled> </dd>
<dt> State:</dt>
<dd><input type="text" name="State" value="Texas" readonly> </dd>
<dt> Zip Code:</dt>
<dd><input type="text" name="Zip Code" size="5" maxlength="5"> </dd>
</dl>
<p><input type="submit" value="Submit form"></p>
</form>
</body>
</html>
```

### 17 - Text area
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Text area</title>
</head>
<body>
<form method="POST" action="http:localhost/echo.pl">
<textarea name="The Future Web" rows="10" cols="65">
HTML5 is a markup language used for structuring and presenting content on the World Wide Web. It is the fifth and final major HTML version that is a World Wide Web Consortium (W3C) recommendation. The current specification is known as the HTML Living Standard.
</textarea>
<p><input type="submit" value="Submit form"></p>
</form>
</body>
</html>
```

### 18 - Audio
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Audio</title>
</head>
<body>
<audio src="audio.ogg" autoplay>Fallback Message</audio>
<audio controls>
<source src="audio.mp3" type="audio/mpeg">
<source src="audio.ogg" type="audio/ogg">
[Fallback Message]
</audio>
</body>
</html>
```

### 19 - Video
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Video</title>
</head>
<body>
<video controls>
<source src="video.mp4" type="video/mpeg">
<source src="video.ogv" type="video/ogg">
[Fallback Message]
</video>
</body>
</html>
```

### 20 - Pdf
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Pdf</title>
</head>
<body>
<p>This is text in the main document that...<br>
<object type="application/pdf" data="piechart.pdf" width="580" height="310">
<strong> [PDF Document - Requires Adobe Reader Plugin] </strong>
</object>
<br>...continues around an embedded resource.</p>
</body>
</html>
```

### 21 - Animation
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Animation</title>
<link rel="stylesheet" href="Animation.css">
</head>
<body>
<div id="box-1"></div>
<div id="box-2"></div>
<div id="box-3"></div>
</body>
</html>
```

### 22 - Animation.css
```
div { position: absolute ; top: 10px ; height : 120px ; width : 120px ; border : 5px solid black }
div#box-1 { background : yellow ; left : 50px ; z-index : 1}
div#box-2 { background : lime ; left : 400px ; z-index : 1}
div#box-3 { background-color : aqua ; left : 50px ; border-radius : 65px ; Z-index :2}
@-ms-keyframes slide { from { left : 50px } to { left : 400px } }
@-moz-keyframes slide { from { left : 50px } to { left : 400px } }
@-webkit- keyframes slide { from { left : 50px } to { left : 400px } }
@-o-keyframes slide { from { left : 50px } to { left : 400px } }
@keyframes slide { from { left : 50px } to { left : 400px } }
div#box-3
{
-ms-animation : slide 3s alternate infinite ;
-moz-animation : slide 3s alternate infinite ;
-webkit-animation : slide 3s alternate infinite ;
-o-animation : slide 3s alternate infinite ;
animation : slide 3s alternate infinite ;
}
```

### 23 - Flex
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Animation</title>
<link rel="stylesheet" type="text/css" href="flex.css">
</head>
<body>
<div id="wrapper">
<div id="box-1">Flex=1</p></div>
<div id="box-2">Flex=2</p></div>
<div id="box-3">Flex=3</p></div>
</div>
</body>
</html>
```

### 24 - Flex.css
```
div#wrapper { height : 120px ; width: 95% ; border: 5px solid black ; text-align: center }
div#wrapper { display: -ms-flexbox ; display: -moz-box ; display: -webkit-box ; display: -o-flexbox; display: box; display: flexbox }
div#box-1 { background: yellow ; -ms-flex: 1; -moz-box-flex: 1 ; -webkit-box-flex: 1 ; -o-flex: 1; box-flex: 1; flex: 1 }
div#box-2 { background: lime ; -ms-flex: 2; -moz-box-flex: 2 ; -webkit-box-flex: 2 ; -o-flex: 2; box-flex: 2; flex: 2 }
div#box-3 { background: aqua ; -ms-flex: 3; -moz-box-flex: 3 ; -webkit-box-flex: 3 ; -o-flex: 3; box-flex: 3; flex: 3 }
```

# 25 - Grid
```
<!DOCTYPE HTML>
<html lang="en">
<head>
<style>
.grid-container {
display:grid;
grid-template-columns: auto auto auto auto;
gap: 10px;
background-color: lime;
padding: 10px;
}
.grid-container > div {
background-color: rgba(255, 255, 255, 0.8);
text-align: center;
padding: 20px 0;
font-size: 30px;
}
</style>
</head>
<body>
<h1>The grid-template-columns Property</h1>
<div class="grid-container">
<div>1</div>
<div>2</div>
<div>3</div>
<div>4</div>
<div>5</div>
<div>6</div>
<div>7</div>
<div>8</div>
</div>
</body>
</html>
```

# 26 - Inline Frame Example
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Inline Frame Example</title>
<link rel="stylesheet" href="iframe.css">
</head>
<body>
<article class="left220">
<h3>Concept Cars</h3>
<p>Many of the creative...</p>
</article>
<aside>
<iframe src="concept.html" width="300" height="200">
<strong>[Framed Document - Requires iframe Support]</strong>
</iframe>
</aside>
</body>
</html>
```

# 27 - iframe.css
```
p {font-family:sans-serif;}

article.left220 {width:220px; float:left; margin-right:20px;}

body.concept {width:1500px}
p.concept {width:300px; float:left; margin:0;}
```

# 28 - concept.html
```
<! DOCTYPE HTML>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>ConceptCars</title>
<link rel="stylesheet" href="iframe.css">
</head>
<body class="concept">
<p class="concept"><strong>1. Renault Dezir</strong><br>
<img src="dezir.jpg">
</p>
<p class="concept"><strong>2. Lamborghini Sesto Elemento</strong><br>
<img src="lambo.jpg">
</p>
<p class="concept"><strong>3. Jaguar C-X75</strong><br>
<img src="jaguar.jpg">
</p>
<p class="concept"><strong>4. Lotus Esprit</strong><br>
<img src="lotus.jpg">
</p>
<p class="concept"><strong>5. Audi Quattro</strong><br>
<img src="audi.jpg">
</p>
</body>
</html>
```

# 28 - 
```
