 
//File containing pseudocode  and sample code for checking if a number is prime

***PSEUDOCODE***
Loop from i=2 to i<9 and if(num%i==0)
divisiblityCount++;
if divisibilityCount>1==> not prime
if num<10 and count==1 ==>prime
if num not perfect sqr and num>10 and count==0 ==>prime


***FUNCTION***
public static bool isPrime( int num){
    int divisibilityCount=0;
    bool flag=false;
 if(num<=1){
   return flag;
 }else{
   for(int i=2; i<9;i++){
     if(num%i==0){
       divisibilityCount++;
     }

   }
   if(num<10 && divisibilityCount>1){
     return flag;
   }else if(num<10 && divisibilityCount==1){
     flag=true;
     return flag;
   }else if(num%(Math.Sqrt(num))!=0 && num>10 && divisibilityCount==0){
     flag=true;
     return flag;
   }


   }
   return flag;


 }