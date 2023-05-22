# CSS Animations

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/5d97d99e-fa39-4465-8825-d2d47b95e403)


CSS animations allow you to add dynamic and interactive effects to elements. Here's an example of a simple animation:



@keyframes slide-in {

  0% {

    transform: translateX(-100%);

  }

  100% {

    transform: translateX(0);

  }

}



.box {

  animation: slide-in 1s forwards;

}
