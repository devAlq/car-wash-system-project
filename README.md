# Car Wash System

## Objective 
The purpose of this project is to validate your knowledge of the `queue` **data structure**. 

## Problem
A car wash company needs a `customer management program` to manage the cars waiting to be washed. The system should be able to **add cars to the waiting queue** and **process them in the order they arrived**, so the first car that arrived should be the first to be washed.

## Implementation 
Create a class called `Car` to hold the information of a car such as the type, color, and plate number.
Create a WashQueue class that will manage the cars, the class should able to do the following
operations:
- Add a car to the queue.
- Wash the first car in the queue and remove it from the queue.
- Print the total number of cars in the queue.
- Print the first car in the queue.


## Test Case 
```java

public static void main(String[] args) {
    WashQueue queue = new WashQueue();
    queue.addCar(new Car("Sedan", "Red", "1234"));
    queue.addCar(new Car("SUV", "Black", "5678"));
    queue.addCar(new Car("Truck", "White", "91011"));
    queue.addCar(new Car("Sedan", "Blue", "1213"));

    queue.printFirstCar();
    queue.printTotalCars();
    
    queue.washCar();

    queue.printFirstCar();
    queue.printTotalCars();
}

```

```OUTPUT
Car Type: Sedan
Car Color: Red
Car Plate: 1234

Total Cars: 4

Car Type: SUV
Car Color: Black
Car Plate: 5678

Total Cars: 3
```

## Qualification to pass 
- The system shall run without any errors.
- The system ouputs shall match the test case output.
- The system shall be able to add cars to the queue, remove the first car in the queue, print the first car in the queue, and print the total number of cars in the queue.
