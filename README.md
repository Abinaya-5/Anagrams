# Anagrams
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;
public class Solution {
	public static String isAnagram(String input1, String input2) {
        if(input1.length()==input2.length()){            
        char[] ch1=input1.toCharArray();
        char[] ch2=input2.toCharArray();
        Arrays.sort(ch1);
        Arrays.sort(ch2);
        if(Arrays.equals(ch1,ch2))
            return "YES";
        else
            return "NO";  
        }
        else
        return "NO";
}
    public static void main(String[] args) {
      Scanner in = new Scanner(System.in);
      String input1= in.nextLine();
      String input2 = in.nextLine();
      System.out.println(isAnagram(input1, input2));
    }
}
