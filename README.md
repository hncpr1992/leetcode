# leetcode 
  -- # 158
  
## Tips
1. Care about the special cases<br>
2. Think in diverse directions<br>
3. <br>


## Easy
### Array
1.Two Sum -> Use hash table to avoid going through the list <br>
448.Find All Numbers Disappeared in an Array -> 1.Build a buffer to count the numbers | 2.Use the array as a buffer with sign <br>
118.Pascal's Triangle -> understand structure and do it<br>
167	Two Sum II - Input array is sorted: Use the condition of sorted array, use the two pointers at front and rear<br>
35.Search Insert Position -> linear search / binary search (left and right has 1 gap) <br>
66.Plus One -> understand the process of addition<br>
122.Best Time to Buy and Sell Stock II -> dynamic programming -> <br>
27.Remove Element -> Two pointers, front and rear, swap<br>
268.Missing Number -> the sum of numbers　[0,1,2,...,n] is a constant, so the missing one can be calculated<br>
169.Majority Element -> Hashtable | Boyer–Moore majority vote algorithm<br>
283.Move Zeroes -> 27.Remove Element<br>
243.Shortest Word Distance -> Move forward and record the words position to calculate distance<br>
219.Contains Duplicate II -> 243.Shortest Word Distance with a buffer recording multiple elements' index<br>
217.Contains Duplicate -> 219.Contains Duplicate II Hash table or buffer<br>
119.Pascal's Triangle II -> Next one add to the prior one and get the number in next row<br>
26.Remove Duplicates from Sorted Array -> move and swap, two pointers | 27.Remove Element, 283.Move Zeroes<br>
189.Rotate Array<br>
186.Reverse Words in a String II<br>
414.Third Maximum Number -> A slide window that capture the first second and third<br>

### Dynamic Programming
121.Best Time to Buy and Sell Stock -> get today's maxprofit based on yesterday's<br>
122.Best Time to Buy and Sell Stock II<br>
53.Maximum Subarray<br>
198.House Robber -> build a recurrence relation
70.Climbing Stairs -> build a recurrence relation <br>

256.Paint House -> Use previous steps' costs as base and get new min costs<br>
276.Paint Fence -> Same or not Same situations<br>
303.Range Sum Query - Immutable -> Cumsum in a list to get sum of a slice<br>

### Linked List
206.Reverse Linked List -> keep the code in mind<br>
141.Linked List Cycle -> fast and slow pointers<br>
83.Remove Duplicates from Sorted List -> Use the sorted condition <br>
203.Remove Linked List Elements -> take care of the situation that head.val == val<br>
237.Delete Node in a Linked List -> copy next and remove next<br>
234.Palindrome Linked List -> two poiinters with half reversing<br>
160.Intersection of Two Linked Lists -> scan two lists in a loop until find first common node<br>
21.Merge Two Sorted Lists -> merge one node by another O(m+n)<br>

### Hash table
349.Intersection of Two Arrays -> build a hash table and check existence<br>
350.Intersection of Two Arrays II -> hash table but keep the amount of numbers<br>
438.Find All Anagrams in a String -> slide window and form hash table each step<br>
205.Isomorphic Strings　-> build hash table along the way<br>
359.Logger Rate Limiter -> build hash table along the way<br>
204.Count Primes -> Sieve of Eratosthenes<br>


409.Longest Palindrome -> do not iterate to find, learn how to calculate the result, get the pattern<br>
447.Number of Boomerangs -> see the pattern and calculate, build a hash table to store the distance<br>
389.Find the Difference -> trade space for time<br>
246.Strobogrammatic Number -> build a rule and check<br>
242.Valid Anagram -> 389.Find the Difference<br>
136.Single Number -> hash | bit manipulation<br>
290.Word Pattern -> 205.Isomorphic Strings<br>
170.Two Sum III - Data structure design -> Two sum<br>
266.Palindrome Permutation -> 409.Longest Palindrome<br>
202.Happy Number -> build along the way | two pointers (cycle)<br>

### Two pointers
125.Valid Palindrome -> skip punctuations and other<br>
345.Reverse Vowels of a String -> reverse a list with hash table as vowels<br>
344.Reverse String -> just reverse with two pointers<br>

### Stack
155.Min Stack -> remember to use a minStack array to keep the minimum for each push<br>
20.Valid Parentheses -> use a stack to match the input parenthesis<br>
***496.Next Greater Element I -> Use a stack to keep the decreasing sequence***<br>
232.Implement Queue using Stacks -><br>
225. Implement Stack using Queues -><br>

### String
344.Reverse String -> two pointers<br>
13.Roman to Integer -> if left number is smaller than the right number, subtract the left one from the total<br>
293.Flip Game -> slide window to flip<br>
520.Detect Capital -> follow the rules and compare three situations<br>

### Tree
226.Invert Binary Tree -> recurse to flip left and right <br>
270.Closest Binary Search Tree Value -> make your code simple<br>
***235.Lowest Common Ancestor of a Binary Search Tree -> Compare the two nodes' values with root, if at two side, return root, else go left or right***<br>
112.Path Sum -> take the sum at last recursion as argument in the next recursion and manipulate<br>
257.Binary Tree Paths -> dfs<br>
111.Minimum Depth of Binary Tree -> dfs -> 257<br>
100.Same Tree -> compare left , right structure and the root value in recursion<br>
101.Symmetric Tree -> Same as the 100 Same Tree, but compare the left with the right<br>
104.Maximum Depth of Binary Tree -> Same as the 111.Minimum Depth of Binary Tree, but use max<br>
404.Sum of Left Leaves -> memorize the code as a sample<br>
110.Balanced Binary Tree -> memorize the code as a sample | use some value as signals<br>
108. Convert Sorted Array to Binary Search Tree -> memorize the code <br>

### Math
258.Add Digits -> use // and %<br>
171.Excel Sheet Column Number -> calculate like a number<br>
172.Factorial Trailing Zeroes -> Find how many 5 we have n/5 + n/25 + n/125 + n/625 + n/3125+...<br>
202.Happy Number -> when there is a cycle, use two pointers<br>
7.Reverse Integer -> get number by //10 and reverse, set condition for overflow<br>
9.Palindrome Number -> Use % 10 and // 10 in flexible way<br>
453.Minimum Moves to Equal Array Elements -> transform the issue from add to subtract<br>
69.Sqrt(x) -> binary search<br>
204.Count Primes -> memorize the mothod <br>
168.Excel Sheet Column Title -> reduce 1-10 to 0-9<br>
441.Arranging Coins -> you can add number, but you can also subtract number<br>
231. Power of Two -> same as 441.Arranging Coins<br>

### DFS
339.Nested List Weight Sum -> DFS with recursion on nested list<br>

### BFS
107.Binary Tree Level Order Traversal II -> typical BFS algo<br>

2.Add Two Numbers -> Go through two list until empty | add == 1 or 0 <br>
6.ZigZag Conversion -> make sure the period of the string character collection<br>
3.Longest Substring Without Repeating Characters -> two pointers and dynamic hash table<br>
388.Longest Absolute File Path -> hash table + loop <br>
12.Integer to Roman -> follow the rule, go from large number to small number<br>
5.Longest Palindromic Substring -> DP, build a matrix to maintain the states of symmetrics | Manacher's algorithm<br>

540.Single Element in a Sorted Array -> logn indicate binary search, use odd or even amount as the criteria<br>
238.Product of Array Except Self -> two pointers from left to right with an output array<br>
328.Odd Even Linked List -> two pointers slow and fast, do not make mistake at exchange link list nodes<br>
338. Counting Bits -> DP, find the relation between 2^n + i where i <= 2^n and 2^n + i <= num<br>
***148. Sort List***<br>

139.Word Break -> DP, <br>
137.Single Number II -> bit manipulation | hash table<br>
17.Letter Combinations of a Phone Number -> iterate one digit by another<br>
***50. Pow(x, n)***<br>
200.Number of Islands -> DFS, step on to the island and mark it | similar to 419.Battleships in a Board <br>

319.Bulb Switcher -> brain teaser (the factorial come as pairs except for n^2) so just get the square root<br>
153.Find Minimum in Rotated Sorted Array -> binary search<br>
49.Group Anagrams -> sort the string characters and use hash table to store them<br>
22.Generate Parentheses -> backtracking<br>
150.Evaluate Reverse Polish Notation -> stack<br>

223.Rectangle Area -> reframe the construction of the overlap area (right left, left right, bottom top and top bottom)<br>
419.Battleships in a Board -> count the head of the ship<br>
152.Maximum Product Subarray -> record max and min during the DP, swap max and min when nums[i] < 0 <br>
179.Largest Number -> sort two number by comparing their combination str(x)+str(y) and str(y)+str(x)<br>

96.Unique Binary Search Trees -> DP + find the relation btw G(n) and G(0) to G(n-1) with the F(i,n)<br>
56.Merge Intervals -> sort the intervals first and then compare the start of intervals
173.Binary Search Tree Iterator -> DFS inorder but not O(h) complexity | stack plus pointer to push right to the stack whiel evaluating the left O(h)<br>
48.Rotate Image -> flip along diagnal and y axis<br>
228.Summary Ranges -> go through the list and decide ajacent intergers interval<br>

33.Search in Rotated Sorted Array ->　similar method like 153.Find Minimum in Rotated Sorted Array but need to compare target <br>
46.Permutations -> backtracking<br>
36.Valid Sudoku -> Dynamic hash table in 2D<br>

54.Spiral Matrix -> dynamic hash table and set the boundary for turning (need to imrpove) <br>
***147.Insertion Sort List*** <br>
287.Find the Duplicate Number -> pointer lead to the duplicate method<br>
142.Linked List Cycle II -> 2(a+b) = a+b+nk -> a+b = nk -> a = nk-b<br>
***89.Gray Code ->*** <br>
***260.Single Number III ->*** <br>
187.Repeated DNA Sequences -> dynamic hash table | bitmanipulation <br>
220.Contains Duplicate III -> use bucket to separate the values' ranges and maintain a sliding window <br>
***79.Word Search*** <br>
347.Top K Frequent Elements -> hash table + heap sort<br>

***289.Game of Life*** -> <br>
306.Additive Number -> this problem is determined by the choice of first two numbers (loop), them iterate to end to check conditions<br>
229.Majority Element II -> Boyer–Moore majority vote algorithm | not related to order of list<br>
240.Search a 2D Matrix II -> use the sorted attribute of the matrix<br>

222.Count Complete Tree Nodes -> dfs, set condition to decide whether it is a complete binary tree in the recursion<nr>
230.Kth Smallest Element in a BST -> inorder traversal + a kind of pattern for meeting a certain condition in traversal<br>
34.Search for a Range -> binary search and extend the boundary at the last step<br>
74.Search a 2D Matrix -> two times binary search<br>

116.Populating Next Right Pointers in Each Node -> dfs<br>
105. Construct Binary Tree from Preorder and Inorder Traversal -> dfs<br>

114.Flatten Binary Tree to Linked List -> dfs, move left to right, keep track of last node at left<br>
109.Convert Sorted List to Binary Search Tree -> dfs, use slow fast pointer to devide the linklist<br>
199.Binary Tree Right Side View -> BFS, create a list of queues to store the nodes in each level and keep the right most <br>
103.Binary Tree Zigzag Level Order Traversal -> bfs, reverse the level <br>

279.Perfect Squares -> DP, at each step, go through all choices(optimize with only consider squares addition)<br>
62.Unique Paths -> DP, subproblem is m*n, dependecy is P(i-1,j) + P(i,j-1) = P(i,j)<br>
64. Minimum Path Sum -> similar to 62.Unique Paths, DP, get min of left and top<br>
91. Decode Ways -> DP, decide the last two steps, whether they are consistent with the condition<br>
322. Coin Change -> DP<br>

79.Word Search -> backtracking, start from each position of board and decide whether to go next<br>
39.Combination Sum -> Backtracking<br>
78.Subsets -> Backtracking<br>
77.Combinations -> Backtracking<br>
93.Restore IP Addresses -> Backtracking<br>

120.Triangle -> DP<br>
73.Set Matrix Zeroes -> modify first row and col to store 0<br>

88.Merge Sorted Array -> merge from end<br>
617.Merge Two Binary Trees - > DFS<br>

657.Judge Route Circle -> hash table<br>
653.Two Sum IV - Input is a BST -> DFS with hash table<br>
645.Set Mismatch -> index minus method<br>
643.Maximum Average Subarray I -> do not calculate agian<br>
637.Average of Levels in Binary Tree -> DFS<br>

---

## Twitter
161.One Edit Distance -> know the concept of edit difference<br>
60.Permutation Sequence -> math<br>
433.Minimum Genetic Mutation -> Backtracking<br>
380.Insert Delete GetRandom O(1) -> Hash Table<br>
251.Flatten 2D Vector -> stack<br>

341.Flatten Nested List Iterator -> stack<br>
355.Design Twitter -> Hash<br>
378.Kth Smallest Element in a Sorted Matrix -> Binary Search | low or high will move to the kth smallest and then the other bound reaches to be the same<br>
43.Multiply Strings -> implement the manual multiply<br>

42.Trapping Rain Water -> stack to keep a list of descending bars<br>

296.Best Meeting Point -> <br>

---

581.Shortest Unsorted Continuous Subarray -> sort and compare<br>
654.Maximum Binary Tree -> DFS<br>
525.Contiguous Array -> Hash Table | 1 and 0 represent up and down to accumulate<br>
209.Minimum Size Subarray Sum -> 蠕虫法<br>
647.Palindromic Substrings -> 矩阵法+DP<br>

500.Keyboard Row -> Hashtable<br>
557.Reverse Words in a String III -> string problem<br>
575.Distribute Candies -> hashtable<br>
566.Reshape the Matrix -> array<br>
412.Fizz Buzz -> N/A<br>

674.Longest Continuous Increasing Subsequence -> two pointers
671.Second Minimum Node In a Binary Tree -> dfs














