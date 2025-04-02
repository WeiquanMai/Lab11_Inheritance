/*
 * CSC-239 Java
 * Project Name: Inheritance
 * Student: Weiquan Mai
 * Date: March 18, 2025
 * Description: Project utilizes inheritance to create class NewPoint from class MyPoint, and then calculates the distance between NewPoint, and MyPoint.
 */

public class MyPoint {
    double x, y;
    
    // No-arg constructors
    public MyPoint(){
        this.x = 0;
        this.y = 0;
    }
    
    // Constructor with arguments
    public MyPoint(double xValue, double yValue){
        this.x = xValue;
        this.y = yValue;
    }

    // Accessors
    public double getX(){
        return x;
    }
    public double getY(){
        return y;
    }
    
    // Returns distance from this point to another point with specified x,y coordinates
    public double distance(double xValue, double yValue){
        double distance = Math.sqrt(Math.pow(this.x - xValue,2) + Math.pow (this.y - yValue, 2));
        return distance;
    }

    // Returns distance from this point to another object of MyPoint type
    public double distance(MyPoint otherPoint){
        double distance = Math.sqrt(Math.pow(this.x - otherPoint.x ,2) + Math.pow(this.y - otherPoint.y, 2));
        return distance;
    }
} // End of class MyPoint

class NewPoint extends MyPoint{
    private static int numberOfObjects = 0;

    // No-arg constructor
    public NewPoint(){
        x = 0;
        y = 0;
        numberOfObjects++;
    }

    // Constructor with arguments
    public NewPoint(double xValue, double yValue){
        x = xValue;
        y = yValue;
        numberOfObjects++;
    }

    // Return numberOfObjects created so far
    public static int getNumberOfObjects(){
        return numberOfObjects;
    }
} // End of class NewPoint
