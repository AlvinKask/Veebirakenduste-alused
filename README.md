www.w3schools.com

[04.11.2022.zip](https://github.com/AlvinKask/Arvutivorkude-alused/files/9937815/04.11.2022.zip)

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

# 5 - box.css
```
p	{ background : yellow; width : 20em }
p.pad	{ padding : 1em }
p.bdr	{ border : 0.5em red solid }
p.mgn	{ margin : 2em }
```

# 6 - Taust 1
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

# 7 - background.css
![tile](https://user-images.githubusercontent.com/115221752/199756486-98a255b4-32f0-44bc-a8ac-9092f3506728.png)

```
span	{ background : yellow; margin : 0 0 0 10em }
p	{ background : url(tile.png) fuchsia repeat ; height : 3.5em }
p#x	{ background-repeat : repeat-x }
p#y	{ background-repeat : repeat-y }
p#no	{ background-repeat : no-repeat }
```

# 8 - Taust 2
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

# 9 - background2.css
![flower](https://user-images.githubusercontent.com/115221752/199756536-9c0a08c1-57c4-4067-9329-ecc2aeb7c829.png)

```
div { float : left ; margin : 10px ; height : 120px ; width : 120px ; border: 5px solid black ; background : url(flower.png) ; }
div#box-1	{ background-size : 100% 100% }
div#box-2	{ background-size : 50% 50% }
div#box-3	{ background-size : 200% 200% }
```

# 10 - Kodulehe alge
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

# 11 - columns.css
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
