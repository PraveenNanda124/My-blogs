# Custom Elements

![c](https://user-images.githubusercontent.com/116082827/235812341-efd20a08-6a9f-4cdd-a37f-383d68978862.png)


Custom elements allow you to create your own HTML tags with custom functionality. They are created using the CustomElementRegistry API and can be used like any other HTML tag. Custom elements can encapsulate functionality and simplify the structure of your HTML code.

Here's an example of how to create a custom element:





class MyElement extends HTMLElement {

  constructor() {

    super();

    this.textContent = "Hello, World!";

  }

}

customElements.define('my-element', MyElement);

And here's how to use the custom element in your HTML code:





<my-element></my-element>
