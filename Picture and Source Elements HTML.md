 # Picture and Source Elements

![h](https://user-images.githubusercontent.com/116082827/235954812-53730272-6e08-4a02-a12b-defe27de1d24.png)


The picture and source elements are used to provide alternative image sources for different screen sizes and resolutions. The picture element is used to wrap different source elements, each specifying a different image source and media query. The browser will select the appropriate image source based on the device's screen size and resolution.

Here's an example of how to use the picture and source elements:





<picture>

  <source media="(min-width: 800px)" srcset="large-image.jpg">

  <source media="(min-width: 400px)" srcset="medium-image.jpg">

  <img src="small-image.jpg" alt="My Image">

</picture>
