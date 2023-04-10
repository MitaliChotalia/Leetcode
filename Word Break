class Solution {
    public boolean wordBreak(String s, List<String> wordDict) {
        int len = s.length();
        boolean [] dp = new boolean[len];
        for(int k = 0; k < len; k++)
        {
            for(int j = 0; j <= k; j++)
            {
                if((j == 0 || dp[j-1] == true) && wordDict.contains(s.substring(j, k + 1)))
                {
                    dp[k] = true;
                    break;
                }
            }
        }
        return dp[len-1];
    }
}
