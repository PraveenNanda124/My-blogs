# Inheritance

![a](https://user-images.githubusercontent.com/116082827/235278750-a4859a61-68b0-4953-a002-93e55d533efc.jpeg)


Inheritance is the process of creating a new class from an existing class, inheriting all the attributes and methods of the parent class. In OOP, inheritance is used to create specialized classes from a base class.



Here's an example of inheritance in C++:





class Vehicle {

protected:

    int num_wheels;

    int num_seats;



public:

    Vehicle(int wheels, int seats) {

        num_wheels = wheels;

        num_seats = seats;

    }



    void drive() {

        std::cout << "Driving the vehicle" << std::endl;

    }

};



class Car : public Vehicle {

public:

    Car(int seats) : Vehicle(4, seats) {}



    void park() {

        std::cout << "Parking the car" << std::endl;

    }

};

In this example, we define a base class called Vehicle that has a num_wheels and num_seats attributes and a drive method. We then define a derived class called Car that inherits from Vehicle and has a park method. The Car class calls the constructor of the Vehicle class using the : public Vehicle syntax.
