<html>
	<head>
		<style>
			#main{width: 300px; height: 280px; background-color: black;}
			input{width: 20%; height: 40px; font-size: 20 px; margin: 6px;}
			#eee{width:96%;height: 50px; background-color: silver;}
		</style>
	</head>
	<body>
		<div id="main">
				<form name="f">
					<input type="text" name="ddd" placeholder="0" id='eee'> 
					<br>
					<input type="button" value="1" onclick="f.ddd.value+=1">
					<input type="button" value="2" onclick="f.ddd.value+=2">
					<input type="button" value="3" onclick="f.ddd.value+=3">
					<input type="button" value="+" onclick="add()">
					<br>
					<input type="button" value="4" onclick="f.ddd.value+=4">
					<input type="button" value="5" onclick="f.ddd.value+=5">
					<input type="button" value="6" onclick="f.ddd.value+=6">
					<input type="button" value="-" onclick="sub()">
					<br>
					<input type="button" value="7" onclick="f.ddd.value+=7">
					<input type="button" value="8" onclick="f.ddd.value+=8">
					<input type="button" value="9" onclick="f.ddd.value+=9">
					<input type="button" value="%" onclick="di()">
					<br>
					<input type="button" value="C" onclick="f.ddd.value=''">
					<input type="button" value="0" onclick="f.ddd.value+=0">
					<input type="button" value="=" onclick="f.ddd.value=eval(f.ddd.value)">
					<input type="button" value="X" onclick="mul()">
					
				</form>
		</div>
		
		<script>
			function add(){
				var a=0, b=0;
			a= f.ddd.value;
			b=a.charAt(a.length-1);
			if(b=='+' || b=='-' || b=='/'|| b=='*'){
				f.ddd.value=a.substring(0,a.length-1);
				f.ddd.value+='+';
				
			}
			else {
				f.ddd.value+='+';
			
			}
			
			}
			
			function sub(){
				var a=0, b=0;
			a= f.ddd.value;
			b=a.charAt(a.length-1);
			if(b=='+' || b=='-' || b=='/'|| b=='*'){
				f.ddd.value=a.substring(0,a.length-1);
				f.ddd.value+='-';
				
			}
			else {
				f.ddd.value+='-';
			
			}
			
			}
			
			
			
			
			function di(){
				var a=0, b=0;
			a= f.ddd.value;
			b=a.charAt(a.length-1);
			if(b=='+' || b=='-' || b=='/'|| b=='*'){
				f.ddd.value=a.substring(0,a.length-1);
				f.ddd.value+='/';
				
			}
			else {
				f.ddd.value+='/';
			
			}
			
			}
			
			
			
			
			function mul(){
				var a=0, b=0;
			a= f.ddd.value;
			b=a.charAt(a.length-1);
			if(b=='+' || b=='-' || b=='/'|| b=='*'){
				f.ddd.value=a.substring(0,a.length-1);
				f.ddd.value+='*';
				
			}
			else {
				f.ddd.value+='*';
			
			}
			
			}
		
		</script>
		

	</body>
</html>
