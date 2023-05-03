# HTML Forms

![h](https://user-images.githubusercontent.com/116082827/235820185-4c76cd61-42f6-480d-8f17-d0a2fdbf9910.png)


HTML forms allow users to input data and submit it to a server. The form element is used to create a form, and various input elements are used to collect data from the user, such as text boxes, checkboxes, radio buttons, and drop-down lists. The action and method attributes are used to specify where and how the form data should be submitted.

Here's an example of how to create a simple form:





  <form action="/submit-form" method="post">

  <label for="name">Name:</label>

  <input type="text" id="name" name="name"><br>



  <label for="email">Email:</label>

  <input type="email" id="email" name="email"><br>



  <label for="message">Message:</label> */

  <textarea id="message" name="message"></textarea><br>



  <input type="submit" value="Submit">

</form>
