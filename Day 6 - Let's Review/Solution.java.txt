import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        Scanner sc = new Scanner(System.in);
        int testCases = sc.nextInt();
        
        for(int i =1 ; i <= testCases ; i++){
            String input = sc.next();
            System.out.println(review(input));
        }
        sc.close();
    }
    
    public static String review(String str){
        String even="" , odd="";
        for(int i = 0 ; i < str.length() ; i++){
            
            if(i%2==0){
                even = even+str.charAt(i);
            }
            else {
                odd +=  str.charAt(i);
            }
            
        }
        
        
        return even + " " + odd;
    }
}
