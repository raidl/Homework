# Homework
package boring_grid_5.pkg11.pkg20;

import java.util.*;
public class Boring_Grid_51120 {

    
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        String ABCDEFGHIJ = null;
        
        int[] rows = {1,2,3,4,5,6,7,8,9,10};
        String[] columns = {"A","B","C","D","E","F","G","H","I","J"};
        System.out.println("I have planted battle ships at different location, find them and sink them by entering the column and row to shoot at.");
        int shipsHit = 0;
        char again = 'y';
        while (again == 'y'){
        
        
        
        System.out.println("Please input a number for the column you want from 1 to 10");
        int chosenRow = input.nextInt();
        while (chosenRow > 10 || chosenRow < 1){
            System.out.println("Invalid input, try again");
        
            System.out.println("Please input a number for the row you want from 1 to 10");
            int chosenRow1 = input.nextInt();
            chosenRow = chosenRow1;
        }
        System.out.println("Please input a letter for the row you want in caps, A to J e.g. D");
        String chosenColumn = input.next();
        //battle ships at D6, B4, C10, G8 and J1

//while (!ABCDEFGHIJ.contains(chosenColumn) ){
while (!chosenColumn.equals("A") && !chosenColumn.equals("B")&& !chosenColumn.equals("C")&& !chosenColumn.equals("D")&& !chosenColumn.equals("E")&& !chosenColumn.equals("F")&& !chosenColumn.equals("G")&& !chosenColumn.equals("H")&& !chosenColumn.equals("I")&& !chosenColumn.equals("J")){
            System.out.println("Invalid input, try again");
            System.out.println("Please input a letter for the column you want, A to J e.g. D");
            String chosenColumn1 = input.next();
            chosenColumn = chosenColumn1;
}

if (chosenColumn.equals("A")){
    System.out.println("You missed");
    
}else if(chosenColumn.equals("E")){
    System.out.println("You missed");   
    
}
else if(chosenColumn.equals("F")){
    System.out.println("You missed");
    
}
else if(chosenColumn.equals("H")){
    System.out.println("You missed");
    
}
else if(chosenColumn.equals("I")){
    System.out.println("You missed");
    
}
                
if (chosenColumn.equals("B")) 
    if (chosenRow == 4){
        shipsHit++;
        System.out.println("You hit one of the ships"); //make sure to add loop to the beginning and counter for ships destroyed
    }else {
        System.out.println("You missed");
    }
if (chosenColumn.equals("C")) 
    if (chosenRow == 10){
        shipsHit++;
        System.out.println("You hit one of the ships");
    }else {
        System.out.println("You missed");
    }
if (chosenColumn.equals("D")) 
    if (chosenRow == 6){
        shipsHit++;
        System.out.println("You hit one of the ships");
    }else {
        System.out.println("You missed");
    }
if (chosenColumn.equals("J")) 
    if (chosenRow == 10){
        shipsHit++;
        System.out.println("You hit one of the ships");
    }else {
        System.out.println("You missed");
    }
if (chosenColumn.equals("G")) 
    if (chosenRow == 8){
        shipsHit++;
        System.out.println("You hit one of the ships");
    }else {
        System.out.println("You missed");
        
        
    if (shipsHit == 5){
        System.out.println("You have hit all the ships, well done");
        again = 'n';
    }
    }
    
}
    }               
}
