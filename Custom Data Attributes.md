# Custom Data Attributes

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/265f6726-281d-4989-9b55-35a353b8df72)


HTML allows you to define custom data attributes on HTML elements using the data- prefix. These attributes can store additional information that can be accessed using JavaScript. Here's an example:



<div id="myElement" data-color="blue" data-size="large"></div>



<script>

  const element = document.getElementById("myElement");

  const color = element.dataset.color;

  const size = element.dataset.size;



  console.log(color); // Output: blue

  console.log(size); // Output: large

</script>
