# LeapYearChecker
LeapYearChecker
import java.util.Scanner;

public class LeapYearChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите год: ");
        int year = scanner.nextInt();

        boolean isLeapYear = checkLeapYear(year);
        if (isLeapYear) {
            System.out.println("Год является високосным!");
        } else {
            System.out.println("Год не является високосным.");
        }
    }

    public static boolean checkLeapYear(int year) {
        return (year % 4 == 0 && year % 100 != 0) || (year % 400 == 0);
    }
}
