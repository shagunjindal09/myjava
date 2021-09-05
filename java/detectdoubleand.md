# detect double and triple spaces
public class Main
{
	public static void main(String[] args) {
  
	String myString="My string contains      double and triple spaces";
  
	System.out.println(myString.indexOf("  "));
  
	System.out.println(myString.indexOf("   "));
	}
}
