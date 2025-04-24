//Find the missing number in an array from 1 to n , in java

public class MissingNumber {
    public static int findMissingNumber(int[] arr, int n) {
        int total = n * (n + 1) / 2; // Sum of 1 to n
        int sum = 0;
        for (int num : arr) {
            sum += num;
        }
        return total - sum;
    }

    public static void main(String[] args) {
        int[] arr = {1, 2, 4, 5, 6}; // Missing 3
        int n = 6;
        int missing = findMissingNumber(arr, n);
        System.out.println("Missing number is: " + missing);
    }
}
