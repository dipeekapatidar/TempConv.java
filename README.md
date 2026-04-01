import java.util.Scanner;

public class TempConv {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Temperature Converter");
        System.out.println("1. Celsius to Fahrenheit");
        System.out.println("2. Fahrenheit to Celsius");
        System.out.println("3. Celsius to Kelvin");
        System.out.println("4. Kelvin to Celsius");

        System.out.print("Enter your choice: ");
        int choice = sc.nextInt();

        double temp, result;

        switch(choice) {
            case 1:
                System.out.print("Enter temperature in Celsius: ");
                temp = sc.nextDouble();
                result = (temp * 9/5) + 32;
                System.out.println("Fahrenheit: " + result);
                break;

            case 2:
                System.out.print("Enter temperature in Fahrenheit: ");
                temp = sc.nextDouble();
                result = (temp - 32) * 5/9;
                System.out.println("Celsius: " + result);
                break;

            case 3:
                System.out.print("Enter temperature in Celsius: ");
                temp = sc.nextDouble();
                result = temp + 273.15;
                System.out.println("Kelvin: " + result);
                break;

            case 4:
                System.out.print("Enter temperature in Kelvin: ");
                temp = sc.nextDouble();
                result = temp - 273.15;
                System.out.println("Celsius: " + result);
                break;

            default:
                System.out.println("Invalid choice!");
        }
Added TempConv.java
        sc.close();
    }
}
