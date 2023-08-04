class Solution {
public:
    
bool wordBreakHelper(const string& s, int start, const unordered_set<string>& wordDict, vector<int>& memo) {
    if (start == s.length()) {
        return true;
    }

    if (memo[start] != -1) {
        return memo[start];
    }

    for (int end = start + 1; end <= s.length(); ++end) {
        string word = s.substr(start, end - start);
        cout<<"hello"<<endl;
        if (wordDict.find(word) != wordDict.end() && wordBreakHelper(s, end, wordDict, memo)) {
            return memo[start] = 1;
        }
    }

    return memo[start] = 0;
}
    
bool wordBreak(const string& s, const vector<string>& wordDict) {
    unordered_set<string> wordSet(wordDict.begin(), wordDict.end());
    vector<int> memo(s.length(), -1);
    return wordBreakHelper(s, 0, wordSet, memo);
}
};
