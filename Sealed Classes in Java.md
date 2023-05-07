# Sealed Classes in Java

![j](https://user-images.githubusercontent.com/116082827/236656012-1cf62053-957d-44c6-a5bd-b6cb49290aac.png)


Java 15 introduced Sealed Classes, which provide a way to restrict the inheritance hierarchy of a class to a finite set of subclasses. Sealed classes are declared using the sealed modifier, and their permitted subclasses are declared using the permits keyword.

Example:





public sealed class Shape permits Circle, Rectangle, Triangle {

    // ...

}



public final class Circle extends Shape {

    // ...

}



public final class Rectangle extends Shape {

    // ...

}



public final class Triangle extends Shape {

    // ...

}
