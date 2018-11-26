import java.util.Locale;
import java.util.Random;
import java.util.Scanner;



public class Application_1 {

    /**
     Simple game.
     */
    public static void guessing(){    
    Scanner reader = new Scanner(System.in);
    int counter=4;  
        System.out.println("Guess number between 1 and 20 in 4 moves");
            Random rand = new Random();
            int number;
            String info = null;
            number = rand.nextInt(21);
            int guess = Integer.parseInt(reader.nextLine());
            while (guess != number && counter > 1) {
                    counter--;
                if (guess<number) {
                    info = ("litte");
                }
                if (guess>number) {
                    info = ("much");
                }
                 if (number!=guess) {
                    System.out.println("too " + info +"! " + counter + " moves");
                    guess = Integer.parseInt(reader.nextLine());
                }
             }
            //Inner while loop is done, 4 guesses have passed or user have found the right value
           if (number == guess && counter<4) {
                System.out.println("You guessed!");
           }else if (counter == 4){    
                System.out.println("Pure luck!");    
           } else {
               System.out.println("You ran out of guesses. It was " + number );
           }
    }
    
    public static void main(String[] args) {
    Scanner reader = new Scanner(System.in);
    String quit = "Y";
    while (quit.equals("Y")) {   
        guessing();
            //Checks if the user wants to play again
        System.out.println("New game? Y/N");
        quit = reader.nextLine().toUpperCase(Locale.ROOT);
        while (!(quit.equals ("N") || quit.equals ("Y"))){
            System.out.println("Only Y or N, please!");    
            quit = reader.nextLine().toUpperCase(Locale.ROOT);
        }
    }
    if (quit.equals("N")){
        System.out.println("Thanks for playing! Have a nice day!");
    }        
    }
}       
