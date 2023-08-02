class Solution {
public:
    void helper(vector<int>& nums,vector<vector<int>> &ans,vector<int>& curr){
        if(curr.size()==nums.size()){
            ans.push_back(curr);return;
        }
        // for(int i=0;i<nums.size();i++){
        //     int x=nums[i];
        //     if(find(curr.begin(),curr.end(),x)==curr.end()){
        //         curr.push_back(x);
        //         helper(nums,ans,curr);
        //         curr.pop_back();
        //     }
        // }
        for(int x:nums){
            if(find(curr.begin(),curr.end(),x)==curr.end()){
                curr.push_back(x);
                helper(nums,ans,curr);
                curr.pop_back();
            }
        }
    }
    vector<vector<int>> permute(vector<int>& nums) {
        vector<int> curr;
        vector<vector<int>> ans;
        helper(nums,ans,curr);
        return ans;
    }
};
