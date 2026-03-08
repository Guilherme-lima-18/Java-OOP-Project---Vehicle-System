# Java OOP Project - Vehicle System

This project is a simple **Object-Oriented Programming (OOP)** exercise written in **Java** that demonstrates the concepts of **inheritance, method overriding, and polymorphism**.

The program allows the user to create different types of vehicles through a **terminal menu**, such as **cars and motorcycles**, and display their information.

---

## About the Project

This project was created to practice important Java OOP concepts, including:

- Inheritance
- Method Overriding
- Polymorphism
- Classes and Objects
- User input with `Scanner`
- Menu-driven programs

The system works directly in the **terminal**, where the user can choose the type of vehicle and input its information.

---

## How the Program Works
When the program starts, a **menu** appears:

---
===== Vehicle Model =====
1. Car
2. Motorcycle
3. Exit
---
The user selects one of the available options.

---

### Car Option

If the user chooses **Car**, the program asks for:
- Vehicle brand
- Vehicle model
- Number of doors
Then the program displays the vehicle information.

Example output:
---
1. Brand: Toyota
2. Model: Corolla
3. Doors: 4

---

### Motorcycle Option

If the user chooses **Motorcycle**, the program asks for:
- Vehicle brand
- Vehicle model
- Engine displacement (cc)
  
Example output:
---
1. Brand: Yamaha
2. Model: MT-07
3. Cylinders: 689

---

### Exit

Selecting **3** ends the program.

---

## OOP Concepts Demonstrated

### Inheritance

The classes **Car** and **Moto** inherit from the base class **Veiculo**.

```java
class Carro extends Veiculo
class Moto extends Veiculo
```
---

## Method Overriding
### Each subclass overrides the mostrarInfo() method to display its specific information.
```Java
@Override
void mostrarInfo(){
    System.out.println("Marca: " + marca);
    System.out.println("Modelo: " + modelo);
    System.out.println("Portas: " + portas);
}
```

---

## Polymorphism
### The program uses a reference of type Veiculo to store objects of different subclasses.
```Java
Veiculo v = null;

