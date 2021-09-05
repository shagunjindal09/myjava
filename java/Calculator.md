# calculator
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
		
	    Scanner sc = new Scanner(System.in);
      
	    double a,b;
      
	    double output;
      
	    System.out.println("enter two numbers");
      
	    a=sc.nextDouble();
      
	    b=sc.nextDouble();
      
	    System.out.println("enter an operator");
      
	    char operator=sc.next().charAt(0);
      
	    switch(operator){
      
	        case '+':
          
	        output=a+b;
          
	        //System.out.println(output);
	        break;
          
	        case '-':
          
	        output=a-b;
          
	        //System.out.println(output);
	        break;
	        
	        case '*':
	        output=a*b;
	       // System.out.println(output);
	        break;
	        case '/':
	        output=a/b;
	       // System.out.println(output);
	        break;
	        default:
	        System.out.println("you entered an wrong operator");
	        return;
	    }
	    System.out.println(a+" "+operator+" "+b+" :" +output);
	}
}
