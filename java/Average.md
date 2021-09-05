# average of some subject marks
import java.util.Scanner;

public class Main
{
	public static void main(String[] args) {
  
	byte m1,m2,m3;
  
	Scanner sc = new Scanner(System.in);
  
		System.out.println("enter your physics marks");
    
	m1=sc.nextByte();
  
System.out.println("enter ur chemistry marks");

		m2=sc.nextByte();
    
		System.out.println("enter ur maths marks");

		m3=sc.nextByte();
    
    
	float avg= (m1+m2+m3)/3f;
  
	System.out.println(avg);
  
	if(avg>=44 && m1>=33 && m2>=33 && m3>=33)
  
	System.out.println("congratulation you are passed");
  
	else
  
	System.out.println("u are failed");
	}
}
