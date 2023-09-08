import java.util.Random;
import java.util.Scanner;

public class Memorygame {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Random random = new Random();
		Scanner in = new Scanner(System.in);
		
		int[] number_randompicked = new int[7];
		int[] number_typed = new int[7];

		
		for (int i = 0; i < 7; i++) {
			
			number_randompicked[i] = random.nextInt(5) + 1;
			System.out.print(number_randompicked[i] + " ");
			
			 try{
			//The pause will last 1 second 
			Thread.sleep(1000);
			}
			catch(InterruptedException	ex)
			{
				Thread.currentThread().interrupt();				
			}
			
		}

		for (int i = 0; i < 20; ++i) {
			System.out.println();			
		}
		
		for (int i = 0; i < 7; i++) {
			System.out.println("Type number: ");
			int number = in.nextInt();
			number_typed[i] =  number;
			
		}
		System.out.println();
		System.out.println("Your numbers were : ");
		for (int a = 0; a < 7; a++) {
			System.out.print(number_typed[a] + " ");
		}
		numbersFound(number_randompicked, number_typed);
	}
		
		public static void numbersFound(int[] number_randompicked, int[] number_typed){
			int n = 0;
			for (int i = 0; i < 7; i++) {
				if (number_typed[i] == number_randompicked[i]){
						n = n+1;
					}
					
				}
			System.out.println("You got " + n + "numbers right. ");	
			}

	}