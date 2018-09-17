/*
Created By: Nicholas Brean
Created On: September 16 2018
This program is a string blow up program. 
A quick explanation is here, it returns a version of the original string as 
follows: each digit 0-9 that appears in the original string is replaced by 
that many occurrences of the character to the right of the digit
*/

import java.util.Scanner;
public class StringBlowUp {
	public static void main(String args[]){
		
		 //Declaring Values
		 StringBuffer buffer = new StringBuffer(18); //Buffer is like a string which you can edit, I set the max size to 18 characters.
		 Scanner userinput = new Scanner(System.in); //Gets the user input
		 String userInitialString;
		 char nextPositionInString;
		 char positionInString;
		 int counter;
		 int appenedingCounter;

		 //Explain What this project does
		 System.out.println("String blow up will change numbers next to letters into that letter, so '2ax3t' would be 'aaaxtttt'");
		 System.out.println(""); // Skips a line
		 //Telling User What to do
		 System.out.println("Please Enter any string you want that is more than 1 letter and contains 1 number before a letter.");
		 
		 //Assign values to variables
		 userInitialString = userinput.nextLine();
		 
		 //Dummy Proof
		 if (userInitialString.length() == 0){
			 System.out.println("Please Enter a String next time.");
			 System.exit(0);
		 }
		 
		 //Start Of Real Program
		     for (counter = 0; counter < userInitialString.length(); counter++) {

	                positionInString = userInitialString.charAt(counter); //Getting the position in string (How to use char at https://bit.ly/2pcAMSa)

	                if (Character.isDigit(positionInString) && counter < userInitialString.length()-1) { //If position in string is a digit and is not the last position

	                	nextPositionInString = userInitialString.charAt(counter + 1); //If position in string is a digit and is not the last position
	                    
	                    if (!Character.isDigit(nextPositionInString)){ //If the character is a letter
	                    	int repTimes = Integer.parseInt(Character.toString(positionInString));//getting the amount of letters to add
	                    	
	                    	for (appenedingCounter = 0; appenedingCounter < repTimes; appenedingCounter++) { //Made a counter for adding letters to string
	                    		
	                    		 buffer.append(nextPositionInString);//Adding the letter 
	                    	}
	                    	
	                    } else {
	                        buffer.append(userInitialString.charAt(counter+1)); //add the amount of letters the number is
	                    }
	                } else {
	                    buffer.append(positionInString); //simply add if not digit
	                }
	            }
		     System.out.println("Your String Blowup is " + buffer);
	                    
			 }
		
	}

	

