class Solution {
public:
    void combinations(string input, string output, int i, vector<string>& ans, string keypad[]) {
        if (input[i] == '\0') {
            ans.push_back(output);
            return;
        }

    //     if(current_digit==0 or current_digit==1){
    //     printKeypadOutput(input,output,i+1);
    // }
        int currEle = input[i] - '0';

        if(currEle==0 or currEle==1){
            combinations(input,output,i+1,ans,keypad);
        }
        for (int k = 0; k < keypad[currEle].size(); k++) {
            combinations(input, output + keypad[currEle][k], i + 1, ans, keypad);
        }
    }

    vector<string> letterCombinations(string digits) {
        
        string keypad[] = {"", "", "abc", "def", "ghi", "jkl", "mno", "pqrs", "tuv", "wxyz"};
        string output = "";
        int i = 0;
        vector<string> ans;
        if(digits=="")return ans;
        combinations(digits, output, i, ans, keypad);
        return ans;
    }
};
