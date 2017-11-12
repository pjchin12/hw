# hw

import java.util.*;
public class Tieckets{

     public static void main(String []args){
        Scanner in = new Scanner(System.in);
        System.out.println("Number of half price tickets: ");
        int hp=in.nextInt();
        System.out.println("Number of full price tickets: ");
        int fp = in.nextInt();
        
        boolean isPostive = hp && fp >0;
        boolean isFive = hp + fp <6;
        
        double iprice = hp*45 + fp*90;
        double price;
        final int maxTickets = 100;
        
        int totHpTickets = 0;
        int totFpTickets = 0;
        int purchase = 0;
        double totPrice;
        
        while (isPositive && isFive)
        {
            
            //updates
            purchase++;
            totHpTickets = totHpTickets + hp;
            totFpTickets = totFpTickets + fp;
            
            if (iprice <= 180)
                price = iprice*1.15;
            else 
                if (iprice <= 270)
                    price = iprice*1.1;
                else
                    price = iprice*1.05;
                    
            totPrice = totPrice + price;
            System.out.println("Number of Tickets sold: ");
            System.out.println("Price: "+ price);
            
            //next entry
            
            System.out.println("Number of half price ticekts: ")
            int hp1 = in.nextInt();
            hp = hp1;
            
            System.out.println("Number of full price tickets: ");
            int fp1 = in.nextInt();
            fp = fp1;
            
            isPostive = hp && fp >0;
            isFive = hp + fp <6;
            iprice = hp*45 + fp*90;


        }
        if (isPositive == false)
        {
            System.out.println(purchase + " were made.")
            System.out.println("Total of " + hp + " half-price tickets and "+ fp + " full-price tickets.")
            System.out.println("Amount: " + totPrice)
            
        }
        


     }
}
