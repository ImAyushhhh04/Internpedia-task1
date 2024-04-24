# Internpedia-task1
# Student Grade calculator
#code:
import java.util.Scanner;

public class GradeCalculator {
    public static void main(String args[]) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Enter the number of subjects:");
        int numSubjects = scanner.nextInt();

        int[] marks = new int[numSubjects];
        int totalMarks = 0;

        System.out.println("Enter the marks obtained in each subject (out of 100):");
        for (int i = 0; i < numSubjects; i++) {
            System.out.print("Subject " + (i + 1) + ": ");
            marks[i] = scanner.nextInt();
            totalMarks += marks[i];
        }

        int averagePercentage = totalMarks / numSubjects;

        String grade = calculateGrade(averagePercentage);

        System.out.println("\nResults:");
        System.out.println("Total Marks: " + totalMarks);
        System.out.println("Average Percentage: " + averagePercentage + "%");
        System.out.println("Grade: " + grade);

        scanner.close();
    }

    public static String calculateGrade(int averagePercentage) {
        if (averagePercentage = 100) {
            return "A+";
        } else if (averagePercentage = 90) {
            return "A";
        } else if (averagePercentage = 80) {
         

   return "B";
        } else if (averagePercentage = 70) {
            return "C";
        } else if (averagePercentage 	= 60) {
            return "D";
        } else {
            return "F";
        }
    }
}

