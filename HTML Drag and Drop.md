# HTML Drag and Drop

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/529d5171-5228-4c0b-8b32-7321832e5423)


HTML5 includes a drag and drop API that allows you to make elements draggable and define drop zones. You can use JavaScript event handlers to handle drag and drop events. Here's an example:



<div id="dragElement" draggable="true" ondragstart="dragStart(event)">Drag me</div>

<div id="dropZone" ondrop="drop(event)" ondragover="allowDrop(event)">Drop here</div>



<script>

  function dragStart(event) {

    event.dataTransfer.setData("text", event.target.id);

  }



  function allowDrop(event) {

    event.preventDefault();

  }



  function drop(event) {

    event.preventDefault();

    const data = event.dataTransfer.getData("text");

    const draggedElement = document.getElementById(data);

    event.target.appendChild(draggedElement);

  }

</script>
