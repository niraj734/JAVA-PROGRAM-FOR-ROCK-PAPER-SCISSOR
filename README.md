# JAVA-PROGRAM-FOR-ROCK-PAPER-SCISSOR
import java.util.Scanner;
public class LAB3HW1 
{
    public static void main(String[] args) 
    {
        int min=0;
        int max=2;
        Scanner sc=new Scanner(System.in);
        System.out.println("ENTER A NUMBER BETWEEN 0 to 2");
        int user=sc.nextInt();
        if (user==0) 
        {
            System.out.println("You are scissor");
        }
        else if (user==1) 
        {
            System.out.println("You are rock");
        }
        else if(user==2)
        {
            System.out.println("You are paper");
        }
        int com_user=(int)(Math.random()*(max-min+1))+min;
        if (com_user==0) 
        {
            System.out.println("Computer is scissor");
        }
        else if (com_user==1) 
            {
                System.out.println("Computer is rock");
            }
        else if (com_user==2) 
        {
            System.out.println("Computer is paper");
        }
        if (com_user==user) 
        {
            System.out.println("It's a draw");
        }
        else if (user==0 && com_user==2) 
        {
            System.out.println("You won");
        }
        else if(user==1 && com_user==0)
        {
            System.out.println("computer won");
        }
        else if(user==2 && com_user==1)
        {
            System.out.println("You won");
        }

        
    }
    
}
