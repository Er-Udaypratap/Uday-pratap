# Uday-pratap
This is an Integer number guessing game 


import java.util.Scanner;
class Main {
    public static void main(String[] args) {
        System.out.println("***Number Guessing Game***");
        int n =(int) (Math.random()*100);
        System.out.println("Enter number between 1 to 100:");
        Scanner sc=new Scanner(System.in);
        int t=1;
         do{
          int g=sc.nextInt();
            if(n<g){
                System.out.println("choose smaller number, it's big:");
            }
            else if(n>g){
                System.out.println("choose big number, it's small:");
            }
            else if(g==n){
                System.out.println("you Win "+t+" term in, it's same number");
            }
            else{
                System.out.println("not valid:");
            }
            t++;
        }while(true);
    }
}
