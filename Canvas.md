# Canvas 

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/05fce46c-abc1-421d-ba34-ee148a48dff8)


The <canvas> tag allows you to create dynamic graphics and animations using JavaScript. You can use the Canvas API to draw shapes, lines, and text, as well as create animations and interactive applications.



<canvas id="myCanvas"></canvas>



<script>

  const canvas = document.getElementById("myCanvas");

  const ctx = canvas.getContext("2d");



  // Draw a rectangle

  ctx.fillStyle = "red";

  ctx.fillRect(10, 10, 50, 50);



  // Draw a circle

  ctx.beginPath();

  ctx.arc(75, 75, 30, 0, 2 * Math.PI);

  ctx.fillStyle = "blue";

  ctx.fill();

</script>
