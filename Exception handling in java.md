# Exception handling in java

![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/48c28d96-f2b9-4205-b434-062f63195533)


Exception handling is a mechanism in Java that allows developers to handle errors and exceptions that occur during program execution. Here is an example of how to use exception handling in Java:



import java.io.File;

import java.io.FileNotFoundException;

import java.util.Scanner;



public class Main {

  public static void main(String[] args) {

    try {

      File file = new File("input.txt");

      Scanner scanner = new Scanner(file);



      while (scanner.hasNextLine()) {

        String line = scanner.nextLine();

        System.out.println(line);

      }



      scanner.close();

    } catch (FileNotFoundException e) {

      System.out.println("Error: file not found");

    }

  }

}![s](https://github.com/PraveenNanda124/Technical-blogs/assets/116082827/a397dae7-d61e-4ee3-988d-3b83db0dc549)


In this example, we try to read data from a file called input.txt. If the file is not found, the FileNotFoundException exception is thrown. We catch this exception and print an error message. If the file is found, we read each line of the file and print it to the console.

