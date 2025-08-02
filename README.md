# Day9-of-43-of-Teachersdaychallenge
A. Petya and Strings
Problem Description: Compare two strings lexicographically, ignoring case. Print "-1" if the first is less, "1" if the second is less, and "0" if they are equal. Strings consist of uppercase and lowercase Latin letters and have lengths from 1 to 100.

Key Idea/Logic:

To compare strings lexicographically without considering case, convert both strings to a consistent case (e.g., all lowercase or all uppercase) before comparison.

Most programming languages have built-in functions for case conversion and lexicographical comparison.

Read the two input strings.

Convert both strings to lowercase (or uppercase).

Compare the converted strings directly:

If s1 < s2, print "-1".

If s1 > s2, print "1".

If s1 == s2, print "0".

Time Complexity: O(L) where L is the length of the strings (up to 100), as string conversion and comparison take linear time.

Space Complexity: O(L) for storing the converted strings.

Example:
Input:

abs
Abz
Output: -1
Explanation: abs vs abz (after lowercasing) means abs is lexicographically smaller than abz.



 A. Team
Problem Description: Three friends decide to implement a programming problem if at least two of them are sure about the solution. Given n problems, and for each problem, whether Petya, Vasya, and Tonya are sure (1) or not (0), count how many problems they will solve.

Key Idea/Logic:

Read the number of problems n.

Initialize a counter for solved problems to 0.

Loop n times:

In each iteration, read three integers (0 or 1) representing the friends' certainty for the current problem.

Sum these three integers.

If the sum is 2 or 3 (meaning at least two friends are sure), increment the solved problems counter.

After the loop, print the total count.

Time Complexity: O(N) where N is the number of problems, as each problem's input is processed in constant time.

Space Complexity: O(1) (only a few variables needed).


Example:
Input:

3
1 1 0
1 1 1
1 0 0
Output: 2
Explanation:
Problem 1: 1 + 1 + 0 = 2 (solve)
Problem 2: 1 + 1 + 1 = 3 (solve)
Problem 3: 1 + 0 + 0 = 1 (don't solve)
Total solved: 2

