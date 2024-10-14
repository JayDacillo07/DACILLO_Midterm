// Base class: Person
class Person {
    // Fields
    String name;
    int age;

    //  initializing name and age
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    //  displaying information
    public void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}

// Subclass: Student
class Student extends Person {
    //  Student
    String studentID;
    String course;
    int units;
    final int feePerUnit = 1000; // Fixed fee per unit

    //  initializing student details
    public Student(String name, int age, String studentID, String course, int units) {
        super(name, age); // Calling the constructor of the parent class (Person)
        this.studentID = studentID;
        this.course = course;
        this.units = units;
    }

    //  calculating total fee based on units
    public double calculateFees() {
        return units * feePerUnit;
    }

    // Overriding displayInfo() method to include student-specific details
    @Override
    public void displayInfo() {
        super.displayInfo(); // Displaying Person details
        System.out.println("Student ID: " + studentID);
        System.out.println("Course: " + course);
        System.out.println("Units: " + units);
        System.out.println("Total Fee: " + calculateFees());
    }
}

// Subclass: Instructor
class Instructor extends Person {
    //  Instructor
    String employeeID;
    String department;
    double salary;

    // initializing instructor details
    public Instructor(String name, int age, String employeeID, String department, double salary) {
        super(name, age); // Calling the constructor of the parent class (Person)
        this.employeeID = employeeID;
        this.department = department;
        this.salary = salary;
    }

    // Overriding displayInfo() method to include instructor-specific details
    @Override
    public void displayInfo() {
        super.displayInfo(); // Displaying Person details
        System.out.println("Employee ID: " + employeeID);
        System.out.println("Department: " + department);
        System.out.println("Salary: " + salary);
    }
}

// Main class to test the system
public class UniversityEnrolmentSystem {
    
    // Polymorphic method to print details of any Person (Student or Instructor)
    public static void printDetails(Person p) {
        p.displayInfo(); // Calls the appropriate displayInfo() method based on the object's type
    }

    public static void main(String[] args) {
        // Creating two Student objects
        Student student1 = new Student("Jay", 20, "231000326", "Computer Engineering", 21);
        Student student2 = new Student("James", 20, "231000341", "Computer Engineering", 19);

        // Creating two Instructor objects
        Instructor instructor1 = new Instructor(" Mr. Velitario", 35, "12345", " College of Engineering and Architecture", 12000);
        Instructor instructor2 = new Instructor("Mr. Bargo", 29, "12345", "College of Engineering and Architecture", 10000);

        // Using printDetails method to display information for each person
        System.out.println("Student 1:");
        printDetails(student1);
        System.out.println();

        System.out.println("Student 2:");
        printDetails(student2);
        System.out.println();

        System.out.println("Instructor 1:");
        printDetails(instructor1);
        System.out.println();

        System.out.println("Instructor 2:");
        printDetails(instructor2);
    }
}
