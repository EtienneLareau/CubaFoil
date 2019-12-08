<script>
	export let segment;
	let logo = 'images/supatitle.png';

	// function readMenu() {
	// 	var el = document.getElementById('open');
	// 	if (el.className === 'openMenu'){
	// 		el.className = ' ';
	// 	} else {
	// 		el.className = 'openMenu';
	// 	}
	// }
	// console.log(readMenu);

	/// Function for opening and closing the menu bar ///
	// function openNav() {
  	// 	document.getElementById("Nav").style.width="100%";
	// 	document.getElementById("Nav").style.opacity="1";
	// 	document.getElementById("Nav").style.display="inherit";		 
	// }

	// function closeNav() {
  	// 	document.getElementById("Nav").style.width="0%";
	// 	  document.getElementById("Nav").style.opacity="0";
	// 	  document.getElementById("Nav").style.display="none";	  
	// }


	/// Function for sub menu and rotating arrow Simon ///
// function openSubSim() {
// 	document.getElementById("openSubSim").style.height="210px";
// 	document.getElementById("arrowChirSim").style.color="#f49a6d";
	
// 	var el = document.getElementById("arrowChirSim");
//   	el.classList.remove("rotatingArrowTop");

// 	var element, name, arr;
// 	element = document.getElementById("arrowChirSim");
// 	name = "rotatingArrow";
// 	arr = element.className.split(" ");
// 	if (arr.indexOf(name) == -1) {
// 	  element.className += " " + name;
// 	}
// }

// function openTopSim() {
// 	document.getElementById("openSubSim").style.height="0px";
// 	document.getElementById("arrowChirSim").style.color="#18385f";
	
// 	var el = document.getElementById("arrowChirSim");
//   	el.classList.remove("rotatingArrow");

// 	var element, name, arr;
// 	element = document.getElementById("arrowChirSim");
// 	name = "rotatingArrowTop";
// 	arr = element.className.split(" ");
// 	if (arr.indexOf(name) == -1) {
// 	  element.className += " " + name;
// 	}
// }
///////////////////////////////////////////////////////

// SmoothScroll

    function scrollDown() {
        document.querySelector('#Register').scrollIntoView({ 
        behavior: 'smooth' });
    }

</script>

<style>
	
	/* clearfix */
	/* ul::after {
		content: '';
		display: block;
		clear: both;
	} */
/* 
	.selected {
		position: relative;
		display: inline-block;
	}

	.selected::after {
		position: absolute;
		content: '';
		width: calc(100% - 2em);
		
		
		height: 5px;
		background-color: rgb(255, 74, 104);
		display: block;
		bottom: -1px;
	} */
/* 

	/* a:hover {
		color:pink;
	} */

	/* .ul-center {
		
		top:50%;
		position: relative;
		transform: translate(0,-50%);
		list-style-type: none;
	} */

	/* .vert { list-style-type: none;
			margin: 0 0 30px 0;
			text-align: center; }


	.menu {
		position: relative;
		float: right;
		z-index:2010;
		padding:30px;
		cursor: pointer;
	} */

	/* .bars { width:3em;
			height:4px;
			margin-bottom:6px;
			background: #ff22aa;
	}

	

	#Nav {  position: fixed;
			display:none;
			margin:0;
			padding:0;
			z-index: 2200;
			top:0;
			left:0;
			width:0%;
			height:100%;
			background: #86fadb;
			opacity:1;
			transition: all 0.15s ease-out, width 0s; } */

	/* .close-Btn {
		position: absolute;
		right:0;
		top:0;
		z-index: 5500;
		color:rgb(134, 126, 126);
		background: #86fadb;
		font-size: 3em;
		padding:18px 30px;
		text-align:right;
		font-family: 'battlefin', sans-serif;
        font-weight: 700;
		font-style: normal;
		text-decoration: none;
	} */

	img {
		position: absolute;
		width:200px;
		top:24px;
		left:30px;
		z-index: 7000;
	}

	.rolldown {
		position: relative;
		float: right;
		z-index:2010;
		padding:2px 20px;
		cursor: pointer;
		
	}

	p {
		color:white;
		border-radius: 10px;
		background: #ff22aa;
		padding: 10px 30px;
		font-size:1.5rem;
		transition: all 0.25s ease;
		font-family: bicyclette, sans-serif;
		font-weight: 400;
		font-style: normal;
	}

	p:focus, p:hover {
		color:#ff22aa;
		background: #86fadb;
	}

	.fly { display:none }

	@media only screen and (max-width:725px){
		.fly {
		display: block;
		width:30px;
		position: relative;
		padding:0;
		margin-right:40px;
		}
		.regEx { display:none; }
		img { width:125px; }
	}

</style>

<!-- Register Menu -->
	<!-- <a class="rolldown" href="#Register">
		<p class="regEx">Inscrivez-vous</p>
		<img class="fly" src="/images/flywithus.png" alt="">
	</a> -->
	<div class="rolldown" on:click={scrollDown}>
		<p class="regEx">Inscrivez-vous</p>
		<img class="fly" src="/images/flywithus.png" alt="">
	</div>
 <!-- ************* -->



<!-- hamburger menu -->
	<!-- <div class="menu" on:click={openNav}>
		<div class="bars first"></div>
		<div class="bars second"></div>
		<div class="bars third"></div>
	</div> -->
 <!-- ************* -->

<img src="/images/supatitle2.png" alt="Logo KiteTrips.ca">
	
	<!-- <div id="Nav">

		<ul class="ul-center">	
			<li class="vert"><a class='{segment === undefined ? "selected" : ""}' href='.' on:click={closeNav}>Accueil</a></li>
			<li class="vert"><a class='{segment === "about" ? "selected" : ""}' href='about' on:click={closeNav}>Services</a></li>
			
				for the blog link, we're using rel=prefetch so that Sapper prefetches
				the blog data when we hover over the link or tap it on a touchscreen 
			<li class="vert"><a rel=prefetch class='{segment === "blog" ? "selected" : ""}' href='blog' on:click={closeNav}>Cours</a></li>
			<li class="vert"><a class='{segment === "contact" ? "selected" : ""}' href='contact' on:click={closeNav}>Contactez-nous</a></li>
		</ul>
		<a href="javascript:void(0)" class="close-Btn" on:click={closeNav}>X</a>
	</div> -->