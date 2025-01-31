Diamond number pattern printing
In this section, we learn about  Diamond numbers pattern printing. Here we will see how to use loops to print the numbers starting from 1 up to N in the form of diamond. the diamond will be made using two triangles one triangle will be printed by one loop and other by another loop.  Both the triangles in Diamond numbers pattern printing are opposite from each other that why we need to take two loop for print diamond pattern. 

diamond number pattern
1. Write a program to print the following pattern
Enter the number of row 5

    1
   123
  12345
 1234567
123456789
 1234567
  12345
   123
    1
Working
Step 1- Initialize first outer loop for the print the first pyramid, this loop work from 1 to row.

Step 2- Now we need two loop inside the outer loop .

Step 3- The first inner loop work on printing space, so this loop work from 1 to n-i, because we need to reduce space after every row.

Step 4- The second inner loop work on the printing number, so it will start from 1 to 2*i-1, because we need to increment number with 2 in every row.

Step 5- Now initialize second outer loop which is work for the second opposite pyramid.this loop start from row-1 to 1

Step 6 – The inner loop of the second pyramid work same as the first outer loop.

Step 7- Stop. 

 

C	JAVA	Python
import java.util.Scanner;
public class Main
{
      public static void main(String[] args)
      {
           Scanner sc=new Scanner(System.in);
           System.out.print("Enter the number of row ");
           int n=sc.nextInt(); 
           //declaration first outer for loop for print the first number pyramid
           for(int i=1;i<=n;i++)
           {
                //declare inner loop for print the spaces
                for(int j=1;j<=n-i;j++)
                {
                       System.out.print(" ");
                }
                //declare inner loop for print the number
                for(int j=1;j<=i*2-1;j++)
                {
                      //here we print j, here j print different number in a row
                       System.out.print(j);
                }
                System.out.println();
            } 
            //declare second outer loop for printing opposite number pyramid
            for(int i=n-1;i>0;i--)
            {
                  //declare inner loop for print the spaces
                  for(int j=1;j<=n-i;j++)
                  {
                         System.out.print(" ");
                  }
                  //declare inner loop for print the number
                  for(int j=1;j<=i*2-1;j++)
                  {
                         System.out.print(j);
                  }
                  System.out.println();
             }
       }
}
2. Write a program to print the following pattern
Enter the number of row 5

    1
   222
  33333
 4444444
555555555
 4444444
  33333
   222
    1
C	JAVA	Python
import java.util.Scanner;
public class Main
{
      public static void main(String[] args)
      {
           Scanner sc=new Scanner(System.in);
           System.out.print("Enter the number of row ");
           int n=sc.nextInt(); 
           //declaration first outer for loop for print the first number pyramid
           for(int i=1;i<=n;i++)
           {
                //declare inner loop for print the spaces
                for(int j=1;j<=n-i;j++)
                {
                       System.out.print(" ");
                }
                //declare inner loop for print the number
                for(int j=1;j<=i*2-1;j++)
                {
                      //here we print i, here  print same number in a row
                       System.out.print(i);
                }
                System.out.println();
            } 
            //declare second outer loop for printing opposite number pyramid
            for(int i=n-1;i>0;i--)
            {
                  //declare inner loop for print the spaces
                  for(int j=1;j<=n-i;j++)
                  {
                         System.out.print(" ");
                  }
                  //declare inner loop for print the number
                  for(int j=1;j<=i*2-1;j++)
                  {
                         System.out.print(i);
                  }
                  System.out.println();
             }
       }
}
