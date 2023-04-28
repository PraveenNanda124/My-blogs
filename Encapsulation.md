# Encapsulation

![a](https://user-images.githubusercontent.com/116082827/235221282-5a515752-71d6-4c9c-ac90-973a7db05bba.jpeg)


Encapsulation is the process of hiding the internal details of an object from the outside world. In OOP, encapsulation is achieved through access modifiers such as private, protected, and public.



Here's an example of encapsulation in Java:





public class BankAccount {

    private double balance;



    public void deposit(double amount) {

        balance += amount;

    }



    public double withdraw(double amount) {

        if (balance < amount) {

            throw new IllegalArgumentException("Insufficient balance");

        }

        balance -= amount;

        return amount;

    }

}

In this example, we define a class called BankAccount. The balance field is declared as private, which means it can only be accessed within the class. The deposit and withdraw methods are declared as public, which means they can be accessed from outside the class. However, the withdraw method checks if the account has sufficient balance before allowing a withdrawal.
