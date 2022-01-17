# FINDINGODDNUMBERS
this code will loops through given rage or numbers and print them out then sum them and return the sum of all all numbers. 

public class SumOddRange {

    public static boolean isOdd(int number) {
        if (number < 0) {
            return false;
        }
        return (number % 2 != 0);

    }

    public static int sumOdd(int start, int end) {

        int sum = 0;
        if(end >= start && start > 0) {

            for(int i = start; i <= end; i++) {
                if(isOdd(i)) {
                    sum = sum + i;   
                    System.out.println(i);    /* you don't have to add these codes
                    if (i == 101 || i == 97 || i == 201 || i == 701) {
                        System.out.println("HOLD ON! FETCHING MORE ODD NUMBERS..."); *\
                    }
        }

            }
            return sum ;

        }
        return -1;


    }

    public static void main(String[] args) {
        System.out.println(isOdd(3));
        System.out.println(sumOdd(200, 1000));
    }

}
