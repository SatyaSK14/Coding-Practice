Write a function to find the longest common prefix string amongst an array of strings.

If there is no common prefix, return an empty string "".

 

Example 1:

Input: strs = ["flower","flow","flight"]
Output: "fl"
Example 2:

Input: strs = ["dog","racecar","car"]
Output: ""
Explanation: There is no common prefix among the input strings.
 

Constraints:

1 <= strs.length <= 200
0 <= strs[i].length <= 200
strs[i] consists of only lower-case English letters.


--------------------------------------------------------------------------
Solution:-----

class Solution:
    def longestCommonPrefix(self, strs: List[str]) -> str:
        s=""
        if len(strs)==0:
            return s
        elif len(strs)==1:
            return strs[0]
        shortest_word = min(strs)
        for index_of_word in range (len(shortest_word)):
            for index_of_list in range (1,len(strs)):
                if strs[0][index_of_word] == strs[index_of_list][index_of_word]:
                    if index_of_list != len(strs)-1 :
                        continue
                    s= s+strs[0][index_of_word]
                else :
                    return s
        return s
