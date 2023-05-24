# Pattern Matching for Switch (introduced in Java 14)

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/194cbd00-bcc7-425d-ae88-3539e8f179d8)


Pattern matching for switch simplifies the common use case of performing different actions based on the value of a variable. It eliminates the need for repetitive casting and enhances code readability. Here's an example:



String day = "Sunday";



switch (day) {

    case "Monday", "Tuesday", "Wednesday", "Thursday", "Friday" ->

        System.out.println("It's a weekday.");

    case "Saturday", "Sunday" ->

        System.out.println("It's a weekend day.");

    default ->

        System.out.println("Invalid day.");

}
