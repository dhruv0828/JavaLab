// Abstract class
abstract class Shape {
    // Abstract methods (to be implemented by subclasses)
    abstract double calculateArea();
    abstract double calculatePerimeter();

    // Concrete method
    void displayDetails() {
        System.out.println("Shape details:");
        System.out.println("Area: " + calculateArea());
        System.out.println("Perimeter: " + calculatePerimeter());
    }
}

// Concrete subclass 1
class Circle extends Shape {
    private double radius;

    // Constructor
    Circle(double radius) {
        this.radius = radius;
    }

    // Implementing abstract methods
    @Override
    double calculateArea() {
        return Math.PI * radius * radius;
    }

    @Override
    double calculatePerimeter() {
        return 2 * Math.PI * radius;
    }
}

// Concrete subclass 2
class Rectangle extends Shape {
    private double length;
    private double width;

    // Constructor
    Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }

    // Implementing abstract methods
    @Override
    double calculateArea() {
        return length * width;
    }

    @Override
    double calculatePerimeter() {
        return 2 * (length + width);
    }
}

public class ShapeDemo {
    public static void main(String[] args) {
        System.out.println("Kumari Priya 079");

        // Creating objects of concrete subclasses
        Circle circle = new Circle(5.0);
        Rectangle rectangle = new Rectangle(4.0, 6.0);

        // Using abstract class reference to refer to concrete objects
        Shape shape1 = circle;
        Shape shape2 = rectangle;

        // Calling methods
        shape1.displayDetails();
        System.out.println("--------------------------");
        shape2.displayDetails();
    }
}
