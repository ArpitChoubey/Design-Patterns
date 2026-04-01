# Test-Automation-Design-Patterns-Java-Framework


# 📘 Overview

This repository contains implementations of the **most important Design Patterns** in Java. These patterns represent **proven solutions** to commonly occurring design problems. They help structure code, make it reusable, scalable, and maintainable.

Design Patterns are broadly categorized into:

## ✔ Creational Patterns

* **Factory Pattern**
* **Builder Pattern**
* **Singleton Pattern**

## ✔ Structural Patterns

* **Decorator Pattern**
* (Other structural examples like Adapter/Proxy not included in repo, but theory applies.)

## ✔ Behavioral Patterns

* **Strategy Pattern**

This repository includes Java examples for all major patterns implemented inside:

```
eclipse-workspace/
└── SeleniumPractice/
    └── Design Patterns/
        └── src/
            ├── BuilderPattern/
            ├── DecoratorDesignPattern/
            ├── FactoryDesignPattern/
            ├── SingletonPattern/
            └── StrategyPattern/
```

---

# 🧩 Detailed Explanation of Design Patterns

## 1️⃣ Singleton Design Pattern

The **Singleton Pattern** ensures that **only one instance** of a class is created during runtime and provides a global point of access.

### 🔹 Why Singleton?

* Useful when exactly **one object** is needed (e.g., WebDriver instance, database connection, configuration reader)
* Prevents memory leaks
* Ensures controlled access

### 🔹 Features

* Private constructor
* Static instance variable
* Public static method that returns the instance

### 🔹 Advantages

* Controlled object creation
* Saves system resources

---

## 2️⃣ Builder Design Pattern

Used when constructing an object **requires many parameters**, especially optional ones.

### 🔹 Why Builder?

* Constructor becomes large & confusing if many parameters exist
* Factory becomes difficult to manage for complex objects
* Builder breaks object creation into **small steps**

### 🔹 Benefits

* Cleaner object creation
* Supports optional parameters
* Improves code readability

### 🔹 Example Areas

* Creating objects with 10–15 fields
* Selenium pages, test data models

---

## 3️⃣ Factory Design Pattern

Factory Pattern is used when there is a **superclass** and multiple **subclass implementations**, and the object creation must be delegated.

### 🔹 Problem Solved

* Removes `if-else` and `switch` conditions scattered throughout the code
* Centralizes object creation inside a **Factory class**

### 🔹 Advantages

* Loose coupling
* Focus on **interface**, not implementation
* Easy extension—add new subclass without modifying client code

---

## 4️⃣ Decorator Design Pattern

Decorator is a **structural pattern** used to add new functionalities to an object **dynamically**, without modifying its original structure.

### 🔹 Why Decorator?

* Inheritance leads to too many subclasses
* Need to add features at runtime (e.g., adding milk, sugar, cream)

### 🔹 How It Works

* Base component (e.g., Coffee)
* Decorators wrap the base component and add functionality

### 🔹 Benefits

* Flexible feature addition
* Promotes composition over inheritance

---

## 5️⃣ Strategy Design Pattern

Strategy defines a **family of algorithms**, encapsulates each one, and makes them interchangeable.

### 🔹 Use Case

Perfect when multiple actions depend on selected behavior, such as:

* PayPal payment
* Credit/Debit card payment
* Bank transfer

### 🔹 How It Works

* Strategy interface → defines common behavior
* Concrete strategies → each algorithm implementation
* Context → uses strategy object

### 🔹 Advantages

* Eliminates complex `if-else`
* Easy to add new strategies

---

# 📂 Folder Structure

```
Design-Patterns/
└── src/
    ├── BuilderPattern/
    │   ├── Product.java
    │   ├── ProductTest.java
    │   └── package-info.java
    │
    ├── DecoratorDesignPattern/
    │   ├── Coffee.java
    │   ├── CoffeeDecorator.java
    │   ├── SimpleCoffee.java
    │   ├── MilkDecorator.java
    │   ├── CreamCoffee.java
    │   ├── SugarDecorator.java
    │   ├── CoffeeShop.java
    │   └── package-info.java
    │
    ├── FactoryDesignPattern/
    │   ├── CarFactory.java
    │   ├── Car.java
    │   ├── Mini.java
    │   ├── SEDAN.java
    │   ├── SUV.java
    │   ├── CarTest.java
    │   └── package-info.java
    │
    ├── SingletonPattern/
    │   ├── Examples.java
    │   ├── Jalebi.java
    │   ├── Samosa.java
    │   └── package-info.java
    │
    └── StrategyPattern/
        ├── PaymentStrategy.java
        ├── PayPalPayment.java
        ├── CreditCardPayment.java
        ├── BankTransferPayment.java
        ├── PaymentContext.java
        ├── PaymentTest.java
        └── package-info.java
```

---

# 🎯 Summary

This repository provides clear and practical Java examples of the most commonly used **Design Patterns**:

* Singleton
* Builder
* Factory
* Decorator
* Strategy

These implementations are ideal for:

* Interview preparation
* Framework design
* Improving OOP and design architecture skills

## 👨‍💻 Author

**Arpit Choubey — SDET | QA | Automation Engineer**
🔗 **LinkedIn** | **Medium**

## ⭐ Support

If this repository helps you, please **Star 🌟** it.



