//brute force
class Solution {
    public int getSecondLargest(int[] arr) {
        // code here
        int max = Integer.MIN_VALUE;
        int sec = Integer.MIN_VALUE;
        for(int i : arr){
            if(i > max){
                max = i;
            }
        }
        
        for(int i : arr){
            if(max != i && i > sec){
                sec = i;
            }
        }
        
        
        return (sec == Integer.MIN_VALUE) ? -1 : sec;
    }
}

//little more optimal
class Solution {
    public int getSecondLargest(int[] arr) {
        // code here
        int max = Integer.MIN_VALUE;
        int sec = Integer.MIN_VALUE;
        for(int num : arr){
            
            if(num > max){
                sec = max;
                max = num;
            }
            
            else if(num > sec && num != max){
                sec = num;
            }
        }
        
        
        return (sec == Integer.MIN_VALUE) ? -1 : sec;
    }
}
