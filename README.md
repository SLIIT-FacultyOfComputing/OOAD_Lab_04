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
`` `

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

