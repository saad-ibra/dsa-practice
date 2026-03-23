https://leetcode.com/problems/check-if-array-is-sorted-and-rotated/description/

a->b->c->x->y->z
  <-----------
only one decrease while comparing nums[i] and nums[i+1] allowed
all rest should be same or increase

class Solution {
    public boolean check(int[] nums) {
        int x=0;
        if(nums[nums.length-1]>nums[0]){
            x++;
        }
        for(int i=0;i<nums.length-1;i++){
            if ((nums[i]-nums[i+1])>0){
                x++;
            }
        }
        if(x<=1){
        return true;
        }
        else {
        return false;
        }
    }
}