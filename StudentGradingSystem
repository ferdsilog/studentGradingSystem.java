import java.util.Scanner;

public class StudentGradingSystem {
    public static void main(String[] args) {
        int numOfSubjects = 8;
        String[] subjects = {"Math", "Programming", "Intro to Computing", "Discrete Math", "Accounting for IT"
                , "Fundamentals of Algorithm", "Physical Education: Karate", "ROTC"};
        float[] grades = new float[8];
        float totalGrades = 0;
        double average = 0;

     //Input student name and grades
     //Compute average
     //Determine Pass/Fail
     //Display summary

        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter your name: ");
        String name = scanner.nextLine();

        System.out.println("---Student Grading System---");


        for (int i = 0; i < numOfSubjects; i++) {
            float input = -1;

            while (input < 0 || input > 100) {
                System.out.print("Enter your grade in " + subjects[i] + " (0-100): ");
                input = scanner.nextFloat();
                scanner.nextLine();
                if (input < 0 || input > 100) {
                    System.out.println("Invalid grade! Please enter a number between 0 and 100.");
                }
            }
            grades[i] = input;
            totalGrades += input;
        }

        System.out.println("---Summary-----");
        System.out.println("Name : " + name );
        for (int i = 0; i < numOfSubjects; i++) {
            System.out.println(subjects[i] + ": " + grades[i]);
        }
        average = totalGrades / numOfSubjects;

        System.out.println("Average: " + average);
        System.out.print("Status: ");
        if (average >= 75) {
            System.out.println("You Passed");
        } else {
            System.out.println("You Failed");
        }
        System.out.print("Remarks: ");
        if (average == 100) {
            System.out.println("Perfect!");
        } else if (average > 96 && average < 100) {
            System.out.println("You are a genius!");
        } else if (average > 92 && average < 97) {
            System.out.println("Excellent!");
        } else if (average > 88 && average < 93) {
            System.out.println("Amazing");
        } else if (average > 84 && average < 89) {
            System.out.println("Very Good");
        } else if (average > 79 && average < 86) {
            System.out.println("Good");
        } else if (average >= 75 && average < 80) {
            System.out.println("Fair");
        } else {
            System.out.println("Better Luck Next Time!");
        }

        scanner.close();
    }
}
