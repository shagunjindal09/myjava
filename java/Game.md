# GUESS THE NUMBER 
import  java.util.Scanner;

import java.util.Random;

class Game{

    public int noOfGuesses=0;
    
    public int inputNumber;
    
    public int number;
    
    public int getNoOfGuesses(){
    
        return noOfGuesses;
    }
    public void setNoOfGuesses(int noOfGuesses){
    
        this.noOfGuesses = noOfGuesses;
    }
    Game(){
    
        Random r = new Random();
        
        this.number = r.nextInt(100);
    }
    void takeUserInput(){
    
        System.out.println("Guess the number");
        
        Scanner sc = new Scanner(System.in);
        
        inputNumber = sc.nextInt();
    }
    boolean isCorrectNumber(){
    
        noOfGuesses++;
        
        if(inputNumber==number){
        
            System.out.format("Alas! you guessed it right . the number is %d and the guessing no. is %d ",number,noOfGuesses);
            
            return true;
        }
        else if(inputNumber<number){
        
            System.out.println("you are guessed the number is too low");
        }
        else if(inputNumber>number){
        
            System.out.println("you are guessed the number is too high");
        }
        return false;
    }
}
public class Main
{
	public static void main(String[] args) {
	Game g = new Game();
  
	boolean b = false;
  
	while(!b){
  
	    g.takeUserInput();
      
	   b= g.isCorrectNumber();
	}
	}
}
