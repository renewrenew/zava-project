
 
public class twelve {
   public static void main(String[] args) {
      Scanner sc = new Scanner(System.in);
      
      String sign;
      System.out.print("연산>>");
      double num = sc.nextDouble();
      sign = sc.next();
      double num1 = sc.nextDouble();
      
      if(sign.equals("+"))
         System.out.print(num+sign+num1+"의 계산 결과는 "+(num + num1));
      else if(sign.equals("-"))
          System.out.print(num+sign+num1+"의 계산 결과는 "+(num - num1));
      else if(sign.equals("*"))
         System.out.print(num+sign+num1+"의 계산 결과는 "+(num*num1));
      else if(sign.equals("/"))
      {  
         if(num1==0)
            System.out.print("0으로 나눌 수 없습니다.");
         else
            System.out.print(num+sign+num1+"의 계산 결과는 "+(num/num1));
      }
      sc.close();
   }
}

import java.util.Scanner;
 
public class twelve {
   public static void main(String[] args) {
      Scanner sc = new Scanner(System.in);
      
      String sign;
      
      System.out.print("연산>> ");
      double num = sc.nextDouble();
      sign = sc.next();
      double num1 = sc.nextDouble();
 
      switch(sign) {
      case "+" :
         System.out.print(num+sign+num1+"의 계산 결과는 "+(num+num1));
         break;
      case "-":
          System.out.print(num+sign+num1+"의 계산 결과는 "+(num-num1));
         break;
      case "*":
          System.out.print(num+sign+num1+"의 계산 결과는 "+(num*num1));
         break;
      case "/":
         if(num1==0) {
            System.out.print("0으로 나눌 수 없습니다.");
            break;
         }
         else {
            System.out.print(num+sign+num1+"의 계산 결과는 "+(num+num1));
            break;
         }
      default:
         System.out.print("잘못 입력하였습니다.");
         break;
      }
      sc.close();
   }
}
