# HTML & CSS

Cheat-sheet for HTML & CSS syntax.
For Markdown preview use ctrl + shift + v

**Meta tags**

Meta tags are needed for certain features of the web page.

```html
<head>
	<!-- Keyboard -->
	<meta charset="UTF-8">

	<!-- For responsive design -->
	<meta name="viewport" content="width=device-width, initial-scale=1.0">

	<!-- For browser compatibility -->
	<meta http-equiv="X-UA-Compatible" content="ie=edge">

	<!-- Description of the site - shown in the search engine -->
	<meta name="description" content="This is my web-site description">

	<!-- Keywords, around eight or so -->
	<meta name="keywords" content="web development, coding, web design">

	<!-- For not indexing on search engines -->
	<meta name="robots" content="NOINDEX, NOFOLLOW">

	<!-- CSS -->
	<link rel="stylesheet" href="./style.css">

	<!-- Fonts -->
	<link href="https://fonts.googleapis.com/css?family=Inter&display=swap" rel="stylesheet">

	<!-- Title is what is shown in the search engine -->
	<title>My web-site title</title>
</head>
```

**Most popular HTML5 tags**

There are plenty of them, but these are the most used ones.

```html
<header>

<nav>

<main>

<section>

<article>

<aside>

<footer>

<!-- Other useful tags -->

<p>

<span>

<em>

<strong>

<br>

<ol><li>

<ul><li>

<!-- Images -->
<img scr="img/image.png" alt="My Image">
<img scr="https://source.unsplash.com/200x200/?surf" alt="My Image">

<!-- Links -->
<a href="digitalcollars.com" target="_blank">Go to my webpage</a>
<a href="/about.html">About</a>

<video scr="youtube.com">

```

**CSS**

```html
<style>

	/* . is for classes */
	.primary-heading{
		color: blue;
		font-size: 20px;
	}

	/* # is for IDs */
	#welcome, #about{
		background-color: white;

		<!-- Margin is the space outside of the border -->
		margin: 5px;

		<!-- Padding is the space inside of the border -->
		padding: 10px;

		<!-- Shorthand = top, right, bottom, left -->
		<!-- Shorthand = top/bottom, left/right -->
	}

	/* Fonts */
	body{
		background-image: url('./img/background.jpg')
		color: #fff;
		height: 300px;
		width: 600px;
	}

	/* Backgrounds */
	body{
		font-family: 'Inter', sans-serif;
		font-size: 18x;
	}	

	/* Borders */
	#box{
		background-color: white;
		border: 3px solid red;
		border-radius: 10px;
	}

	/* Buttons */
	.btn{
		background: blue;
		color: white;
		border: none;
		font-size: 10px;
		padding: 10px 20px;
		border-radius: 5px;
		cursor: pointer;
	}

	.btn:hover{
		background: green;
		color: grey;
	}

</style>
```

**Responsive design**

1. Media queries

```html
<style>

	/* CSS applied as long as screen width is smaller than 500px */
	@media(max-width: 500px){

		body{
			background: red;
		}

		#smartphone h1{
			display: block;
		}
	}

	/* Tablets */
	@media(min-width: 501px) and (max-width: 768px){
		#tablet h1{
			display: block;
		}
	}

	/* rem units - root element is always 16px */
	#box{
		font-size: 2rem;
	}

	/* Changing root element */
	html{
		font-size: 10px;
	}

</style>
```

2. View-ports

```html
<style>
	header{
		background: url('https://source.unsplash.com/daily') no-repeat center center/cover;
		color: white;
		height: 100vh;
		text-align: center;
	}
</style>
```

**Flexbox**

```html
<style>

	.container{
		/* Flex creates a "flex container" and all direct child elements are "flex items" */
		display: flex; 

		/* Create a column of four items */
		flex-direction: column;

		/* Do not add horizontal scroll. Put items in the following lines */
		flex-wrap: wrap;

		/* Align items horizontally */
		justify-content: space-evenly;

		/* Align items vertically, but there must be a height */
		align-items: center;
	}

	.item{
		/* Make all the items equals in width */
		flex: 1;
	}

	.item:first-child{
		/* Make the Item 1 bigger */
		flex: 3;

		/* Place the Item 1 in the fourth position */
		order: 4;
	}

</style>

<body>
	<div class="container">
		<div class="item">Item 1</div>
		<div class="item">Item 2</div>
		<div class="item">Item 3</div>
		<div class="item">Item 4</div>
	</div>
</body>
```

**VSCode shortcuts**

- Copy entire line up/down: Shift + Alt + Arrows
- Move entire line up/down: Alt + Arrows
- Move word by word: Ctrl + Arrows
- Comment entire line: Ctrl + Shift + /
