# Rock-Paper-Scissors-game
import java.util.*;
import java.util.Random;

public class Rock_Paper_Scissors {
    public static void main(String[] args) {
//        int rock= 0;
//        int paper= 1;
//        int scissors= 2;
        System.out.println(" taking input from  user ");
        System.out.println("rock= 0;" + "paper= 1;" + "scissors=2;");
        System.out.println(" enter your move");
        Scanner sc = new Scanner(System.in);
        int user = sc.nextInt();
        System.out.println(" player move is: " + user);
        // for generating random number
        Random r1 = new Random();
        int computer = r1.nextInt(3);
        System.out.println(" computer move is:" + computer);
        if (computer == user) {
            System.out.println(" the match is draw");
        } else if (user == 0 && computer == 1 || user == 1 && computer == 2 || user==2 && computer ==0){
            System.out.println(" you lost the match");
        }
        else {
            System.out.println(" you win the match");
        }
        System.out.println(" thanks for playing the game");
    }
}


