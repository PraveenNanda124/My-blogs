# Web Components

![w](https://user-images.githubusercontent.com/116082827/235355007-14a61ba5-74c2-4fab-9340-a043344a4e47.jpeg)


Web Components are a set of standards that allow developers to create reusable UI components that can be used across multiple projects and frameworks. Web Components consist of three main technologies: Custom Elements, Shadow DOM, and HTML Templates. Here's an example of using Custom Elements to create a custom button component:





class MyButton extends HTMLElement {

  constructor() {

    super();

    this.addEventListener('click', () => {

      console.log('Button clicked!');

    });

  }

}



customElements.define('my-button', MyButton);

In this code, we're using the class syntax to define a custom element called my-button. We're adding a click event listener that logs a message to the console when the button is clicked. We're also using the customElements.define method to register our custom element with the browser. Once registered, we can use our custom button component in any HTML document by adding a <my-button> tag.
