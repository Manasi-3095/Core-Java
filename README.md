# Core-Java

# WAP to check the age of the customer whether it is more than 18 or not
package learn;
class ageexception extends Exception{
	ageexception(String Message){
		super(Message);
	}
	
}
public class cstmmovie {
	
	
	static void checkage(int age) throws ageexception {
		if(age<18) {
			throw new ageexception("For This Movie Age Age Should Be Greater Then 18");
		}
		else {
			System.out.println("Enjoy Your Movie");
			
		}
	}
	

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		try {
			checkage(67);
		}
		catch(ageexception e) {
			System.out.println(e.getMessage());
		}

	}

}

 # WAP to check the age of the customer by taking the input from the user....
 
Custom Exception
package learn;
import java.util.Scanner;
class ageexception extends Exception
{
	ageexception(String Mess)
	{
		super(Mess);
	}
}



public class customexception 
{
	static void checkage (int age)throws ageexception
	{
		if (age<19) 
		{
			throw new ageexception("Next time Pleaseeeee");
		}
		else
		{
			System.out.println("Welcom to the movieee.....");
		}
	}

	public static void main(String[] args)
	{
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter Your Age: ");
		int a = sc.nextInt();
		try {
		checkage(a);
		}
		catch(ageexception e){
			System.out.println(e.getMessage());
		}

	}

}
