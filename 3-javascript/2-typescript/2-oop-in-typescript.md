# Object-Oriented Programming in TypeScript

to Object-Oriented Programming in TypeScript

**Object-Oriented Programming (OOP)** is a programming approach that revolves around "objects" containing both data and methods. It focuses on four key principles: _encapsulation_, _inheritance_, _polymorphism_, and _abstraction_. These principles empower developers to build code that is modular, reusable, and easy to maintain. OOP is widely used in software development because it allows us to model real-world scenarios effectively and handle complex applications efficiently.

By embracing OOP concepts in TypeScript, we can create cleaner architecture and more manageable code, ultimately leading to better software development practices.

## Classes and Objects

In TypeScript, _classes_ serve as blueprints for creating objects. These structures encapsulate data and behavior that objects instantiated from the class can use. A _class_ defines properties (data) and methods (functions) that the objects will have.

To create a class in TypeScript, use the `class` keyword followed by the class name. Inside the class body, define properties and methods:

```typescript
class Person {
  name: string;
  age: number;

  constructor(name: string, age: number) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name}`);
  }
}
```

Properties are variables associated with a class. Methods are functions that describe actions an object can perform.

### Example: Properties and Methods in a Class

In the `Person` class example above:

- Properties:
- `name`: Stores the name of the person.
- `age`: Stores the age of the person.
- Method:
- `greet()`: Logs a greeting message to the console.

To create an instance (object) of a class, use the `new` keyword followed by the class constructor:

```typescript
let person1 = new Person("Alice", 30);
person1.greet(); // Output: Hello, my name is Alice
```

An object like `person1` has access to all properties and methods defined in its class. This approach ensures organized code and reusability by defining a template through classes.

## Interfaces and Abstract Classes

### Interfaces

Interfaces in Object-Oriented Programming define a contract for classes. They specify what properties and methods an object should have without implementing them. In TypeScript, interfaces are particularly useful:

```typescript
interface Vehicle {
  make: string;
  model: string;
  year: number;
  startEngine(): void;
}
```

This interface ensures that any class implementing it will have the specified properties and methods.

Utilizing interfaces enforces consistency across different parts of your application. When a class implements an interface, it must provide concrete implementations for the declared members:

```typescript
class Car implements Vehicle {
  make: string;
  model: string;
  year: number;

  constructor(make: string, model: string, year: number) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  startEngine() {
    console.log("Engine started");
  }
}
```

`Vehicle` is an interface with four members: `make`, `model`, `year` (properties), and `startEngine()` (method).

### Abstract Classes

Abstract classes in TypeScript are blueprints for other classes. They can contain both fully implemented methods and abstract methods that must be implemented by derived classes. This combination provides a balance between code reuse and enforcing certain behaviors.

An abstract method is defined without implementation in an abstract class. Derived classes must implement these methods:

```typescript
abstract class Animal {
  abstract makeSound(): void;

  move(): void {
    console.log("Moving...");
  }
}

class Dog extends Animal {
  makeSound() {
    console.log("Bark");
  }
}
```

`Animal` is an abstract class, which means it cannot be instantiated directly. It has an abstract method `makeSound()` that doesn't have an implementation, and a concrete method `move()` that logs "Moving...".

## Inheritance and Polymorphism

### Inheritance in TypeScript

Inheritance allows you to create a new class that reuses, extends, or modifies the behavior of another class. This is a fundamental concept in OOP that promotes code reusability.

```typescript
class Car implements Vehicle {
  make: string;
  model: string;
  year: number;

  constructor(make: string, model: string, year: number) {
    this.make = make;
    this.model = model;
    this.year = year;
  }

  startEngine() {
    console.log("Engine started");
  }
}
```

`Car` is a class that implements the `Vehicle` interface, meaning it must have the properties and methods declared in the Vehicle interface.

The `Car` class has a constructor that takes three parameters (`make`, `model`, `year`) and assigns them to the class properties.

The `startEngine()` method in the `Car` class is an implementation of the `startEngine()` method declared in the `Vehicle` interface. It logs "Engine started" to the console when called.

### Implementing Inheritance Hierarchies

Inheritance hierarchies allow for more complex relationships between classes. Child classes inherit properties and methods from parent classes, which can be further extended.

```typescript
class Dog extends Animal {
  makeSound() {
    console.log("Bark");
  }
}
```

`Dog` is a concrete class that extends the `Animal` abstract class. It provides an implementation for the `makeSound()` method, which logs "Bark".

### Exploring Polymorphism

Polymorphism enables objects to be treated as instances of their parent class rather than their actual class. This allows for more flexible code.

```typescript
const dog = new Dog();
dog.makeSound(); // Output: Bark
dog.move(); // Output: Moving...
```

A new Dog object is created and its `makeSound()` and `move()` methods are called. The `makeSound()` method uses the implementation provided in the `Dog` class, and the `move()` method uses the implementation inherited from the `Animal` class

## Encapsulation, Access Modifiers, and Encapsulation

Encapsulation is a core principle in Object-Oriented Programming that involves bundling data with methods that operate on that data. This principle protects the internal state of an object and restricts direct access to some of its components. In TypeScript, encapsulation not only enhances modularity but also ensures data integrity.

### Using Access Modifiers in TypeScript

TypeScript provides three primary access modifiers to control the visibility of class members:

- **public**: Members are accessible from anywhere.
- **private**: Members are accessible only within the class.
- **protected**: Members are accessible within the class and its subclasses.

Here is an example demonstrating these access modifiers:

```typescript
class Person {
  public name: string;
  private age: number;
  protected address: string;

  constructor(name: string, age: number, address: string) {
    this.name = name;
    this.age = age;
    this.address = address;
  }

  public getAge(): number {
    return this.age;
  }
}
```

In this example, we define a `Person` class with three properties: `name`, `age`, and `address`.

`name` is a public property, meaning it can be accessed from anywhere.

`age` is a private property, meaning it can only be accessed within the `Person` class.

`address` is a protected property, meaning it can be accessed within the `Person` class and any class that extends it.

The `Person` class has a constructor that takes three parameters (`name`, `age`, `address`) and assigns them to the class properties.

The `getAge()` method is a public method that returns the `age` of the `Person`. Since `age` is private, this method provides a way to access the `age` property outside of the `Person` class.

### Setters and Getters

Setters and getters provide controlled access to private properties. They allow you to implement logic when accessing or modifying properties.

```typescript
class Employee {
  private _salary: number;

  constructor(salary: number) {
    this._salary = salary;
  }

  get salary(): number {
    return this._salary;
  }

  set salary(newSalary: number) {
    if (newSalary > 0) {
      this._salary = newSalary;
    } else {
      throw new Error("Invalid salary amount");
    }
  }
}
```

This example code defines a `Employee` class with a private property `_salary`.

The get `salary()` method is a getter that returns the value of the `_salary` property. This allows external code to read the value of `_salary`.

The `set salary(newSalary: number)` method is a setter that allows external code to change the value of `_salary`. It checks if the `newSalary` is greater than 0 before assigning it to `_salary`. If `newSalary` is not greater than 0, it throws an error.

Getters and setters are used to control the access and modification of class properties. They provide a way to add additional logic (like validation) when getting or setting a property.

## Conclusion

Using **Object-Oriented Programming** principles in **TypeScript** can greatly improve your development process. It makes your code easier to maintain and reuse, leading to more efficient development overall. By utilizing features like classes, inheritance, polymorphism, and encapsulation, you can create powerful and flexible applications.
