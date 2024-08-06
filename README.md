  <p align="center">
    <img src="resources/media/m1.PNG" alt="Image description" style="width:100%; height:100%;">
  </p>

## Section 1: Notes

### Basics of Classes

- A class is a blueprint for creating objects.
- A class defines attributes (fields/variables) and methods (functions) that describe the behavior of the objects created from the class.
- Example:
  ```java
  public class Car {
      // Attributes
      String color;
      String model;
      int year;
      
      // Methods
      void drive() {
          System.out.println("The car is driving");
      }
  }
  
# Visibility Levels

- public: Accessible from any other class.
- private: Accessible only within the same class.
- protected: Accessible within the same package and subclasses.
- default (no modifier): Accessible only within the same package.

```
    java
    Copy code
    public class Car {
        public String color;
        private String model;
        protected int year;
        int speed; // default
    }
```

# Attributes
- Variables that hold the data associated with an object.
- Declared within a class but outside any method.

```
    java
    Copy code
    public class Car {
        String color; // attribute
        String model; // attribute
    }

```
# Operations (Methods)

- Functions that define the behavior of objects.
- Can be used to perform operations, return values, or modify object state.

```
java
Copy code
public class Car {
    void drive() {
        System.out.println("The car is driving");
    }
}

```
# Creating Objects and Accessing Variables

- Objects are instances of classes.
- Use the new keyword to create an object.
- Access attributes and methods using the dot . operator.

  ```
    java
    Copy code
    public class Car {
        String color;
        String model;
        
        void drive() {
            System.out.println("The car is driving");
        }
        
        public static void main(String[] args) {
            Car myCar = new Car(); 
            myCar.color = "Red";
            myCar.model = "Toyota";
            System.out.println(myCar.color); // Outputs: Red
            myCar.drive(); // Outputs: The car is driving
        }
    }
```

# Getters and Setters

- Methods that provide access to private attributes.
- Getters return the value of a private attribute.
- Setters allow modifying the value of a private attribute.
   
```
    java
    Copy code
    public class Car {
        private String color;
        private String model;
        
        // Getter for color
        public String getColor() {
            return color;
        }
        
        // Setter for color
        public void setColor(String color) {
            this.color = color;
        }
        
        // Getter for model
        public String getModel() {
            return model;
        }
        
        // Setter for model
        public void setModel(String model) {
            this.model = model;
        }
    }

```

## Section 2: Basic Guided Questions

1. **Creating a Class and Objects:**
   - Write a class `Dog` with attributes `name` and `breed`.
   - Write a method `bark()` that prints "Woof!".
   - Create an object of the class and call the `bark()` method.

2. **Using Visibility Levels:**
   - Modify the `Dog` class to have `name` as public and `breed` as private.
   - Add a method `getBreed()` to return the breed.
   - Try accessing `breed` directly from another class and observe the result.
   - **Explanation Required:** Explain why `breed` cannot be accessed directly and how the `getBreed()` method allows access.
   - Create a class `Person` with the following attributes and methods:
     - `private String name`
     - `protected int age`
     - `public String getName()`
     - `public void setName(String name)`
     - `protected void setAge(int age)`
   - Try accessing the attributes and methods of the `Person` class from another class in the same package and from a different package.
   - **Explanation Required:** Explain the access levels for each visibility modifier when accessing the `Person` class attributes and methods.

3. **Visibility Check for Classes and Methods in Packages:**
   - Create a package `mypackage` and a class `Person` inside it.
   - Create another class `TestPerson` in the same package and try accessing the `Person` class.
   - Create another package `anotherpackage` and a class `TestPersonInAnotherPackage` inside it. Try accessing the `Person` class from this new class.
   - **Explanation Required:** Explain the class access levels within and across packages.

4. **Using Getters and Setters:**
   - Modify the `Book` class to make the attributes `title` and `author` private.
   - Add getters and setters for these attributes.
   - Try accessing the private attributes directly and explain the result.
   - **Explanation Required:** Explain the purpose of getters and setters and how they provide controlled access to private attributes.




