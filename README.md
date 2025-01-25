Palindromic pyramid pattern
The palindromic number are the number whose reverse is equal to the original number.

For example- 12321 is a original number whose reverse is same as the original number, that is 12321

So, here we learn how to print the pyramid pattern on palindromic number or word.

palindromic pattren
1. Write a program to print the following pattern.
Enter the row 5

    1
   121
  12321
 1234321
123454321
Working
Step 1- Initialize the there variable for the loop

Step 2- the first loop is for the the row, in how many row you want to print data.

Step 3- the second loop is for the spaces, the space print in the row from i to row-1.

Step 4- the third loop is for the the print element from i to row.

Step 5- print j.

Step 6. the forth loop is for print reverse number.

Step 7- print j.

Step 8. Stop.

C	JAVA
import java.util.Scanner;

public class Main
{
    public static void main(String[] args) 
    {
        int i,j;
        //Scanner class declaration
        Scanner sc = new Scanner(System.in);
        //input from user
        System.out.print("Enter the row");
        int row = sc.nextInt();
        //declare for loop for every new row
        for(i=1;i<=row;i++)
        {
            //this lopp is for the space
            for(j=i;j<=row;j++)
                System.out.print(" ");
            //this loop is for print number 1 to i
            for(j=1;j<=i;j++)
                System.out.print(j+"");
            //this loop is for the number in reverse order
            for(j=i-1;j>=1;j--)
                System.out.print(j+"");
            System.out.println();
         }
    }
}
2. Write a program to print the following pattern
Enter the row 5                                                                                                             

     A                                                                                                                     
    ABA                                                                                                                    
   ABCBA                                                                                                                   
  ABCDCBA                                                                                                                  
 ABCDEDCBA  
C	JAVA
import java.util.Scanner;
public class Main
{
      public static void main(String[] args) 
      {
          int i,j,k;
          //scanner class declaration          
          Scanner sc=new Scanner(System.in);
          //enter user input
          System.out.print("Enter the row");
          int row = sc.nextInt();
          //this loop is for the every new row
          for(i=1;i<=row;i++)
          {
              // this loop is for the space from i to row
              for(j=i;j<=row;j++)
                    System.out.print(" ");
              //this loop is for print alphabet A to (J+64)
              for(j=1;j<=i;j++)
                    System.out.print((char)(j+64)+"");
               // this loop is for the reverse order of alphabet
              for(k=i-1;k>=1;k--)
                    System.out.print((char)(k+64)+"");
              System.out.println();
           }
        }
}
