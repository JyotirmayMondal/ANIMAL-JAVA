Java OOP Assignment: Animal Inheritance System
----------------------------------------------

📌 Objective:
-------------
To demonstrate the use of Object-Oriented Programming concepts in Java:
- Abstract classes
- Inheritance
- Polymorphism
- Interfaces
- UML diagram representation

📂 Project Structure:
---------------------
The project includes the following classes and interface:

1. Animal.java (Abstract Class)
   - Attributes: name (String), age (int)
   - Abstract Method: makeSound()
   - Concrete Methods: getName(), getAge()

2. Dog.java (Class)
   - Extends: Animal
   - Implements: Pet
   - Additional Attribute: breed (String)
   - Methods: makeSound(), displayBreed(), play()

3. Cat.java (Class)
   - Extends: Animal
   - Implements: Pet
   - Additional Attribute: color (String)
   - Methods: makeSound(), displayColor(), play()

4. Pet.java (Interface)
   - Method: play()

5. AnimalTest.java (Tester Class)
   - Contains main() method
   - Creates Dog and Cat objects
   - Demonstrates polymorphism via Animal[] array
   - Calls makeSound(), play(), and specific attribute display methods

📈 UML Diagram:
---------------
The UML diagram shows the relationship between:
- `Animal` as an abstract superclass
- `Dog` and `Cat` as subclasses that also implement the `Pet` interface
- `AnimalTest` class that uses `Dog` and `Cat` objects
(See UML_diagram.png if included)

🛠️ How to Run:
---------------
1. Compile all `.java` files:
   javac *.java

2. Run the tester class:
   java AnimalTest

📤 Output:
----------
- Displays name and age of each animal
- Outputs each animal's sound (polymorphic behavior)
- Shows breed/color via class-specific methods
- Demonstrates play() method from Pet interface

🧠 Notes:
---------
- The `makeSound()` method is abstract in `Animal`, so each subclass must override it.
- The `play()` method is defined in the `Pet` interface and implemented in `Dog` and `Cat`.
- `instanceof` is used in the tester class to safely access subclass-specific methods.

📅 Author:
----------
Jyotirmay Mondal
Date: 09-05-2025
