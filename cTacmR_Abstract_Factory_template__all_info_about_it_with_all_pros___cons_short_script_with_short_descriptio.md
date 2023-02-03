

# Abstract Factory Template
Abstract Factory is a creational design pattern that provides an interface for creating families of related or dependent objects without specifying their concrete classes.

## Pros
* Introduces decoupling between the client and the product family.
* Easily expandable to accommodate new types of products.
* A well-designed abstract factory should make adding new products easy.

## Cons
* Complexity: the pattern requires a lot of new interfaces, classes and other elements, making the code more complex.
* Extensibility: not open for extension. It’s hard to add new products to an existing product family since you have to change the abstract factory interface.

## Solution
The following example uses a **Factory of Factories** to create a family of related objects.

![Abstract Factory UML Diagram](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Abstract_factory_UML.svg/1200px-Abstract_factory_UML.svg.png)

The Abstract Factory interface declares a set of methods that return different abstract products. These products are called a **family** and are related by a high-level theme or concept.

The Factory of Factories is an abstract class that provides a method for creating a concrete factory. The concrete factory is responsible for creating a family of products.

The Concrete Factory knows and creates the concrete products that belong to a family.

The Abstract Product declares an interface for a type of product object.

The Concrete Product is a product object to be created by the corresponding Concrete Factory and it must implement the Abstract Product interface.

The Client uses only the Abstract Factory and Abstract Product interfaces. Thus, it can work with any concrete product and factory without knowing the concrete classes that represent them.