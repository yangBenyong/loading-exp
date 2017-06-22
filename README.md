# loading-exp

<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-7">
		<title>medo11</title>
<style type="text/css">
	* {
	    padding:0px;margin:0px;box-sizing:border-box;
	}
	.box{
		transform-style: preserve-3d;
		transform:perspective(700px) rotateX(0deg);
		width: 200px;height:200px;
		line-height: 200px;
		float: left;
		border:1px solid red ;
		position: relative;
	}
	.box:first-of-type >div{background: #10BF0B;
		width: 10px;height: 10px;float: left;
		margin-left: 10px;opacity: 0;margin-top: 50%;
	}
	.box:first-of-type >div:first-child{
		animation: opt 1s ease 0s infinite;
	}
	.box:first-of-type > div:nth-child(2){
		animation: opt 1s ease 0.2s infinite;
	}
	.box:first-of-type > div:nth-child(3){
		animation: opt 1s ease 0.4s infinite;
	}
	.box:first-of-type > div:nth-child(4){
		animation: opt 1s ease 0.6s infinite;
	}
	.box:first-of-type > div:last-child{
		animation: opt 1s ease 0.8s infinite;
	}			
	@keyframes opt{
		0%{opacity: 0; transform: scale(2);}
		50%{opacity: 1;}
		100%{opacity: 0; transform: scale(0);}
	}
	.box:nth-of-type(2) > div{margin-top: 50%;
		width: 200px;height:10px;background: green;overflow: hidden;
	}
	.box:nth-of-type(2) > div>div{
		width: 200px;height:20px;background: blue;
		animation: move 3s linear 0s infinite;
	}			
	@keyframes move{
		from{transform: translateX(-200px);}
		to{transform: translateX(200px);}
	}

	.box:nth-of-type(3) >div{		
		background: forestgreen;
		width: 20px;height: 40px;
		position: absolute;
		opacity: 0;border-radius: 10px 10px 0 0;
		transform-style: preserve-3d;
		margin: auto;
	}
	.box:nth-of-type(3) >div:first-child{
		top: 0px;
		left: 50px;
		transform:rotate(0deg);
		animation: opt3 1s ease 0.1s infinite;
	}
	.box:nth-of-type(3) > div:nth-child(2){
		left:15px;
		top:15px;
		transform:rotate(-45deg);
		animation: opt3 1s ease 0.2s infinite;
	}
	.box:nth-of-type(3) > div:nth-child(3){
	left: 0px;
	top: 50px;
		transform:rotate(-90deg);
		animation: opt3 1s ease 0.3s infinite;
	}
	.box:nth-of-type(3) > div:nth-child(4){
		left: 15px;
		top: 90px;
		transform:rotate(-135deg);
		animation: opt3 1s ease 0.4s infinite;
	}
	.box:nth-of-type(3) > div:nth-child(5){
	left: 50px;
	top:100px;
		transform:rotate(-180deg);
		animation: opt3 1s ease 0.5s infinite;
	}
	.box:nth-of-type(3) > div:nth-child(6){
	left: 85px;
	top:85px;
		transform:rotate(-225deg);
		animation: opt3 1s ease 0.6s infinite;
	}
	.box:nth-of-type(3) > div:nth-child(7){
	left: 100px;
	top:50px;
		transform:rotate(-270deg);
		animation: opt3 1s ease 0.7s infinite;
	}
	.box:nth-of-type(3) > div:last-child{
	left: 85px;
	top:15px;
		transform:rotate(-315deg);
		animation: opt3 1s ease 0.8s infinite;
	}
	@keyframes opt3{
		0%{opacity: 0;}
		50%{opacity: 1;}
		100%{opacity: 0;}
	}
	.box:nth-of-type(4) >div{
		background: #10BF0B;
		width: 20px;height: 20px;border-radius:10px;float: left;margin-left: 10px;opacity: 0;
	}
	.box:nth-of-type(4) >div:first-child{
		animation: opt3 1s ease 0.1s infinite;
	}
	.box:nth-of-type(4) > div:nth-child(2){
		animation: opt3 1s ease 0.2s infinite;
	}
	.box:nth-of-type(4)> div:nth-child(3){
		animation: opt3 1s ease 0.3s infinite;
	}
	.box:nth-of-type(4) > div:nth-child(4){
		animation: opt3 1s ease 0.4s infinite;
	}
	.box:nth-of-type(4) > div:last-child{
		animation: opt3 1s ease 0.5s infinite;
	}
	.box:nth-of-type(5)>div{
		position: absolute;left: 10px;top:25px;
		width: 10px;height: 30px;border-radius: 5px;background: #10BF0B;
		animation: my 1s linear 0.1s infinite alternate-reverse;
	}
	.box:nth-of-type(5) >div:nth-child(2){
		left:30px;animation: my 1s linear 0.2s infinite alternate-reverse;
	}
	.box:nth-of-type(5) >div:nth-child(3){
		left:50px;animation: my 1s linear 0.3s infinite alternate-reverse;
	}
	.box:nth-of-type(5) >div:nth-child(4){
		left:70px;animation: my 1s linear 0.4s infinite alternate-reverse;
	}
	.box:nth-of-type(5) >div:last-child{
		left:90px;animation: my 1s linear 0.5s infinite alternate-reverse;
	}
	@keyframes my{
		0%{height: 30px;top: 25px;}
		80%{background: #00FFFF}
		100%{height: 80px;top: 0px;}
	}
	.box:nth-of-type(6) >div{background: #10BF0B;
		width: 20px;height: 20px;float: left;margin-left: 10px;opacity: 0;
	}
	.box:nth-of-type(6) >div:first-child{
		animation: opt6 1s ease 0.1s infinite;
	}
	.box:nth-of-type(6) > div:nth-child(2){
		animation: opt6 1s ease 0.2s infinite;
	}
	.box:nth-of-type(6) > div:nth-child(3){
		animation: opt6 1s ease 0.3s infinite;
	}
	.box:nth-of-type(6) > div:nth-child(4){
		animation: opt6 1s ease 0.4s infinite;
	}
	.box:nth-of-type(6) > div:last-child{
		animation: opt6 1s ease 0.5s infinite;
	}
	@keyframes opt6{
		0%{opacity: 0;transform: rotate(0deg);}
		50%{opacity: 1;}
		100%{opacity: 0;transform: rotate(90deg);}
	}
	.box:nth-of-type(7)>div{
		width: 20px;height: 20px;
		background: black;
		border-radius: 50%;
		position: absolute;
		top: 50%;left: 50%;
		margin: 40px 0 0 -10px;
		transform-origin: 50% -50px;		
	}
	.box:nth-of-type(7)>div:first-child{
		animation: name 2s linear 0s infinite;
	}
	.box:nth-of-type(7)>div:nth-child(2){
		animation: name 2s linear .2s infinite;
	}
	.box:nth-of-type(7)>div:nth-child(3){
		animation: name 2s linear .4s infinite;
	}
	.box:nth-of-type(7)>div:last-child{
		animation: name 2s linear .6s infinite;
	}
	@keyframes name{
		0%{transform:rotate(0deg);animation-timing-function:linear;}			
		10%{transform:rotate(90deg);
			animation-timing-function:cubic-bezier(.28,.49,0,0.14);
			}
		50%{
			transform:rotate(180deg);animation-timing-function:cubic-bezier(.18,.29,0,1.14);opacity: 1;
		}
		100%{
			transform:rotate(360deg);opacity: 0;
		}
	}
	.range{
		position: absolute;top: 50%;left: 50%;margin: -5px 0 0 -100px;
		transform-style: preserve-3d;transform:perspective(800px) rotateX(0deg);
		width: 200px;height: 5px;
		background: #10BF0B;
		border-radius: 10px;
		animation: color 1s linear 0.5s infinite;
	}
	.range > div{
		width: 15px;height: 15px;border-radius: 50%;background: #10BF0B;
		position: absolute;left: 0px;top: -6px;animation: goto 1s linear .5s infinite alternate-reverse;
	}
	@keyframes goto{
		0%{left: 1px;}
		50%{background: #197FEE;}
		100%{left: 185px;background: #197FEE;}
	}
	@keyframes color{
		0%{background: #10BF0B;}
		50%{background: #197FEE;}
		100%{background: #197FEE;}
	}
	.box:nth-of-type(9) >div{
		background: #10BF0B;opacity: 0;margin-top: calc(50% - 20px);
		width: 20px;height: 20px;float: left;margin-left: 10px;				
	}
	.box:nth-of-type(9) >div:first-child{
		animation: opt3 1s ease 0.1s infinite;
	}
	.box:nth-of-type(9) > div:nth-child(2){
		animation: opt3 1s ease 0.2s infinite;
	}
	.box:nth-of-type(9) > div:nth-child(3){
		animation: opt3 1s ease 0.3s infinite;
	}
	.box:nth-of-type(9) > div:nth-child(4){
		animation: opt3 1s ease 0.4s infinite;
	}
	.box:nth-of-type(9) > div:last-child{
		animation: opt3 1s ease 0.5s infinite;
	}
	.box:nth-of-type(10) >div{background: forestgreen;
		width: 20px;height: 20px;position: absolute;left: 50px;top: 40px;
		opacity: 0;border-radius: 50px;
		transform-origin: 50px 50px;
	}
	.box:nth-of-type(10) >div:first-child{
		transform:rotate(0deg);
		animation: opt3 1s ease 0.1s infinite;
	}
	.box:nth-of-type(10) > div:nth-child(2){
		transform:rotate(-45deg);
		animation: opt3 1s ease 0.2s infinite;
	}
	.box:nth-of-type(10) > div:nth-child(3){
		transform:rotate(-90deg);
		animation: opt3 1s ease 0.3s infinite;
	}
	.box:nth-of-type(10) > div:nth-child(4){
		transform:rotate(-135deg);
		animation: opt3 1s ease 0.4s infinite;
	}
	.box:nth-of-type(10) > div:nth-child(5){
		transform:rotate(-180deg);
		animation: opt3 1s ease 0.5s infinite;
	}
	.box:nth-of-type(10) > div:nth-child(6){
		transform:rotate(-225deg);
		animation: opt3 1s ease 0.6s infinite;
	}
	.box:nth-of-type(10) > div:nth-child(7){
		transform:rotate(-270deg);
		animation: opt3 1s ease 0.7s infinite;
	}
	.box:nth-of-type(10) > div:last-child{
		transform:rotate(-315deg);
		animation: opt3 1s ease 0.8s infinite;
	}
	.box:nth-of-type(11)>div{
		position: absolute;left: 10px;bottom:0px;
		width: 10px;height: 50px;border-radius: 5px;background: #10BF0B;animation: my .5s linear 0.1s infinite alternate-reverse;
	}
	.box:nth-of-type(11) >div:first-child{
		left:10px;animation: my1 .5s linear 0.1s infinite alternate-reverse;
	}
	.box:nth-of-type(11) >div:nth-child(2){
		left:30px;animation: my1 .5s linear 0.2s infinite alternate-reverse;
	}
	.box:nth-of-type(11) >div:nth-child(3){
		left:50px;animation: my1 .5s linear 0.3s infinite alternate-reverse;
	}
	.box:nth-of-type(11) >div:nth-child(4){
		left:70px;animation: my1 .5s linear 0.4s infinite alternate-reverse;
	}
	.box:nth-of-type(11) >div:last-child{
		left:90px;animation: my1 .5s linear 0.5s infinite alternate-reverse;
	}
	@keyframes my1{
		0%{height: 50px;}
		80%{background: #00FFFF}
		100%{height: 80px;}
	}
	.tab{
		position: absolute;top:calc(50% - 50px);left:calc(50% - 50px);
		width: 100px;height:100px;background: rgba(0,0,0,0);
		border-radius: 50px;
		border-width: 2px;
		border-style: solid;
		border-color: #008FD0 ;
		/*animation: colo 1s linear 0s infinite;*/
		box-sizing: content-box;
	}
	.tab > div{
		width:20px;height: 20px;background: #008FD0;border-radius: 50%;
		transform-origin: 50px 50px;animation: lasgo 2s linear 0s infinite;
	}
	@keyframes lasgo{
		0%{transform: rotate(0deg);background: #008FD0;}
		50%{background: #00FFFF;}
		100%{transform: rotate(360deg);
	}
	
</style>
	</head>
	<body>
		<div class="box">1
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">
			<div><div></div></div>2
		</div>
		<div class="box">3
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">4
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">5
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">6
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">7
			<div></div>
			<div></div>	
			<div></div>
			<div></div>
		</div>
		<div class="box">8
			<div class="range">
				<div></div>
			</div>
		</div>
		<div class="box">9
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">10
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">11
			<div></div>
			<div></div>
			<div></div>
			<div></div>
			<div></div>
		</div>
		<div class="box">12
			<div class="tab">
			<div></div>
			</div>
		</div>
		
	</body>
</html>
