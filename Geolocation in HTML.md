# Geolocation

![h](https://user-images.githubusercontent.com/116082827/235913357-90dfb9fe-fb06-4620-bef5-030e6ece23d4.jpeg)


HTML provides built-in support for getting the user's location using the Geolocation API. This API allows you to get the user's latitude and longitude, as well as their altitude and speed, if available. You can use this information to provide location-based services, such as finding nearby restaurants or weather information.

Here's an example of how to get the user's location:





<button onclick="getLocation()">Get Location</button>

<p id="location"></p>

<script>

  function getLocation() {

    if (navigator.geolocation) {

      navigator.geolocation.getCurrentPosition(showPosition);

    } else {

      document.getElementById("location").innerHTML = "Geolocation is not supported by this browser.";

    }

  }

  function showPosition(position) {

    document.getElementById("location").innerHTML = "Latitude: " + position.coords.latitude + "<br>Longitude: " + position.coords.longitude;

  }

</script>
