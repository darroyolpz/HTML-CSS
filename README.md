# HTML & CSS

Cheat-sheet for HTML & CSS syntax.

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

	<!-- Description of the site -->
	<meta name="description" content="This is my web-site description">

	<!-- Keywords -->
	<meta name="keywords" content="web development, coding, web design">

	<!-- For not indexing -->
	<meta name="robots" content="NOINDEX, NOFOLLOW">

	<!-- CSS -->
	<link rel="stylesheet" href="/style.css">

	<!-- Fonts -->
	<link href="https://fonts.googleapis.com/css?family=Roboto" rel="stylesheet">

	<!-- Title-->
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
	}

	body{
		font-family: 'Roboto', sans-serif;
	}

</style>
```

**Responsive design**

Media queries

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

</style>
```

View-ports

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