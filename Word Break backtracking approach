class Solution {
public:
    bool helper(int index,string s,unordered_set<string> setOf){
        if(index==s.length()){
            return true;
        }
        for(int i=index+1;i<=s.length();i++){
            string word=s.substr(index,i-index);
            cout<<"hello"<<endl;
            if(setOf.find(word) != setOf.end() and helper(i,s,setOf))return true;
        }
        return false;
    }
    bool wordBreak(string s, vector<string>& wordDict) {
        unordered_set<string> setOfWords(wordDict.begin(),wordDict.end());
        return helper(0,s,setOfWords);
    }
};
