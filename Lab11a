/*
 * CSC-239 JAVA
 * Project Name: Inheritance
 * Student: Weiquan Mai
 * Date: March 18, 2025
 * Description: Project utilizes inheritance to create class NewPoint from class MyPoint, and then calculates the distance between NewPoint, and MyPoint.
 */

import java.util.Scanner;

public class Lab11a {
    public static void main(String[] args){
        // Create a scanner
        Scanner input = new Scanner(System.in);

        // Create an object of NewPoint
        NewPoint obj = new NewPoint();

        // Variables
        boolean keepRunning = true;
        String buffer;
        String [] coordinates = new String[2];

        while(keepRunning){
            System.out.print("Enter x and y coordinates for point 1 (or q to exit): ");
            buffer = input.nextLine();

            if (buffer.equalsIgnoreCase("q")){
                keepRunning = false;
                break;
            }
            // Obtain coordinate points from user input
            coordinates = buffer.split(" ");
            double x1 = Double.parseDouble(coordinates[0]);
            double y1 = Double.parseDouble(coordinates[1]);
            NewPoint Point1 = new NewPoint (x1, y1);

            // Obtain second coordinate points from user input
            System.out.print("Enter x and y coordinates for point 2 (or q to exit): ");
            buffer = input.nextLine();
            coordinates = buffer.split(" ");
            double x2 = Double.parseDouble(coordinates[0]);
            double y2 = Double.parseDouble(coordinates[1]);
            NewPoint Point2 = new NewPoint (x2, y2);

            // Calculate distances
            double distanceObjectToObject = Point2.distance(Point1);
            double distanceObjectToCoordinates = Point2.distance(x1,y1);

            //Obtain numberOfObjects
            int numObjects = (Point2.getNumberOfObjects() - 1);

            // Display data
            System.out.println("p1 =(" + x1 + "," + y1 + "), p2=(" + x2 + "," + y2 + "), numberOfObjects=" + numObjects);
            System.out.printf("Distance (object to object)          = %.4f\n", distanceObjectToObject);
            System.out.printf("Distance (object to X,Y coordinates) = %.4f\n", distanceObjectToCoordinates);
        }

        // Close scanner
        input.close();
        System.out.print("Exiting the program...");
    } // End of main method
}
