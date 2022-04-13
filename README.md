# 283.-Move-Zeroes
class Solution {
    public void moveZeroes(int[] nums) {
        int c1=0,c2=nums.length-1;
        for(int i=0;i<nums.length;i++)
        {
            if(nums[i]!=0)
            {
                nums[c1]=nums[i];
                c1++;
            }          
        }
         while(c1<nums.length)
         {
             nums[c2]=0;
             c2--;
             c1++;
         }
    }
}
