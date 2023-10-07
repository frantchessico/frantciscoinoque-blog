---
title: Understanding Object-Oriented Programming (OOP) in TypeScript
publishDate: 25 Sep 2023
description: Object-Oriented Programming (OOP) stands as one of the most widely embraced paradigms in TypeScript, as well as numerous other programming languages.
---

**Introduction:**

Object-Oriented Programming (OOP) stands as one of the most widely embraced paradigms in TypeScript, as well as numerous other programming languages. TypeScript, recognized for its strong typing system, eagerly embraces the entire spectrum of essential OOP concepts, including classes, objects, inheritance, encapsulation, and polymorphism. In this article, we embark on a journey to delve deep into the realm of OOP within TypeScript, coupled with practical examples to reinforce our understanding.

**1. Classes:**

Classes serve as the bedrock upon which the edifice of Object-Oriented Programming is constructed. Within TypeScript, classes are crafted using the `class` keyword. Let's commence with a straightforward TypeScript class example:

```typescript
class Person {
  name: string;
  age: number;

  constructor(name: string, age: number) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name}, and I'm ${this.age} years old.`);
  }
}

const person1 = new Person('Alice', 30);
person1.greet(); // Output: Hello, my name is Alice, and I'm 30 years old.
```

**2. Objects:**

Objects manifest as instances of classes. The instantiation of a class begets an object. For instance, in the example provided, `person1` embodies an object of the `Person` class.

**3. Inheritance:**

Inheritance is a potent OOP concept, facilitated in TypeScript by the `extends` keyword. This allows for the creation of new classes that inherit attributes and behaviors from existing ones. Witness this in practice:

```typescript
class Student extends Person {
  course: string;

  constructor(name: string, age: number, course: string) {
    super(name, age);
    this.course = course;
  }

  greet() {
    console.log(`Hello, I'm a student named ${this.name}, and I'm studying ${this.course}.`);
  }
}

const student1 = new Student('Bob', 25, 'Computer Science');
student1.greet(); // Output: Hello, I'm a student named Bob, and I'm studying Computer Science.
```

**4. Encapsulation:**

In TypeScript, control over the accessibility of class members is wielded through access modifiers like `public`, `private`, and `protected`. By default, members are public. Observe this principle in action:

```typescript
class Animal {
  private name: string;

  constructor(name: string) {
    this.name = name;
  }

  getName() {
    return this.name;
  }
}

const animal1 = new Animal('Lion');
console.log(animal1.getName()); // Output: Lion
console.log(animal1.name); // Error: Property 'name' is private and only accessible within class 'Animal'.
```

**5. Polymorphism:**

Polymorphism, a cornerstone of OOP, enables the uniform treatment of objects from diverse classes. This feat is accomplished through inheritance and method overriding. The following example exemplifies polymorphism:

```typescript
// Base Animal class
class Animal {
  constructor(public name: string) {}

  makeSound() {
    console.log(`The animal ${this.name} makes a sound.`);
  }
}

// Class to represent a Dog
class Dog extends Animal {
  makeSound() {
    console.log(`${this.name} barks: Woof! Woof!`);
  }
}

// Class to represent a Cat
class Cat extends Animal {
  makeSound() {
    console.log(`${this.name} meows: Meow! Meow!`);
  }
}

// Function that takes an animal and makes it make a sound
function makeAnimalMakeSound(animal: Animal) {
  animal.makeSound();
}

// Creating instances of Dog and Cat
const dog = new Dog('Rex');
const cat = new Cat('Whiskers');

// Calling the function to make the animals make a sound
makeAnimalMakeSound(dog); // Output: Rex barks: Woof! Woof!
makeAnimalMakeSound(cat); // Output: Whiskers meows: Meow! Meow!
```



> **Conclusion (Polymorphism Section):**

Polymorphism, a central tenet of OOP, emerges as a potent tool for enhancing code flexibility and reusability. By forging class hierarchies and method overrides, a consistent approach is achieved when handling objects of diverse types. The example provided here elucidates how polymorphism simplifies code while fostering extensibility, a cornerstone of Object-Oriented Programming.

**Conclusion:**

Our exploration of Object-Oriented Programming in TypeScript unveils a world of code organization, reusability, and flexibility. These fundamental concepts lay the groundwork for crafting well-structured and adaptable codebases, essential for tackling intricate problem domains.