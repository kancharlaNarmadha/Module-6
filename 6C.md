
# EX 6A Inner Class
## DATE:
## AIM:
to write a Java Program using Method Local Inner Class for below Scenario.

Create a class "Department" with

1. String value "Financial and Management Department"

2. Create display() have String "ABC Industries" and inner class as "Inner"

3. Inner class  print() to display department

In main() access all function using its corresponding Object.

Note:

read the input value in string format.














## Algorithm

1.Create a class prog with an instance variable dept and a method display().

2.Inside the display() method, declare a local variable company.

3.Define a local inner class Inner inside the display() method.

4.In the Inner class, define a method print() that prints both dept and company.

5.In main(), create an object of prog and call the display() method.1.





## Program:

Developed by: Kancharla Narmadha
Register Number: 212222110016
```
class prog {
    String dept = "Financial and Management Department";

    void display() {
        String company = "ABC Industries";

        class Inner {
            void print() {
                System.out.println("Department is " + dept);
                System.out.println("Company is " + company);
            }
        }

        Inner obj = new Inner();
        obj.print();
    }

    public static void main(String[] args) {
        prog d = new prog();
        d.display();
    }
}



    
```

## Output:
![image](https://github.com/user-attachments/assets/3d63bd02-8c51-44e2-85d0-c0fa83f75410)


## Result:
The program successfully demonstrates the concept of a local inner class, where the inner class accesses both the outer class member and the local variable from the method in which it's defined.



