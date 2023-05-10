## Software design patterns

### OOP Principles in Java
#### Encapsulation
Encapsulation is the practice of hiding the internal details of a class and exposing only the necessary functionality. It helps protect the internal state of an object and promotes modularity. In the car analogy, encapsulation hides all internal components under the hood, exposing only the steering wheel, which the user can control.

With encapsulation, the state of an instance can be changed or updated only through exposed methods or fields, while everything else remains hidden. In a fantasy football example, a League class may have private fields for teams, players, and the scoring system to prevent direct manipulation of these objects from outside the class.

#### Inheritance
Inheritance allows us to reuse code by creating a new class that inherits properties and methods from an existing class. For instance, a Team class could inherit from the Player class, allowing it to reuse code for getting and setting the team's name, city, and stadium, as well as adding and removing players from the team.

#### Polymorphism
Polymorphism allows multiple subclasses to inherit from the same base class while exhibiting different behaviors. For example, RunningBack and Quarterback subclasses could inherit from a Player class but implement different methods for calculating statistics, such as rushing yards for RunningBacks and passing yards for Quarterbacks.

Java supports two types of polymorphism:
##### Method Overloading (Static Polymorphism)
Method overloading is resolved during program compilation. There are two types of method overloads:
1. Changing the input argument type: Different methods can accept different parameter types, such as a method that takes a Quarterback and another that takes a RunningBack.
2. Changing the number of method arguments: Methods can have a varying number of arguments, such as adding yardage for completed plays.

##### Method Overriding (Dynamic Polymorphism)
Method overriding, also known as dynamic polymorphism, determines the method to be executed at runtime. For example, a completed pass could log the Quarterback's passing yards and the WideReceiver's receiving yards.

#### Abstraction
Abstraction involves creating a general, abstract class to represent common properties and behaviors of related classes. For instance, an abstract Player class can have methods for getting and setting the player's name, position, and team. These methods enable setting essential aspects of all players while hiding the implementation details from the users of the class.

Abstraction can be achieved in two ways:
1. Abstract class:
   * Cannot be instantiated.
   * Provides a common base class, like a Player class for all positions with properties such as name, position, team, and jersey number.
2. Interfaces:
   * A contract that defines a set of methods that must be implemented by any class that implements the interface.
   * Better suited for simpler objects since they can only define methods, not properties.
   * Allows multiple inheritance, unlike abstract classes.
#### Creational patterns
Singleton
Factory
### Singleton
##### Six Words
==Single Instance, private constructor, static method, resource management, concurrency, and enum type==
* A Java object that can only be instantiated once.
* It is a **Creational** Pattern.
* No matter where it's used, it is always the same object
* Useful for classes that represent resources that should only be accessed by one object at a time, such as a database connection or a file.
* Is created using a ==private== constructor, which prevents other classes from creating new instances of the singleton.
* Typically has a static method that returns the singleton instance. This method is used to get the singleton instance from other classes.
* Most common implementation is the enum type--because enums are implicitly serializable, thread-safe, and immutable.
* Most logging frameworks use a singleton logger, and so do objects that manage threadpools.
#### Pitfalls
Not thread-safe by default and  access to the classes instance needs to be synchronized 
#### How and when it's used

##### Common Cases
* In a application that requires access to resources by means of passing a token object, you could follow a singleton pattern. The following are some situations it is used
	1. Database connections
		1. Used to ensure only one db connection is open at a time to prevent resource leaks and race conditions
			1. Race conditions are bugs in a program that occur when the outcome of a computation depends on the sequence or timing of other uncontrollable events. can occur when two or more threads of execution are accessing the same resource at the same time. If the threads are not
		2. Files:
			1. Used to ensure only one file is open at a time to prevent data corruption and race conditions.
		3. Logging:
			1. Logging:
				1. Ensures only one logger is used so other messages aren't overwritten or lost
		4. Concurrency
			1. Ensure only one thread can access a resource at a time--again prevents race conditions.
##### Real-world examples
In a fantasy football application, you might use a singleton pattern to store league settings like number of teams, scoring system, draft date,  and other resources shared by multiple objects in the application. 
It can also be used to implement global objects like current user preferences and config settings that need to be accessed everywhere. 



#### Easy to implement
1. Create a private static variable to store the instance of the singleton.
	1. `private static Singleton instance;`
2. Create a private constructor to prevent instantiation of singleton from outside the class
	1. `private Singleton() {}`
3. Create a public static method to get the instance of the singleton labled below
4. In new method check if null, create new instance if it is and return it, otherwise return existing instance
5. Make sure method is synchronized to prevent race conditions
```java
public class SingletonSafe {
  // Private static variable to store the instance of the singleton.
  private static Singleton instance;

  // Private constructor to prevent instantiation of the singleton from outside the class.
  private Singleton() {}
  
	//step 3
  // Paublic static method to get the instance of the singleton.
  public static Singleton getInstance() {
  //step 4
    // If the instance is null, create a new instance and return it
    if (instance == null) {
      instance = new Singleton();
    }

    // Return the instance.
    return instance;
  }
}
```
Next step
```java
//update method to ensure method is synchronizedd to prevent race conditions
public synchronized static Singleton getInstance() {
  if (instance == null) {
    instance = new Singleton();
  }

  return instance;
}
```


```java
public class NFLData {

    // Private constructor so that the class cannot be instantiated directly.
    private NFLData() {}

    // This static method returns the singleton instance of the class.
    public static NFLData getInstance() {
        return INSTANCE;
    }

    // Adds a new team to the list of teams.
    public void addTeam(Team team) {
        teams.add(team);
    }

    // Returns the list of teams.
    public List<Team> getTeams() {
        return teams;
    }

    // Private field that stores the list of teams.
    private final List<Team> teams = new ArrayList<>();

}

public class NFLLeague {

    // Stores the singleton instance NFLData class.
    private final NFLData data = NFLData.INSTANCE;

    // Adds a new team to the league.
    public void addTeam(Team team) {
        data.addTeam(team);
    }

    // Returns the list of teams in the league.
    public List<Team> getTeams() {
        return data.getTeams();
    }

}

public class Main {

    public static void main(String[] args) {

        NFLLeague league = new NFLLeague();

        // Add three teams to the league.
        league.addTeam(new Team("New England Patriots"));
        league.addTeam(new Team("Green Bay Packers"));
        league.addTeam(new Team("Kansas City Chiefs"));

        // Get the list of teams in the league.
        List<Team> teams = league.getTeams();

        for (Team team : teams) {
            System.out.println(team.getName());
        }
    }

}

```
d




### Abstraction
Software design pattern that provides an abstract way of creating objects. Responsible for creating objects of its associated types without exposing the creation logic to the client.


##### Six words
==Abstraction, Encapsulation, Polymorphism, Reusable==
#### Key details
* Creational pattern--like singleton.
* Used to abstract the creation of objects
* Allows you to create objects without knowing their concrete type
* Can be used to create objects of different types from a single factory class.
* Can be used to create immutable or thread-safe objects.
* Allows us to encapsulate the creation of objects and hide the details of how objects are created from the rest of the code.

#### Examples of how it's used
* To decouple object creation from rest of code
* To create objects of different types
* To achieve polymorphism
* For reusable code.

#### Examples of java implementations
*
*
*

#### Real world examples
*
*
*

#### Related concepts
##### Terms
Polymorphism
	The ability of an object to take many forms. Uses inheritance to inherit properties and methods from other objects--like say speak from an Animal class--and then allows the subclass to provide its own implementation of said method--like printing woof or meow. This allows us to call speak() to print the correct sound for the type of animal the object is without knowing what type it will be. 
Abstraction
	Hiding implementation details of an object from its users.
**Encapsulation:** 
	Grouping together related data and methods into a single unit. A factory class is responsible for creating and managing its own objects.

##### Concepts I should be able to differentiate it from
Builder Pattern
Singleton Pattern
Abstract Factory Pattern

#### Code example

```java
public class PlayerFactory {

    public Player createPlayer(String position) {
        if (position.equals("QB")) {
            return new Quarterback();
        } else if (position.equals("RB")) {
            return new RunningBack();
        } else if (position.equals("WR")) {
            return new WideReceiver();
        } else if (position.equals("TE")) {
            return new TightEnd();
        } else {
            throw new IllegalArgumentException("Invalid player position");
        }
    }
}

	//Use it to create a new quarterback
	PlayerFactory factory = new PlayerFactory();
	Player player = factory.createPlayer("QB");


```



