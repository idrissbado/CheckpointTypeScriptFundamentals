# Vehicle and Car Implementation in TypeScript

This project demonstrates how to define an interface and implement a class in TypeScript. The goal is to create a `Vehicle` interface and a `Car` class that implements this interface. The `Car` class will have properties and methods as specified, and we will test the implementation by creating an instance and calling its methods.

## Instructions

Follow the steps below to complete the exercise:

1. **Define the `Vehicle` Interface**:
   - Create an interface named `Vehicle` with the following properties:
     - `make` of type `string`
     - `model` of type `string`
     - `year` of type `number`
   - Include a `start` method that returns `void` and logs `"Engine started"` to the console.

2. **Implement the `Car` Class**:
   - Create a class named `Car` that implements the `Vehicle` interface.
   - The class should have a constructor that initializes the `make`, `model`, and `year` properties.
   - Implement the `start` method to log `"Car engine started"` to the console.

3. **Create an Instance of `Car`**:
   - Instantiate the `Car` class with some values for `make`, `model`, and `year`.
   - Call the `start` method on the instance to verify that it logs the appropriate message to the console.

4. **Compile and Run**:
   - Compile the TypeScript code into JavaScript using the TypeScript compiler (`tsc`).
   - Run the compiled JavaScript code to ensure everything works as expected.

## Code Implementation

### TypeScript Code

```typescript
// Define the Vehicle interface
interface Vehicle {
    make: string;
    model: string;
    year: number;
    start(): void;
}

// Implement the Car class
class Car implements Vehicle {
    make: string;
    model: string;
    year: number;

    constructor(make: string, model: string, year: number) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    start(): void {
        console.log("Car engine started");
    }
}

// Create an instance of the Car class
const myCar = new Car("Toyota", "Corolla", 2021);

// Call the start method
myCar.start();
Steps to Compile and Run
### Compile TypeScript to JavaScript:

Save the TypeScript code in a file, e.g., vehicle.ts.

### Run the following command to compile the TypeScript code:
tsc vehicle.ts
### Run the JavaScript Code:

Use Node.js to run the compiled JavaScript file:
node vehicle.js
