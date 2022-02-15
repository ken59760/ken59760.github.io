<p>Chart by Haihong Zhou</p>
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  <title>Fruit</title>
<script>
    function changeCanvasColor () {
		// Locate the element "mycanvas" in the document.
	var fruit = [
            {"name":"Apple", "qt":20, "color":"red"},
            {"name":"Orange", "qt":10, color:"orange"},
            {name:"Banana", qt:15, color:"yellow"},
            {name:"Kiwi", qt:3, color:"green"},
            {name:"Blueberry", qt:5, color:"blue"},
            {name:"Grapes", qt:8, color:"purple"}
        ];
        var canvas = document.getElementById("mycanvas");
        var context = canvas.getContext("2d");
        context.fillStyle = "red";
        context.fillRect(0, 0, canvas.width, canvas.height);
		
		context.font="30px Arial";

        context.fillStyle = "black";
		var line=1;
		var height=35;
		context.fillText(fruit[0].name+"   "+fruit[0].qt,10,height*line);
    }
    document.addEventListener('DOMContentLoaded', changeCanvasColor);
</script>
</head>
<body>
<div id="gameArea">
    <canvas id="mycanvas" width="800" height="600"></canvas>
</div>

</body></html>