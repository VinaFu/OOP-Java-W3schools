# FundamentalsOOPJava

Object Orientation Promgram

-- w3schools

Common sense: 

        C1. parentheses - 括号(); semicolon (;)
        C2. out-> till class -> cmd -> "java Main": run in the terminal
            src-> till class -> packages: manually in same folder com.pluralsight.projectName.Main(Othername)

Keywords: see more in modifiers

        1) new:
            How to create an object
            Main myObj = new Main() // an object of Main()
                //    Main myObj = new Main() 
                // [class] objName = new [class] for public class, see below
        
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
            
            5.0) Example for static & private
            
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
                    myStaticMethod(); // Call the static method; no dot
                    
                    Main myObj = new Main(); // Create an object of Main
                    myObj.myPublicMethod(); // Call the public method on the object
                  }
                }
        
            5.1) Access Methods With an Object
                Example Requirements:" Create a Car object named myCar. Call the fullThrottle() and speed() methods on the myCar object, and run the program "
                
                public class Main { // class Name same with the filename = Capitalize
                
                    // build the methods in class
                    public void fullThrottle(){  // method 1
                        System.out.println("This is fullThrottle!");
                    }          
                    public void speed(int maxSpeed){        // method 2 + define parameter and type
                        System.out.println("The max speed is " + maxSpeed + "!");
                    }           

                    // build object to use the methods from class 
                    public static void main(String[] args) { // call the methods in object
                        Main myCar = new Main();        // call from the attributes
                        myCar.fullThrottle();
                        myCar.speed(350);
                        }
                    }
                                                            Outcome:
                                                                This is fullThrottle!
                                                                The max speed is 350!

            5.2) Using Multiple Classes - Essential for OOP
                如果您在不同的页面中有Classes，您仍然可以在不同的页面中使用它们;
                必须确保这些页面在相同的文件下（手动），或者在terminal使用 javac 
                Example Above
                
                [ Main.java ] - one page
                
                        public class Main {
                          public void fullThrottle() {
                            System.out.println("The car is going as fast as it can!");
                          }

                          public void speed(int maxSpeed) {
                            System.out.println("Max speed is: " + maxSpeed);
                          }
                        }         // Null print or return

                [ Second.java ] - another page
                        class Second {
                          public static void main(String[] args) {
                            Main myCar = new Main();     
                            myCar.fullThrottle();      
                            myCar.speed(200);          
                          }
                        }         // call the methods here, so run it, u get the outcomes
            
                                                            Outcome:
                                                                This is fullThrottle!
                                                                The max speed is 200!
            
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
  
  
