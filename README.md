<h1>Blur Menu</h1>

<h2>Introduction</h2>
<p>Ce petit tuto permet de faire un menu avec un style flou qui devient net au survole de la souris</p>
<p>Voici un exemple :</p>
![preview](https://raw.githubusercontent.com/snowpact/blur-menu/master/img/demo.png)

demo : https://jsfiddle.net/sabalotelli/3bm4dL7q/

<h2>Tuto</h2>

<h3>Création du menu HTML</h3>

	<div class="blur-menu">
		<h2><a href="#presentation">Présentation</a></h2>
		<h2><a href="#developpement">Développement</a></h2>
		<h2><a href="#illustrator">Illustrator</a></h2>
		<h2><a href="#photographie">Photographie</a></h2>
		<h2><a href="#contact">Contact</a></h2>
	</div>
	
<h3>Création du CSS</h3>

	.blur-menu a{
		-webkit-filter: blur(3px);
		-moz-filter: blur(3px);
		-ms-filter: blur(3px);
		-o-filter: blur(3px);
		filter: blur(3px);
		color: inherit;
		text-decoration: inherit;
		transition-duration: 0.5s;
	}

	.blur-menu a:hover{
		-webkit-filter: blur(0);
		-moz-filter: blur(0);
		-ms-filter: blur(0);
		-o-filter: blur(0);
		filter: blur(0);
		transition-duration: 0.5s;
	}
	
<h3>En bonus, le style du texte</h3>

	.blur-menu{
		text-align: right;
	}
	
	.blur-menu h2{
		color: white;
		font-family:"Roboto";
		font-weight: 100;
		text-transform: uppercase;
		letter-spacing: 15px;
		font-size: 50px;
		margin: 0;
		padding: 30px;
	}
	
<p>Vous pouvez rajouter la police Roboto de google directement en insérant la ligne suivante dans le head de votre fichier HTML :</p>
	
    <link href='http://fonts.googleapis.com/css?family=Roboto:100' rel='stylesheet' type='text/css'>
	
Fin du tuto :)


