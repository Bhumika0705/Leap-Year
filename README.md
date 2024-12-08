# Leap-Year
In this get to know that weather the  year is leap or not which you had given to the code itself
import java.util.Scanner;

public class Leapyear {
    public Leapyear() {
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the year:");
        int year = sc.nextInt();
        System.out.println(Is_leapyear(year));
    }

    public static boolean Is_leapyear(int y) {
        boolean a = y % 4 == 0;
        boolean b = y % 100 == 0 && y % 400 == 0;
        return a && b;
    }
}
