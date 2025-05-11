// Base class
class Animal {
    // Properties
    String name;

    // Constructor
    public Animal(String name) {
        this.name = name;
    }

    // Method
    public void eat() {
        System.out.println(name + " is eating.");
    }
}

class Dog extends Animal {
    // Constructor
    public Dog(String name) {
        super(name);
    }

    public void bark() {
        System.out.println(name + " is barking.");
    }
}

public class InheritanceDemo {
    public static void main(String[] args) {
        System.out.println("Kumari Priya 079");
        Animal animal = new Animal("Generic Animal");
        animal.eat();

        System.out.println("--------------------------");
        Dog dog = new Dog("Buddy");
        dog.eat();  // Inherited method from Animal class
        dog.bark(); // Method specific to Dog class
    }
}
