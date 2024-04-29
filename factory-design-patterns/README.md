# ![[tktk Module Name] - tktk Microlesson Name](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to examine the advantages and limitations of factory design patterns. 

### Factory design pattern (10 minutes)

The Factory Method pattern is a fundamental creational design pattern widely used in object-oriented software
development. It encapsulates the creation of objects within a class hierarchy, allowing clients to create instances of
objects without needing to know the exact class of the object being instantiated. This promotes loose coupling between
the client code and the classes being instantiated, enhancing flexibility and maintainability in the codebase.

At its core, the Factory Method pattern defines an interface for creating objects but allows subclasses to alter the
type of objects that will be created. This is achieved by defining a separate method, typically named something like "
factoryMethod," within an abstract base class. Subclasses then override this method to instantiate specific types of
objects that adhere to a common interface or are part of a related family of objects.

One of the key benefits of the Factory Method pattern is its ability to delegate the responsibility of object creation
to subclasses. This means that the decision-making process regarding which concrete class to instantiate is
decentralized, allowing each subclass to determine the appropriate type of object to create based on specific
requirements or conditions.

By using the Factory Method pattern, developers can introduce new types of objects into the system without modifying
existing client code. This promotes scalability and extensibility, as the addition of new subclasses enables the
creation of diverse sets of objects while maintaining compatibility with the existing codebase.

Furthermore, the Factory Method pattern is often used in conjunction with other design patterns, such as the Abstract
Factory pattern, to create families of related objects. In such cases, the Factory Method is responsible for creating
individual objects within a family, while the Abstract Factory coordinates the creation of entire families of related
objects.

In summary, the Factory Method pattern provides a flexible and scalable solution for object creation in object-oriented
systems. By encapsulating the instantiation process within subclasses, it promotes loose coupling, extensibility, and
maintainability in software development projects.

#### Advantages of Factory Pattern (10 minutes):

- **Encapsulation**: Factory pattern encapsulates the object creation logic, separating it from the client code. This
  promotes loose coupling between the client and the created objects.
- **Flexibility and Extensibility**: It allows for easy extension and modification of the object creation process. New
  types of objects can be added without altering existing client code, making the system more flexible and easily
  maintainable.
- **Abstraction**: Factory pattern provides an abstraction layer over object creation, allowing clients to work with
  interfaces or abstract classes rather than concrete implementations. This promotes code scalability and modifiability.
- **Centralized Control**: Object creation logic is centralized within the factory class, making it easier to manage and
  control the creation process. Any changes or updates to the creation logic can be applied uniformly across the system.
- **Decoupling**: Factory pattern decouples the client code from the specific types of objects being created, allowing
  clients to focus on their primary responsibilities without being concerned about object creation details.

#### Considerations and Criticisms (10 minutes):

- **Complexity**: In some cases, implementing a factory pattern may introduce additional complexity to the system,
  especially when dealing with a large number of object types or complex object creation logic.
- **Overhead**: Introducing a factory class may add some overhead to the application, particularly if the factory needs
  to be instantiated frequently or if the object creation process is resource-intensive.
- **Reduced Control**: While factory pattern promotes encapsulation and abstraction, it may also reduce the control that
  clients have over the creation process. Clients relying on a factory may have limited control over the specific
  attributes or configurations of the created objects.
- **Dependency Inversion Principle** (DIP): In some cases, the use of factory pattern may violate the Dependency
  Inversion Principle, especially if the factory class becomes a high-level module depending on low-level modules (the
  concrete classes being created).
- **Increased Complexity of Testing**: Testing code that relies heavily on factory pattern may become more complex, as
  it may involve mocking or stubbing factory objects to isolate the behavior being tested.
