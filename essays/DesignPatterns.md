---
layout: essay
type: essay
title: "Learning From Other Mistakes"
# All dates must be YYYY-MM-DD format!
date: 2024-12-05
published: true
labels:
  - Learning
  - Software Engineering
---

<img width="200px" class="rounded float-start pe-4" src="https://miro.medium.com/v2/resize:fit:720/1*t9pXNsn5rUaeECmNTA1m0Q.png">

## What are Design Patterns?

Design patterns are reusable solutions to common problems encountered in software development. Rather than providing specific code, they offer general frameworks that developers can adapt to fit their needs. These patterns help address issues related to object creation, system structure, and behavior, offering an efficient approach to solving recurring design challenges.

Rather than being concrete implementations, design patterns are abstract concepts that guide how to structure code and make design decisions. They emphasize flexibility, scalability, and maintainability, helping developers avoid reinventing the wheel. By using design patterns, teams can improve collaboration, reduce complexity, and create systems that are easier to maintain and extend.

There are three main categories of design patterns. Creational patterns, like the Factory Method and Singleton, focus on how objects are created. Structural patterns, such as the Adapter and Composite, deal with the organization of classes and objects. Behavioral patterns, including the Observer and Strategy, address how objects interact with one another.

## Design Patterns I Have Used Before

One design pattern I’ve implemented is the Factory Method. This pattern defines an interface for creating objects but lets subclasses alter the type of objects they create. It helps separate object creation from the class that uses the object, making the system more flexible and easier to maintain.

In my project, Fishing Frenzy Bash, we used the Factory Method to create different types of fish objects. We had a base Fish class that defined common properties, and subclasses like Uhu and Oama each implemented their own specific behaviors. This approach made it easy to add new fish types without altering the core logic of the game, keeping the system flexible and scalable.

Using design patterns like the Factory Method helps solve problems more efficiently and encourages better software design practices, leading to more maintainable and extensible code.


