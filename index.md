<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
  <head>
    <title>h.html</title>
	
    <meta http-equiv="keywords" content="keyword1,keyword2,keyword3">
    <meta http-equiv="description" content="this is my page">
    <meta http-equiv="content-type" content="text/html; charset=UTF-8">
    
    <!--<link rel="stylesheet" type="text/css" href="./styles.css">-->

  </head>
  
  <body>
   <script>
   var c=0;
   var x=0;
   var t;
   function timedCount(){
   	document.getElementById("txt").value=c;
   	c=c+1;
    	t=setTimeout(timedCount,1000);
   }
   function doTimer(){
   	if (!x){
   		x=1;
   		document.getElementById("txt").innerHTML=timedCount();
   	}
   }
   function stopCount(){
   	clearTimeout(t);
      	x=0;
   }
   </script>
   
   <input type="button" value="开始计数!" onclick="doTimer()" />
   <input type="text" id="txt" />
   <input type="button" value="停止计数!" onclick="stopCount()" />

  </body>
</html>
