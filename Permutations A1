class Solution {
public:
    void helper(vector<int>& nums,int start,vector<vector<int>> &ans){
        if(start==nums.size()){
            ans.push_back(nums);
            return;
        }
        for(int i=start;i<nums.size();i++){
            swap(nums[start],nums[i]);
            helper(nums,start+1,ans);
            swap(nums[start],nums[i]);
        }
    }
    vector<vector<int>> permute(vector<int>& nums) {
        // helper(nums);
        vector<vector<int>> ans;
        helper(nums,0,ans);
        return ans;
    }
};
