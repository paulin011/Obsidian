Popular Testing Framework for Java
easy to use

In separate package (src/test/java)
the actual tests are methods in a seperate special classs.

  
public class Main {  
    public static void main(String[] args) {  
  
    }  
    public static String FizzBuzz(int n) {  
        if(n % 7 == 0 && n % 5 == 0) {  
            return("FizzBuzz");  
        } else if(n % 5 == 0) {  
            return("Fizz");  
        } else if(n % 7 == 0) {  
            return("Buzz");  
        }  
        return "";  
    }  
}