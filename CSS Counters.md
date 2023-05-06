# CSS Counters

![c](https://user-images.githubusercontent.com/116082827/236629915-bab66cfe-107a-497c-9b7a-9437b02f975b.png)


CSS Counters allow you to create automatic numbering and labeling for your content. Here's an example:



ol {

  counter-reset: my-counter;

  list-style-type: none;

}



li::before {

  content: counter(my-counter) ". ";

  counter-increment: my-counter;

}

In this code, we have an ordered list with a custom counter called my-counter defined by the counter-reset property. We use the ::before pseudo-element to insert the counter label before each list item and increment the counter using the counter-increment property.
