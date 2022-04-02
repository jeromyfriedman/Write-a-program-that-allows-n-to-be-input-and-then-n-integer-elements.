# Write-a-program-that-allows-n-to-be-input-and-then-n-integer-elements.
Write a program that allows n to be input, and then n integer elements.
import java.util.Scanner;
public class BaiTapJavaCoBan11
{
    public static void main(String[] args)
    {
       int n;
       int[] soNguyen;
       float ketQua = 0;
       Scanner sc = new Scanner(System.in);

       System.out.println("Enter n:");
       n = sc.nextInt();
       soNguyen = new int[n];
       for (int i = 0; i < n; i++)
       {
          System.out.println("Integer:");
          soNguyen[i] = sc.nextInt();
       }

       for (int i = 0; i < n; i++)
          ketQua += soNguyen[i];
          ketQua = ketQua/n;

       System.out.println("Average of integers is: " + ketQua);
    }
}
