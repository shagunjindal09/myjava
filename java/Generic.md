# generic method
import java.io.*;

import java.util.*;

public class Solution {

    public <T> void printArray(T []s){
    
        for(T x:s){
        
            System.out.println(x);
        }
    }

    public static void main(String[] args) {
    
    
        Solution s1 = new Solution();
        Integer num[] ={1,2,3};
        String Print[]= {"Hello","World"};
        s1.printArray(num);
        s1.printArray(Print);
    }
}
