# game of choosing rock paper and scissor
import java.util.Scanner;

import java.util.Random;

public class Main
{
	public static void main(String[] args) {
  
		Scanner sc = new Scanner(System.in);
    
		System.out.print("Enter 0 for rock,1 for paper,2 for scissor");
    
		int userInput = sc.nextInt();
    
		Random random = new Random();
    
		int computerInput = random.nextInt( 3);
    
		if(userInput==computerInput){
    
		    System.out.println("Draw");
		}
		else if(userInput == 0 && computerInput ==2 || userInput==1 && computerInput ==0 || userInput ==2 && computerInput ==1 ){
    
		    System.out.println("you win");
		}
		else{
    
		    System.out.println("computer win");
		}
	}
}
