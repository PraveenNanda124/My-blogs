# The HTML5 Geolocation 

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/a8d68812-6ade-4d5e-9bc6-a1564e4ca579)


Geolocation API allows you to access the user's location information, with their permission, using JavaScript. You can use this information to display location-based content or to create location-aware web applications.



<button onclick="getLocation()">Get Location</button>



<script>

  function getLocation() {

    if (navigator.geolocation) {

      navigator.geolocation.getCurrentPosition(showPosition);

    } else {

      alert("Geolocation is not supported by this browser.");

    }

  }



  function showPosition(position) {

    alert(`Latitude: ${position.coords.latitude}, Longitude: ${position.coords.longitude}`);

  }

</script>
