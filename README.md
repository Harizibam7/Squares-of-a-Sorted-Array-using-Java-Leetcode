# Squares-of-a-Sorted-Array-using-Java-Leetcode

      class Solution {
          public static void sort(int[] arr){
              int i,j,temp;
              boolean swapped;
              for(i =0; i<arr.length-1;i++){
                  swapped =false;
                  for(j =0; j<arr.length-i-1;j++){
                      if(arr[j]>arr[j+1]){
                          temp = arr[j];
                          arr[j]= arr[j+1];
                          arr[j+1] = temp;
                          swapped = true;
                      }
                  }
                  if(swapped == false){
                      break;
                  }
              }
          }
          public int[] sortedSquares(int[] nums) {
              for(int i =0; i<nums.length;i++){
                  nums[i] = nums[i]*nums[i];
              }
              sort(nums);
              return nums;
          }
      }

      class Solution {
        public int[] sortedSquares(int[] nums) {
            for(int i =0; i<nums.length;i++){
                nums[i] = nums[i]*nums[i];
            }
            Arrays.sort(nums);
            return nums;
        }
    }
      
