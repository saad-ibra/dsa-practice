https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/

a b c x y z 
keep window value 1
start from index 1, check with index 0, if not same store in index window and increment window

class Solution {
    public int removeDuplicates(int[] nums) {

        int y=1;
        for (int i=1; i<=nums.length-1;i++){
            if(nums[i]!=nums[i-1]){
                nums[y]=nums[i];
                y++;
            }
        }
        return y;
    }
}
