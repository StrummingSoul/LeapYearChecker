public class LeapYearChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Введите год: ");
        int year = scanner.nextInt();

        boolean isLeapYear = checkLeapYear(year);
        if (isLeapYear) {
            System.out.println("Год является високосным!");
