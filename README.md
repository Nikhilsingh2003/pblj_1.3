import java.util.Scanner;
  class Fd{
     double amount;
     double intrest_rate;
     double intrest_earned;
     int no_of_days;
     int age_of_account_holder;
     public   double calucate_intrest(double amount,int no_of_days ,int age_of_account_holder ){
         //------->
         // genral less than 1 cr
         // ------>
        if(amount<10000000&&age_of_account_holder<60){
            if(no_of_days>=7&&no_of_days<=14){
                intrest_rate=4.50;
                intrest_earned=(amount*intrest_rate)/100;
            }
            if(no_of_days>14&&no_of_days<=29){
                intrest_rate=4.75;
                intrest_earned=(amount*intrest_rate)/100;
            }
            if(no_of_days>29&&no_of_days<=45){
                intrest_rate=5.50;
                intrest_earned=(amount*intrest_rate)/100;
            }
            if(no_of_days>45&&no_of_days<=60){
                intrest_rate=7;
                intrest_earned=(amount*intrest_rate)/100;
            }
            if(no_of_days>61&&no_of_days<=184){
                intrest_rate=7.50;
                intrest_earned=(amount*intrest_rate)/100;
            }
            if(no_of_days>184&&no_of_days<=365){
                intrest_rate=8;
                intrest_earned=(amount*intrest_rate)/100;
            }
            else if(no_of_days>365){
                intrest_rate=8;
                intrest_earned=(amount*intrest_rate)/100;
            }
            else if(no_of_days<0){
                System.out.println("Plese  enter correct no of days ! number of days can not be less then 1 ");
            }
        }else if(no_of_days>0&&no_of_days<7){
            System.out.println("you have earned "+ 0 +" rupees because in order to earned you have to wait for minimum 7 days ");
        }
        //-------->
        //senior  citezen
         //------>
         if(amount<10000000&&age_of_account_holder>=60){
             if(no_of_days>=7&&no_of_days<=14){
                 intrest_rate=5;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>14&&no_of_days<=29){
                 intrest_rate=5.25;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>29&&no_of_days<=45){
                 intrest_rate=6;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>45&&no_of_days<=60){
                 intrest_rate=7.50;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>61&&no_of_days<=184){
                 intrest_rate=8;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>184&&no_of_days<=365){
                 intrest_rate=8;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             else if(no_of_days>365){
                 intrest_rate=8.50;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             else if(no_of_days<0){
                 System.out.println("Plese  enter correct no of days ! number of days can not be less then 1 ");
             }
         }else if(no_of_days>0&&no_of_days<7){
             System.out.println("you have earned "+ 0 +" rupees because in order to earned you have to wait for minimum 7 days ");
         }
         // ------>
         //amount >1cr
         // ------>

         if(amount>10000000){
             if(no_of_days>=7&&no_of_days<=14){
                 intrest_rate=6.50;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>14&&no_of_days<=29){
                 intrest_rate=6.75;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>29&&no_of_days<=45){
                 intrest_rate=6.75;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>45&&no_of_days<=60){
                 intrest_rate=8;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>61&&no_of_days<=184){
                 intrest_rate=8.50;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             if(no_of_days>184&&no_of_days<=365){
                 intrest_rate=10;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             else if(no_of_days>365){
                 intrest_rate=10;
                 intrest_earned=(amount*intrest_rate)/100;
             }
             else if(no_of_days<0){
                 System.out.println("Plese  enter correct no of days ! number of days can not be less then 1 ");
             }
         }else if(no_of_days>0&&no_of_days<7){
             System.out.println("you have earned "+ 0 +" rupees because in order to earned you have to wait for minimum 7 days ");
         }
        return  intrest_earned;
     }


}
class Rd{
      double intrestRate;
      double amount;
      int maturity_period;
      double monthly_amount;
      int age_of_accont_holder;
      double calculate_intrest(double amount,int maturity_period,int age_of_accont_holder){
double Earning=0.00;
              if(maturity_period>=6&&maturity_period<9){
                 if(age_of_accont_holder<60){
                     intrestRate=7.50;
                     Earning=(amount*intrestRate)/100;
                 }
                 else {
                     intrestRate=8.00;
                     Earning=(amount*intrestRate)/100;
                 }

          }
          if(maturity_period>=9&&maturity_period<12){
              if(age_of_accont_holder<60){
                  intrestRate=7.75;
                  Earning=(amount*intrestRate)/100;
              }
              else {
                  intrestRate=8.25;
                  Earning=(amount*intrestRate)/100;
              }

          }
          if(maturity_period>=12&&maturity_period<15){
              if(age_of_accont_holder<60){
                  intrestRate=8;
                  Earning=(amount*intrestRate)/100;
              }
              else {
                  intrestRate=8.50;
                  Earning=(amount*intrestRate)/100;
              }

          }
          if(maturity_period>=15&&maturity_period<18){
              if(age_of_accont_holder<60){
                  intrestRate=8.25;
                  Earning=(amount*intrestRate)/100;
              }
              else {
                  intrestRate=8.75;
                  Earning=(amount*intrestRate)/100;
              }

          }
          if(maturity_period>=18&&maturity_period<21){
              if(age_of_accont_holder<60){
                  intrestRate=8.50;
                  Earning=(amount*intrestRate)/100;
              }
              else {
                  intrestRate=9.00;
                  Earning=(amount*intrestRate)/100;
              }

          }
          if(maturity_period>=21){
              if(age_of_accont_holder<60){
                  intrestRate=8.75;
                  Earning=(amount*intrestRate)/100;
              }
              else {
                  intrestRate=9.25;
                  Earning=(amount*intrestRate)/100;
              }
          }
else if(maturity_period<6){
              System.out.println("sorry we dont have plan for less than 6 month ");
          }

          //----->
          return  Earning;

      }
}
class sb{
    double amount;
    double intrest_rate;
    double intrest_earned;
    int no_of_days;
    double calculated_intrest(int no_of_days,double amount){
        if(no_of_days>=7&&no_of_days<=14){
            intrest_rate=6.50;
            intrest_earned=(amount*intrest_rate)/100;
        }
        if(no_of_days>14&&no_of_days<=29){
            intrest_earned=(amount*intrest_rate)/100;
        }
        if(no_of_days<0){
            System.out.println("no of days can not be negative ");
        }
        else {
            System.out.println("sorry we dont have plan for you");
        }
        return  intrest_earned;
    }
}
public class account {
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       double amount;
       int age;
       int no_of_days;
       int maturity_period;
       int age_of_accont_holder;
      //  System.out.println(" --------------------------------------------------------------------");
       // System.out.println("                          ----------                                  ");
        //  System.out.println("Enter the amount of which you want to create fd: ");
        // amount=sc.nextDouble();
        // System.out.println(" Enter  the age of customer : ");
        // age=sc.nextInt();
        // System.out.println("Enter  the number of days you want to create FD ");
        // no_of_days=sc.nextInt();

        // Fd f=new Fd();
        // System.out.println("Total intrest earned by the customer is "+ f.calucate_intrest(amount,no_of_days,age);

   System.out.println("           ----------------------------------");
   System.out.println("                  ------MENU------");
   System.out.println("1: Intrest calculator  FD");
   System.out.println("2: Intrest calculator SB");
   System.out.println("3: Intrest calculator RD");
   System.out.println("4: Exit");
           System.out.println(" enter the option you want tpo select from 0----4");
        int option= sc.nextInt();
        
        switch(option){
            case 1:
                 System.out.println("Enter the amount of which you want to create fd: ");
        amount=sc.nextDouble();
        System.out.println(" Enter  the age of customer : ");
        age=sc.nextInt();
        System.out.println("Enter  the number of days you want to create FD ");
        no_of_days=sc.nextInt();

        Fd f=new Fd();
        System.out.println("Total intrest earned by the customer is "+ f.calucate_intrest(amount,no_of_days,age));
             break;
             //------>>>
             //  second case 
             //------
                case 2:
                     System.out.println("Enter the amount of which you want to create  sb: ");
        amount=sc.nextDouble();
      
        System.out.println("Enter  the number of days you want to create sb ");
        no_of_days=sc.nextInt();

        sb s = new sb();
        System.out.println("Total intrest earned by the customer is "+ s.calculated_intrest(no_of_days,amount));
        break;
// third case  
//----------------------------------

case 3:
                    System.out.println("Enter the amount of which you want to create  RD: ");
        amount=sc.nextDouble();
      
        System.out.println("Enter the maturity peroid in month of which  you want to create RD ");
         maturity_period=sc.nextInt();
System.out.println(" Enter  the age of customer : ");
        age_of_accont_holder=sc.nextInt();
        Rd r = new Rd();
        System.out.println("Total intrest earned by the customer is "+ r.calculate_intrest(amount,maturity_period,age_of_accont_holder));
        break;      
            
           // double calculate_intrest(double amount,int maturity_period,int age_of_accont_holder) 
            
            
            case 4:
                System.out.println(" you exit the main menu ");
                break;
        }

    


    }
}
