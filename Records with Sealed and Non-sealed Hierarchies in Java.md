# Records with Sealed and Non-sealed Hierarchies in Java

![j](https://user-images.githubusercontent.com/116082827/236668737-ecc8de95-53b4-460e-839a-57e7a58a56b2.png)


Java 17 introduced an enhancement to records that enables them to participate in sealed and non-sealed hierarchies. This feature allows records to be defined as sealed or non-sealed, and it also enables records to be used as permitted subclasses.

Example:





public sealed interface Animal permits Dog, Cat, Bird, Fish {

    record Dog() implements Animal {}

    record Cat() implements Animal {}

    non-sealed interface Bird extends Animal {}

    final class Fish implements Animal {}

}
