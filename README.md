# HTML-Website, User Brackets to function
<DOCTYPE html>
	<html>
	<head>
		<title>Peace for all</title>
		<style>
			*{
				font-family: fantasy;
				font-weight: 300;
			}
			body,ul,li{
				margin: 0;
				padding: 0;
			}
			p,li,h1,h2,h3,h4{
			  color: black;
			}
			body{
				background-color: lightblue;
			}
			.wrapper{
				width: 96%;
				max-width: 1200px;
				margin: 0 auto;
				padding: 0 2%;
			}
			header{
				background-color: darkblue;
				padding: 10px 0;
			}
			.logo{
				margin: 0;
				background: url(Mental%20health%20website%20logo.jpg);
				background-size: 70px 70px;
				float: left;
				width: 70px;
				height: 70px;
			}
			header nav{
				float: right;
			}
			header:after {
				content: "";
				clear: both;
				display: block;
			}
			header nav li {
				list-style-type: none;
				float: left;
				margin-left: 20px;
				margin-top: 20px;
			}
			header nav li a{
				text-decoration: none;
				color: white;
				font-size: 15px;
				text-transform: uppercase;
			}
			#main-banner {
				width: 100%;
				max-height: 2000;
				overflow: hidden;
				
			}
			#main-banner img {
				width: 100%;
			}
			#slider {
				overflow: hidden;
			}
			#slides {
				position: relative;
				width: 500%;
				margin: 0;
				left: 0;
				text-align: left;
				font-size: 0;
				animation: 18s slidy infinite;
			}
			#slides img {
				width: 20%;
				float: left;
			}
			#usp {
				margin-top: 60px;
			}
			#usp li{
				float: left;
				width: 23%;
				padding: 1%;
				text-align: center;
				list-style-type: none;
			}
			#usp li img {
				height: 80px;
				padding: 20px;
				background-color: red;
				border-radius: 50%;
			}
			#usp li h2{
				font-size: 16px;
				font-weight: 400;
			}
			#usp:after {
				content: "";
				display: block;
				clear: both;
				
			}
			#products{
				padding-top: 30px;
				margin-top: 30px;
				border-top: 2px solid lightgrey;
			}
			#products li{
				float: left;
				width: 32%;
                list-style-type: none;
				text-align: center;
			}
			#products li img {
				width: 100%;
			}
			#products li:nth-child(even) {
				margin: 0 1%;
			}
			#products:after {
				content: "";
				display: block;
				clear: both;
			}
			#our products {
				text-align: center;
			}
			footer {
				width: 100%;
				background-color: blueviolet;
				padding: 30px 0;
				margin-top: 60px;
			}
			footer ul {
				float: left;
				width: 48%;
				margin-top: 1%;
			}
			footer ul h3{
				font-size: 30px;
				color: aqua;
			}
			footer ul li {
				list-style-type: none;
				font-size: 15px;
				color: white;
			}
			footer :after {
				content: "";
				display: inline-flex;
				clear: both;
			}
			/*Animation*/
			@keyframes slidy {
				0% { left: 0%; }
				28% { left: 0%; }
				33% { left: -100%; }
				61% { left: -100%; }
				66% { left: -200%; }
				94% { left: -200%; }
				100% { left: 0%; }
			}
			
           .greet{
                background-color: #48C9B0;
                font-family: fantasy;
                font-size: 20px;
                color: white;
                padding-top: 50px;
                padding-bottom: 50px;
                text-align: center;
                
                
            }
		</style>
	</head>
	<body>
	   <header>
		 <div class="wrapper">
		    <div class="logo"></div>
			 <nav>
			     <ul>
				   <li><a href="#">Home</a></li>
				   <li><a href="#">About us</a></li>
				   <li><a href="#">Products</a></li>
				   <li><a href="#">Contact us</a></li>
					 
				 </ul>
			 </nav>
		   </div>
		</header>
		
		
		<!-- Greet section Starts-->
        <div class="greet">
        <p id="namesec" ></p>   
            </div>
		
		
		<div id="main-banner">
		   <div id="slider">
			<div id="slides">
			   <img src="IMG_20201219_202155.jpg"alt="banner">
				<img src="bannner.jpg" alt="banner">
				<img src="HJHJHJHJHJHJHJHJHJHJH.jpg" alt="banner">
				
			   </div>
			</div>
		</div>
	
		<div class="wrapper">
		   <section id="products">
			   <h2 id="our-products">Food for thought</h2>
			   <ul>
			       <li>
				  <img src="CamScanner%2012-19-2020%2021.33.jpg">
					   <h2>I wonder poem</h2>
					   <p>This is our creative attempt to draw attention towards the differential treatment of mental diseases due to societal stigma, false notions or unjustified opinions. </p>
				   </li>
				   <li>
				     <img src="Spiritual%20wealth.jpg">
					  <h2>Spiritual wealth poster</h2> 
					   <p>This poster is a creative endevor that brings to limelight the importantance of mind body balance for living a healthy lifestyle.</p>
				   </li>
				   <li>
				     <img src="Online%20being.jpg"
					   <h2>Online being poster</h2>
					   <p>This poster attempts to visually depict the ill effects of too much screen time on our mental well being.</p>
				   </li>
			   </ul>
			</section>
		</div>
		<footer>
		    <div class="wrapper">
			   <ul>
				  <h3>Get in touch</h3>
				  <li>Well being for all-Pthways school noida(MYP)</li>
				   <li>Contributors: Aaryaman, saksham, Avyakt, Ridhaan</li>
				</ul>
			</div>
		</footer>
		
		
		<script>
			
			
		 function myFunction(){
            var name=prompt("Hello user, What is your name?","doe");
            var msg;
            var date= new Date();
            var hour=date.getHours();
            
            if (hour<12){
                msg="Hello "+name+" Good Morning";
                document.getElementById("namesec").innerHTML=msg;

            }
            else if (hour>12 && hour<16){
                msg="Hello "+name+" Good Afternoon";
                document.getElementById("namesec").innerHTML=msg;
            }
            else if(hour>16 && hour<23){
                msg="Hello "+name+" Good Evening";
                document.getElementById("namesec").innerHTML=msg;
            }
            else{
                msg="greetings of the day";
                document.getElementById("namesec").innerHTML=msg;

            }
			 
              document.body.style.backgroundColor=bg;   
			 
        }
				
		</script>
	</body>
</html>

