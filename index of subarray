/*Brute Force*/
//time complexity O(n2) due to the nested for loops

import java.util.*;

class Solution {
    static ArrayList<Integer> subarraySum(int[] arr, int target) {
        
        ArrayList<Integer> num = new ArrayList<>();
        
        for(int i = 0 ; i < arr.length ; i++){
            
            int sum = 0;
            
            for(int j = i ; j < arr.length ; j++){
                
                sum += arr[j];
                if(sum > target){
                    break;
                }
                if(sum == target){
                    num.add(i + 1);
                    num.add(j + 1);
                    return num;
                }
            }
        }
        
        num.add(-1);
        return num;
    }
}


// Sliding window where if the sum is too larege shrink the window and add the value. if sum == target return the index
//arr[] = [1, 2, 3, 7, 5], target = 12
import java.util.*;

class Solution {
    static ArrayList<Integer> subarraySum(int[] arr, int target) {
        
        ArrayList<Integer> num = new ArrayList<>();
        
        int start = 0;
        int sum = 0;
        
        for(int i = 0 ; i < arr.length ; i++){
            
            sum += arr[i]; // first index value is added to the sum
            
            while(sum > target && start <= i){// check the sum is less than target and end is greater than or equal to the start
                
                    sum -= arr[start];//remove the start index from the sum
                    start++;// inc the start
            }
             if(sum == target){
                    num.add(start+1);
                    num.add(i+1);
                    return num;
            }
            
            
            }
        
        
        num.add(-1);
        return num;
    }
}
