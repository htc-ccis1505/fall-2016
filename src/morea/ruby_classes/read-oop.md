---
title: "Intro to Object Oriented Programming"
published: true
morea_id: read-oop
morea_summary: "An introduction to the main concepts of Object Oriented Programming."
morea_type: reading
morea_sort_order: 1
morea_labels:
 - ruby
---

# {{ page.title }}
{{ page.morea_summary }}

## What is Object Oriented Programming?
The programming that we have done so far (both in Snap and Ruby) has been focused around building functions to structure and organize our code.  This is referred to as __procedural__ programming.  Procedural programming is one of many [programming paradigms](https://en.wikipedia.org/wiki/Programming_paradigm). (A paradigm is basically a way to do something.)  For the remainder of the course, we'll be looking at a new (both to us and historically newer) paradigm called object-oriented programming.  

In object-oriented programming we structure our code around objects. An object is conceptually a "thing" that you might imagine. Often these tie to physical things that we represent in our program code - like a Person, a Car, an InventoryItem, a Server, a UserGroup, etc.  The things we might represent in code with objects fall out of our application domain.  If we have a program to monitor a network of servers, we might have a Server object or a Router object, but we probably wouldn't have a Car object or a Person object.  On the other hand if we were managing a fleet of vehicles for a document delivery service, those Car and Person objects make more sense.

In object-oriented programming, the code is organized first into objects, but we still use the same tools - variables, functions, and control structures - that you are familiar with from writing procedural code.  However in object-oriented code, these variables and functions exists inside of objects.  Variables that belong to objects are called instance variables, and functions that belong to objects are called methods.  

## Objects, Classes, & Instances
These three terms come up a lot in object oriented programming and understanding what each term means and how it is different from the others is important when discussing object object-oriented program code.

An __object__ is a conceptual thing.  It is the thing you are representing in your code by making a class.

A __class__  defines how to make an object.  It isn't an object itself, it just the definition of what that object is, like a blueprint or a template.  This definition is used to make instances of your object.

An __instance__ is one of many possible "real" (in the code sense) objects that could be made from your class.  

An example might help to make this more clear.  Let focus on Car objects.  (Programmers generally capitalize the names of their objects.)  We might have a class define a Car to have some properties like make, model and year.  These properties are things that help us differentiate one car from another.  They are things that the Car object __HAS__.  A Car HAS-A make. It HAS-A model.  It HAS-A (model) year.

So this Car object is just a concept in our program design.  We make this real in our code by defining a class for that Car object.  We'll look at how to do that in Ruby soon, but for now we'll skip those details.  Once we have a class that says every car has a make, model, and year, we can start making actual Cars in our program code.  We might make a 2000 Toyota Celica, or a 2010 Mini Cooper, or a 2016 Honda Civic.  Each individual car we make is an instance of the Car class, and each one is also considered a (instance of a) Car object.  (I put that in parenthesis because it is true, but wordy and people usually leave that off.)

## What Can Objects Do?
We talked about things that objects *have*, their __properties__, but object often are also able to do things.  A Car wouldn't be much fun if it didn't drive, right?  We call these things that objects can do __behaviors__ and they correspond to methods that are defined for that object in our program code.  

Going back to the Car object, you might have behaviors to accelerate, brake, turn right, turn left, reverse direction, etc. When we talk about properties and behaviors, that is generally while considering the *design* of our object.  When designing, we are imagining what it might be like and deciding what pieces are important to our application. These behaviors are *implemented* or made real in the application by adding methods to the Car class definition.

## What about things that are Car-like?
We will cover this in more detail later, but when thinking about objects, they often (but not always) come in families.  There are many similarities between cars, trucks, SUVs, vans, etc.  Depending on what properties and behaviors we care about for each of those things, they might all be represented by the same class, and maybe that would be better called MotorVehicle?  (Naming is something that tends to change a lot in the design or imagining phase.)  

What about a motorcycle though? It's certainly similar in some ways.  It has the same properties and behaviors we mentioned above.  We would say that a Motorcycle __IS-A__ MotorVehicle, because it is shares all those properties and behaviors.  However, the Motorcycle is clearly visually different.  It only has 2 wheels, and it's not enclosed. There are many ways it is different from a car or truck.  Depending on the program, those things may or may not matter.  

If the differences do matter, we may want to create a different object to represent Motorcycles, but perhaps we want to use some of the same properties and behaviors that we had for our more generic MotorVehicle.  We can do that by extending the MotorVehicle class.  When we extend a class, we __inherit__ it's properties and behaviors.  We also say that the new class is a __child__ of the class we are extending.  The class we are extending is the __parent__ of the new class we are making.  

Classes can be extended multiple times, allowing for many child classes, and child classes can also be further extended.  (In practice though, these class hierarchies (or you might think of them as object family trees) are often very shallow, only 1-2 levels deep.  Imagine not just Motorcycles extending MotorVehicle, but perhaps also RecreationalVehicles, Semi-Trucks, Buses, etc.

There are several benefits to extending classes in this way.  By re-using the properties and methods in the base class, you are getting code that is already tested.  Changes that need to be made are made in one place (the parent class) and then shared by all the child classes.  New child classes can be added easily without affecting the existing parent class or any other child classes.  Changes to the parent affect all children, but changes to children do not affect the parent or any other children.

## IS-A and HAS-A
The IS-A and HAS-A language comes up frequently in object-oriented design and programming.  I will expect you to understand the differences between the two concepts.  This often falls out pretty naturally when talking about the objects.  The IS-A terminology is used for extending classes (inheritance), while the HAS-A terminology is used for instance variables, or properties of a class.

For example, if we are designing a car, which relationship would we use when thinking about the driver?  

A Car HAS-A Driver.  
OR  
A Car IS-A driver.  

Unless we've got self-driving cars, the statement a Car IS-A driver, doesn't make much sense, so it's more likely that our Car HAS-A driver.  That means we would give our Car a property (or instance variable) for the driver instead of having our Car class extend a Driver class.


## Review Questions

- How is object-oriented programming different from functional/procedural programming?
- What is an object?  How is it different from a class?
- What is an instance?
- How are object properties and behaviors implemented in program code?
- Why would you extend a class instead of just creating a new *stand alone* class?
- Explain how the words IS-A and HAS-A are used in object-oriented design.
