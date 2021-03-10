package guessinggame;

import javax.swing.*;
 
public class Code {
    public static void main(String[] args) {
        int computerNumber = (int) (Math.random()*100 + 1);
        int userAnswer = 0;
        System.out.println("Die richtige Antwort lautet " + computerNumber);
        int count = 1;

        while (userAnswer != computerNumber)
        {
            String response = JOptionPane.showInputDialog(null,
                "Bitte eine Zahl zwischen 1-100 eintippen", "Ratespiel", 3);
            userAnswer = Integer.parseInt(response);
            JOptionPane.showMessageDialog(null, ""+ determineGuess(userAnswer, computerNumber, count));
            count++;
        }  
    }

    public static String determineGuess(int userAnswer, int computerNumber, int count){
        if (userAnswer <=0 || userAnswer >100) {
            return "Bitte eine Zahl zwischen 1 und 100 eingeben";
        }
        else if (userAnswer == computerNumber ){
            return "Richtig! Anzahl der Versuche: " + count;
        }
        else if (userAnswer > computerNumber) {
            return "Die Zahl ist zu hoch. Versuch es erneut! Rateversuchnummer: " + count;
        }
        else if (userAnswer < computerNumber) {
            return "Die Zahl ist zu niedrig. Versuch es erneut! Rateversuchnummer: " + count;
        }
        else {
            return "Die Zahl ist nicht korrekt. Versuch es erneut! Rateversuchnummer: " + count;
        }
    }
}
