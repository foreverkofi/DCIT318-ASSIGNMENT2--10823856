using System;

// Base class Animal
class Animal
{
    // Method that prints a generic sound
    public virtual void MakeSound()
    {
        Console.WriteLine("Some generic sound");
    }
}

// Derived class Dog inheriting from Animal
class Dog : Animal
{
    // Override the MakeSound method to print "Bark"
    public override void MakeSound()
    {
        Console.WriteLine("Bark");
    }
}

// Derived class Cat inheriting from Animal
class Cat : Animal
{
    // Override the MakeSound method to print "Meow"
    public override void MakeSound()
    {
        Console.WriteLine("Meow");
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Create an instance of Animal
        Animal animal = new Animal();
        Console.WriteLine("Animal sounds:");
        animal.MakeSound();  // Output: Some generic sound

        // Create an instance of Dog
        Dog dog = new Dog();
        Console.WriteLine("\nDog sounds:");
        dog.MakeSound();     // Output: Bark

        // Create an instance of Cat
        Cat cat = new Cat();
        Console.WriteLine("\nCat sounds:");
        cat.MakeSound();     // Output: Meow
    }
}