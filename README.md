package javaapplication5;

interface Shape {
    double calculateArea();
}

public class JavaApplication5 {
    public static void main(String[] args) {
        Shape circle = () -> {
            double radius = 5;
            return Math.PI * radius * radius;
        };

        Shape rectangle = () -> {
            double length = 4, width = 6;
            return length * width;
        };

        Shape square = () -> {
            double side = 4;
            return side * side;
        };

        Shape triangle = () -> {
            double base = 3, height = 5;
            return 0.5 * base * height;
        };

        System.out.println("Circle Area: " + circle.calculateArea());
        System.out.println("Rectangle Area: " + rectangle.calculateArea());
        System.out.println("Square Area: " + square.calculateArea());
        System.out.println("Triangle Area: " + triangle.calculateArea());
    }
}

out put
run:
Circle Area: 78.53981633974483
Rectangle Area: 24.0
Square Area: 16.0
Triangle Area: 7.5
BUILD SUCCESSFUL (total time: 0 seconds)
# run-time-polymorphism
