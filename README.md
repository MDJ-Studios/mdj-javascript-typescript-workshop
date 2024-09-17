# Introduction to JavaScript and TypeScript

Welcome to your journey into the world of JavaScript and TypeScript! This guide is designed for complete beginners. We'll start with the basics of JavaScript, build a simple project, and then enhance it using TypeScript. By the end of this tutorial, you'll have a solid foundation in programming with JavaScript and TypeScript.

## Table of Contents

1. [Setting Up Your Environment](#setting-up-your-environment)
2. [JavaScript Fundamentals](#javascript-fundamentals)
   - [Variables and Data Types](#variables-and-data-types)
   - [Control Structures](#control-structures)
   - [Functions](#functions)
   - [Classes](#classes)
3. [Building a Simple Project](#building-a-simple-project)
4. [Introduction to TypeScript](#introduction-to-typescript)
   - [Adding Types to Your Project](#adding-types-to-your-project)
5. [Conclusion and Next Steps](#conclusion-and-next-steps)

---

## Setting Up Your Environment

To get started, we'll use [Replit](https://replit.com/), a cloud-based coding platform that allows you to write and run JavaScript and TypeScript code right in your browser.

### Steps to Set Up Replit

1. **Create an Account:**

   - Go to [Replit Sign Up](https://replit.com/signup) and create a free account.

2. **Create a New Repl:**

   - Click on the **"+"** button and select **"JavaScript"** as your language.

3. **Familiarize Yourself with the Interface:**
   - The main area is your code editor.
   - On the right is the console where your code will run.

Now you're ready to start coding!

---

## JavaScript Fundamentals

### Variables and Data Types

#### Variables

Variables store data values. In JavaScript, you can declare variables using `var`, `let`, or `const`.

- `var` is function-scoped or globally scoped.
- `let` and `const` are block-scoped. `const` is used for constants.

**Example:**

```javascript
var name = "Alice";
let age = 25;
const pi = 3.1416;
```

#### Data Types

1. **Number**: Represents both integer and floating-point numbers.

   ```javascript
   let count = 10;
   let price = 19.99;
   ```

2. **String**: Textual data enclosed in quotes.

   ```javascript
   let greeting = "Hello, world!";
   ```

3. **Boolean**: Represents `true` or `false`.

   ```javascript
   let isStudent = true;
   ```

4. **Null**: Represents an intentional absence of value.

   ```javascript
   let emptyValue = null;
   ```

5. **Undefined**: Variable declared but not assigned a value.

   ```javascript
   let notAssigned;
   ```

6. **Object**: Complex data structures.

   ```javascript
   let person = { name: "Bob", age: 30 };
   ```

7. **Symbol**: Unique and immutable identifiers (advanced).

### Control Structures

Control structures determine the flow of execution in your code.

#### Conditional Statements

**`if...else` Statement**

```javascript
let score = 85;

if (score >= 90) {
  console.log("A grade");
} else if (score >= 80) {
  console.log("B grade");
} else {
  console.log("C grade");
}
```

**`switch` Statement**

```javascript
let day = 2;

switch (day) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  default:
    console.log("Another day");
}
```

#### Loops

**`for` Loop**

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Iteration " + i);
}
```

**`while` Loop**

```javascript
let i = 0;
while (i < 5) {
  console.log("Iteration " + i);
  i++;
}
```

### Functions

Functions are reusable blocks of code.

#### Function Declaration

```javascript
function add(a, b) {
  return a + b;
}
```

#### Function Expression

```javascript
const multiply = function (a, b) {
  return a * b;
};
```

#### Arrow Functions

```javascript
const subtract = (a, b) => a - b;
```

### Classes

Classes are blueprints for creating objects.

#### Creating a Class

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log("Hello, my name is " + this.name);
  }
}
```

#### Using a Class

```javascript
let alice = new Person("Alice", 25);
alice.greet(); // Output: Hello, my name is Alice
```

## TypeScript Fundamentals

### TypeScript Variables and Data Types

#### TypeScript Variables

Variables store data values. In TypeScript, you can declare variables using `var`, `let`, or `const`.

- `var` is function-scoped or globally scoped.
- `let` and `const` are block-scoped. `const` is used for constants.

**Example:**

```typescript
var name: string = "Alice";
let age: number = 25;
const pi: number = 3.1416;
```

#### TypeScript Data Types

1. **Number**: Represents both integer and floating-point numbers.

   ```typescript
   let count: number = 10;
   let price: number = 19.99;
   ```

2. **String**: Textual data enclosed in quotes.

   ```typescript
   let greeting: string = "Hello, world!";
   ```

3. **Boolean**: Represents `true` or `false`.

   ```typescript
   let isStudent: boolean = true;
   ```

4. **Null**: Represents an intentional absence of value.

   ```typescript
   let emptyValue: unknown | null = null;
   ```

5. **Undefined**: Variable declared but not assigned a value.

   ```typescript
   let notAssigned: unknown;
   ```

6. **Object**: Complex data structures.

   ```typescript
   interface IPerson {
     name: string;
     age: number;
   }

   let person: IPerson = { name: "Bob", age: 30 };
   ```

7. **Symbol**: Unique and immutable identifiers (advanced).

### TypeScript Control Structures

Control structures determine the flow of execution in your code.

#### TypeScript Conditional Statements

**`if...else` Statement**

```typescript
let score: number = 85;

if (score >= 90) {
  console.log("A grade");
} else if (score >= 80) {
  console.log("B grade");
} else {
  console.log("C grade");
}
```

**`switch` Statement**

```typescript
let day: number = 2;

switch (day) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  default:
    console.log("Another day");
}
```

#### TypeScript Loops

**`for` Loop**

```typescript
for (let i = 0; i < 5; i++) {
  console.log("Iteration " + i);
}
```

**`while` Loop**

```typescript
let i: number = 0;

while (i < 5) {
  console.log("Iteration " + i);
  i++;
}
```

### TypeScript Functions

Functions are reusable blocks of code.

#### TypeScript Function Declaration

```typescript
function add(a: number, b: number): number {
  return a + b;
}
```

#### TypeScript Function Expression

```typescript
const multiply = function (a: number, b: number): number {
  return a * b;
};
```

#### TypeScript Arrow Functions

```typescript
const subtract = (a: number, b: number): number => a - b;
```

### TypeScript Classes

Classes are blueprints for creating objects.

#### TypeScript Creating a Class

```typescript
interface IPerson {
  name: string;
  age: number;
}

class Person implements IPerson {
  age: number;
  name: string;

  constructor({ age, name }: IPerson) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log("Hello, my name is " + this.name);
  }
}
```

#### TypeScript Using a Class

```typescript
let alice: Person = new Person({ name: "Alice", age: 25 });
alice.greet(); // Output: Hello, my name is Alice
```

---

## Building a Simple Project

Let's build a simple **To-Do List** application that incorporates everything we've learned.

### Project Overview

We will:

- Store tasks using variables and arrays.
- Use functions to add, display, and remove tasks.
- Implement control structures to manage task statuses.
- Use a class to represent individual tasks.

### Step-by-Step Guide

#### 1. Create a Task Class

```javascript
class Task {
  constructor(title) {
    this.title = title;
    this.completed = false;
  }

  complete() {
    this.completed = true;
  }
}
```

#### 2. Initialize Task List

```javascript
let tasks = [];
```

#### 3. Function to Add a Task

```javascript
function addTask(title) {
  let task = new Task(title);
  tasks.push(task);
  console.log(`Added task: "${title}"`);
}
```

#### 4. Function to Display Tasks

```javascript
function displayTasks() {
  console.log("To-Do List:");
  tasks.forEach((task, index) => {
    let status = task.completed ? "[✓]" : "[ ]";
    console.log(`${index + 1}. ${status} ${task.title}`);
  });
}
```

#### 5. Function to Complete a Task

```javascript
function completeTask(index) {
  if (tasks[index]) {
    tasks[index].complete();
    console.log(`Completed task: "${tasks[index].title}"`);
  } else {
    console.log("Task not found");
  }
}
```

#### 6. Testing the Application

```javascript
addTask("Learn JavaScript fundamentals");
addTask("Build a simple project");
displayTasks();

completeTask(0);
displayTasks();
```

**Expected Output:**

```bash
Added task: "Learn JavaScript fundamentals"
Added task: "Build a simple project"
To-Do List:
1. [ ] Learn JavaScript fundamentals
2. [ ] Build a simple project
Completed task: "Learn JavaScript fundamentals"
To-Do List:
1. [✓] Learn JavaScript fundamentals
2. [ ] Build a simple project
```

---

## Introduction to TypeScript

TypeScript is a superset of JavaScript that adds static typing, which can help prevent errors and make your code more robust.

### Setting Up TypeScript on Replit

1. **Create a New Repl:**

   - Click on the **"+"** button and select **"TypeScript"** as your language.

2. **Familiarize Yourself with the Interface:**
   - Similar to the JavaScript setup.

### Differences Between JavaScript and TypeScript

- **Static Typing:** Variables and functions can have types.
- **Interfaces and Enums:** Additional structures for defining data shapes.

---

### Adding Types to Your Project

Let's convert our To-Do List application to TypeScript.

#### 1. Define the Task Class with Types

```typescript
class Task {
  title: string;
  completed: boolean;

  constructor(title: string) {
    this.title = title;
    this.completed = false;
  }

  complete(): void {
    this.completed = true;
  }
}
```

#### 2. Initialize Task List with Types

```typescript
let tasks: Task[] = [];
```

#### 3. Function to Add a Task with Types

```typescript
function addTask(title: string): void {
  let task = new Task(title);
  tasks.push(task);
  console.log(`Added task: "${title}"`);
}
```

#### 4. Function to Display Tasks with Types

```typescript
function displayTasks(): void {
  console.log("To-Do List:");
  tasks.forEach((task: Task, index: number) => {
    let status: string = task.completed ? "[✓]" : "[ ]";
    console.log(`${index + 1}. ${status} ${task.title}`);
  });
}
```

#### 5. Function to Complete a Task with Types

```typescript
function completeTask(index: number): void {
  if (tasks[index]) {
    tasks[index].complete();
    console.log(`Completed task: "${tasks[index].title}"`);
  } else {
    console.log("Task not found");
  }
}
```

#### 6. Testing the TypeScript Application

```typescript
addTask("Learn TypeScript");
addTask("Add types to the project");
displayTasks();

completeTask(1);
displayTasks();
```

**Expected Output:**

```bash
Added task: "Learn TypeScript"
Added task: "Add types to the project"
To-Do List:
1. [ ] Learn TypeScript
2. [ ] Add types to the project
Completed task: "Add types to the project"
To-Do List:
1. [ ] Learn TypeScript
2. [✓] Add types to the project
```

---

## Conclusion and Next Steps

Congratulations! You've learned the fundamentals of JavaScript and how to enhance your code with TypeScript. You've:

- Understood variables, data types, control structures, functions, and classes.
- Built a simple To-Do List application.
- Converted your JavaScript project into TypeScript by adding static types.

### Next Steps

- Explore more advanced topics like asynchronous programming with Promises and async/await.
- Learn about modules and how to structure larger applications.
- Experiment with front-end frameworks like React or Angular.
- Practice by building more projects.
