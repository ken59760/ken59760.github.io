<!DOCTYPE html>
<!-- saved from url=(0081)https://www.sci.brooklyn.cuny.edu/~goetz/cisc3610/html5/canvas-text-advanced.html -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <title>Canvas Example</title>
<script>
    function changeCanvasColor () {
		// Locate the element "mycanvas" in the document.
        var canvas = document.getElementById("mycanvas");
        var context = canvas.getContext("2d");
        context.fillStyle = "red";
        context.fillRect(0, 0, canvas.width, canvas.height);
		
		context.font="30px Arial";
        context.fillStyle = "black";
		var line=1;
		var height=35;
		context.fillText("Apple",10,height*line);
		line++;
		context.fillText("20",10,height*line);
    }

	// Once the HTML document has finished loading and has been parsed, call the changeCanvasColor function.
    document.addEventListener('DOMContentLoaded', changeCanvasColor);
</script>
</head>
<body>
<div id="gameArea">
    <canvas id="mycanvas" width="800" height="600"></canvas>
</div>

</body></html>