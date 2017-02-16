<html>
<head>
	<meta charset="utf-8">
	<link href="https://fonts.googleapis.com/css?family=Questrial" rel="stylesheet">
	<link href="https://fonts.googleapis.com/css?family=Prompt" rel="stylesheet">
	<link rel="stylesheet" type="text/css" href="reset.css">
	<title>Currency Calculator</title>
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

	<style type="text/css">
@media screen and (min-width: 749px){
	
	body{
		width: 100%;
		height: 98%;
		background-image: linear-gradient(to top, #f3e7e9 0%, #e3eeff 99%, #e3eeff 100%);
		font-family: 'Questrial';
		position: relative;
		
	}
	
	.content{
		width: 100%;
		height: 100%;
	}
	
	.box-con{
		width:90%;
		height: 80%;
		font-size: 2em;
		text-align: center;
		border-radius: 50px;
		border: 8px solid #fff;
		background: #fff;
		margin: 0 auto;
	}
	.con-in{
		width: 85%;
		height: 100%;
		margin: 0 auto;
	}
	.boxbutton{
		width: 75%;
		height: 8%;
		margin: 0 auto;
		margin-top: 6%;
	}
	.cal{
		width: 40%;
		height: 70%;
		font-size: 3em;
		text-align: center;
		border-radius: 50px;
		background-color: #a9ef88;
		margin-left: 30%;
		-webkit-box-shadow: 13px 10px 63px -17px rgba(0,0,0,0.45);
		-moz-box-shadow: 13px 10px 63px -17px rgba(0,0,0,0.45);
		box-shadow: 13px 10px 63px -17px rgba(0,0,0,0.45);
		color: #fff;
		cursor: pointer;
	}
	
	.gear{
		background-image: url('gear1_s.png');
		width: 300px;
		height: 300px;
		position: absolute;
		
	}
	.gear2{
		background-image: url('gear1_a.png');
		width: 300px;
		height: 300px;
	}
	h3{
		font-size: 2em;
		text-align: center;
		height: 6%;
		padding-top: 3%;
		border-bottom: 2px solid #CCC;
		color: #696969;
	}
	h4{
		font-size: 3em;
		text-align: center;
		height: 8%;
		padding-top: 3%;
		color: #696969;
	}
	h1{
		font-size: 1.2em;
		height: 6%;
		padding-top: 10%;
		padding-bottom: 4%;
		border-bottom: 2px solid #CCC;
		color: #696969;
	}
	h2{
		font-size: 1.2em;
		height: 6%;
		padding-top: 3%;
		padding-left: 8%;
		color: #696969;
		text-align: left;
	}
	.credit{
		height: 5%;
		width: 100%;
		text-align: center;
		font-size: 2em;
		color: #ccc;
		margin-top: 2%;
	}
	.space{
		height: 3%;
		width:100%;
	}
	.flied{
		height: 80%;
		width: 68%;
		border-radius: 50px;
		border: 1px solid #696969;
		font-size: 1.2em;
	}
	.chack{
		height: 70%;
		width: 5%;
		margin-left: 5%;
	}
	.unpaddingleft{
		margin-left: 0.5%;
	}
	.underline{
		border-bottom: 2px solid #CCC;
	}
	.piccal{
		height: 35%;
		width: 100%;
	}
	.wrapper{
		width: 100%;
		height: 100%;
	}
}	

	@media screen and (min-width: 1024px){
		.wrapper{
		width: 600px;
		height: 100%;
		margin: 0 auto;
	}	.box-con{font-size: 0.8em}
		.credit{font-size: 1em}
		.cal{
			font-size: 1.5em;
		}
		h2{
			padding-top: 7px;
		}
		
	}

	</style>

</head>

<body>	
	<div class="wrapper">
			<DIV class="space"></DIV>
			
				<div class="box-con">
					<div class="con-in">
						
					
						<h3>Currency Calculator</h3>
						<form method='post' action='index.php'>
							<h1>VALUE : <input type="number" name="valueNum" class="flied"></h1>
							
							  	<h2>FROM : &nbsp;<input type="radio" name="F" value="FTH" class="chack unpaddingleft"> &nbsp;Thai Baht (THB)<br></h2>
							  	<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<input type="radio" name="F" value="FUS" class="chack"> &nbsp;U.S. Dollar (USD) <br></h2>
							  	<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<input type="radio" name="F" value="FJP" class="chack "> &nbsp;Japanse Yen (JPY) <br></h2>
								<h2 class="underline">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<input type="radio" name="F" value="FKR" class="chack "> &nbsp;Sounth Korean Won (KRW) <br></h2>
							
							  	<h2>TO&nbsp;&nbsp;&nbsp;&nbsp;:<input type="radio" name="T" value="TTH" class="chack"> &nbsp;Thai Baht (THB)<br></h2>
							  	<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<input type="radio" name="T" value="TUS" class="chack"> &nbsp;U.S. Dollar (USD) <br></h2>
							  	<h2>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<input type="radio" name="T" value="TJP" class="chack "> &nbsp;Japanse Yen (JPY) <br></h2>
								<h2 class="underline">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<input type="radio" name="T" value="TKR" class="chack "> &nbsp;Sounth Korean Won (KRW) <br></h2>
							
							<?php 
								if(isset($_POST['submit']))
							{
								$value = $_POST['valueNum'];
								$MAIN = $_POST['F'];
								$CAL = $_POST['T'];
								if($MAIN=="FTH"){
									$Mcurren = 'THB';
									if($CAL=="TTH"){
										$answer = $value*1;
										$curren = 'THB';
									}
									if($CAL=="TUS"){
										$answer = $value*0.034;
										$curren = 'USD';
									}
									if($CAL=="TJP"){
										$answer = $value*3.26;
										$curren = 'JPY';
									}
									if($CAL=="TKR"){
										$answer = $value*30.7;
										$curren = 'KRW';
									}
								}
								if($MAIN=="FUS"){
									$Mcurren = 'USD';
									if($CAL=="TTH"){
										$answer = $value*34.75;
										$curren = 'THB';
									}
									if($CAL=="TUS"){
										$answer = $value*1;
										$curren = 'USD';
									}
									if($CAL=="TJP"){
										$answer = $value*113.85;
										$curren = 'JPY';
									}
									if($CAL=="TKR"){
										$answer = $value*1141;
										$curren = 'KRW';
									}
								}
								if($MAIN=="FJP"){
									$Mcurren = 'JPY';
									if($CAL=="TTH"){
										$answer = $value*0.30;
										$curren = 'THB';
									}
									if($CAL=="TUS"){
										$answer = $value*0.09;
										$curren = 'USD';
									}
									if($CAL=="TJP"){
										$answer = $value*1;
										$curren = 'JPY';
									}
									if($CAL=="TKR"){
										$answer = $value*10;
										$curren = 'KRW';
									}
								}
								if($MAIN=="FKR"){
									$Mcurren = 'KRW';
									if($CAL=="TTH"){
										$answer = $value*0.30;
										$curren = 'THB';
									}
									if($CAL=="TUS"){
										$answer = $value*0.001;
										$curren = 'USD';
									}
									if($CAL=="TJP"){
										$answer = $value*0.1;
										$curren = 'JPY';
									}
									if($CAL=="TKR"){
										$answer = $value*1;
										$curren = 'KRW';
									}
								}


							 ?>
							<h2><?php echo $value ;?> <?php echo $Mcurren ;?> =</h2> 
							<h4><?php echo $answer ;?> <?php echo $curren ; ?></h4> 
							<?php 
							}
							?>
						</div>
					</div>
					
					 <div class="boxbutton">
					 	<input type="submit" name="submit" value="Calculate"class="cal">
					 </div>
			 </form>
			 <div class="credit">By Patimakorn & For education Only</div>
			

		 </div>
</body>
</html>
