class Solution {
public:
    int rev(int n){
        int ans = 0;
        while(n){
            ans = ans * 10 + (n%10);
            n = n/10;
        }
        return ans;
    }
    int countNicePairs(vector<int>& nums) {
        unordered_map<int,int> mp;
        int mod = 1e9+7;
        int count = 0;
        for(int i=0;i<nums.size();i++){
            int req = nums[i] - rev(nums[i]);
            count = (count + mp[req])%mod;
            mp[req]++;
        }
        return count;
    }
};
