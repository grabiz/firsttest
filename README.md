
package exercise;

import java.util.Scanner;

public class Exercise {
   
    public static void main(String[] args) {
   
        System.out.println("Nhap vao hai so nguyen :");
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        Scanner sc1 = new Scanner(System.in);
        int b = sc1.nextInt();
        System.out.println("So lon nhat la :" +solonnhat(a,b));
        
        System.out.println("Nhap vao so tu nhien : ");
        Scanner sc2 = new Scanner(System.in);
        int n= sc2.nextInt();
        System.out.println("He nhi phan la : " +doinhiphan(n));
        
        System.out.println("Nhap vao so tu nhien : ");
        Scanner sc3 = new Scanner(System.in);
        int m = sc3.nextInt();
        System.out.println("He nhi phan la : " +daoso(m));
    }
    public static int solonnhat(int a, int b)
           {
               if (a>b) return a;
               else return b;
           }
    public static int doinhiphan(int n)
           {   
               
           }
    public static int daoso(int n)
           {   
               int reserve = 0;
               while (n/10!=0)
                   {
                     reserve=reserve*10+(n%10);
                     n=n/10;                        
                   }
               return reserve;
           }
}
