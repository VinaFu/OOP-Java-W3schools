# FundamentalsOOPJava

Object Orientation Promgram

-- w3schools

Syntax:

        1) new:
            To create an object of Main, specify the class name, followed by the object name, and use the keyword new: 
            Main myObj = new Main() // an object of Main()
        //  [original class] name = new [original name]
        
        2) final: 
            Avoid a variable from being overriden/changed. Not inherited by other classes.
            final class MyClass
            
        3) import:
            import java.util.XXX
            util - utility
        
        4) extends:
            a class want to inherit the attributes and methods from another class.
            class Car extends Vehicle
            
        5) static & public 
            static: it can be accessed without creating an object of the class         
            public: can only be accessed by objects; so u'll have a dot[.] 
        
                public class Main {
                  // Static method
                  static void myStaticMethod() {
                    System.out.println("Static methods can be called without creating objects");
                  }

                  // Public method
                  public void myPublicMethod() {
                    System.out.println("Public methods must be called by creating objects");
                  }

                  // Main method
                  public static void main(String[] args) {
                    myStaticMethod(); // Call the static method
                    // myPublicMethod(); This would compile an error

                    Main myObj = new Main(); // Create an object of Main
                    myObj.myPublicMethod(); // Call the public method on the object
                  }
                }
        
        6)
        
        
        7)
        this.name = name

Attributes:      class attributes are variables within a class
                An attribute is a named object with associated values

        A.1 Create a class called "Main" with two attributes: x and y:

                public class Main {
                  int x = 5;
                  int y = 3;
                }

        A.2 Multiple Objects
                
                public class Main {
                  int x = 5;

                  public static void main(String[] args) {
                    Main myObj1 = new Main();  // Object 1
                    Main myObj2 = new Main();  // Object 2
                    myObj2.x = 25;      // change the value of object 2
                    System.out.println(myObj1.x);  // Outputs 5
                    System.out.println(myObj2.x);  // Outputs 25
                  }
                }                     // always have .x in the end~ means u use the attribute


        A.3 Multiple Attributes - (object) use different attributes in one class
        
                public class Main {
                  String fname = "John";
                  String lname = "Doe";
                  int age = 24;        // class Main with three attributes

                  public static void main(String[] args) {
                    Main myObj = new Main();
                    System.out.println("Name: " + myObj.fname + " " + myObj.lname);
                    System.out.println("Age: " + myObj.age);
                  }
                }                      // object myObj use the fname/ lname via [.]
                
                
                
                
                
                
                
                

-----------------------------------------------------------------------

Something you already know:
(Pluralsight lesson)

  Objects:
    - State( data)
    - Behavior (method and functions)
  
   - Encapsulation and abstraction  
   - Inheritance and polymorphism
   - Interfaces and system design


Advantages - same with Python
  
    OOP is faster and easier to execute
    OOP provides a clear structure for the programs
    OOP helps to keep the Java code DRY "Don't Repeat Yourself", and makes the code easier to maintain, modify and debug
    OOP makes it possible to create full reusable applications with less code and shorter development time

 General Ideas:
  
      Class:
          Instances - a class is a template for objects, and an object is an instance of a class.
          
      has-a: belonging
      is- a: description
    
    
  
  Review Packages -- can be done in IntelliJ:
  
        1) go to src, right click to New;
        2) create class, name: com.pluralsight.NAME.Main
        3) copy original Main content into this one.
        
        why we need package? Java 中的包用于对相关类进行分组。将其视为文件目录中的文件夹。我们使用package来避免名称冲突，并编写更好的可维护代码。It's like creat a folder to wrap them. 
        ** use the backwards method:com. at the front
  
   Gernate
   
        Automatically change it into String.
        Right click in the comment line; choose Gernate; select toString; select the items you want.
        Then it automatically build a coding block.
        
        
high coupling 高耦合
  
  
