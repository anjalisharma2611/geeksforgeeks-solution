# geeksforgeeks-solution
/*you will find geeksforgeeks solution here

You are given an array A of size N. Replace every element with the next greatest element (greatest element on its right side) in the array. Also, since there is no element next to the last element, replace it with -1.

Input:
The first line of input contains an integer T denoting the number of test cases. T testcases follow. Each testcase contains two lines of input. The first line is N, the size of tha array. The second line contains N space separated integers.

Output:
For each testcase, print the modified array.

Constraints:
1 <= T <= 50
1 <= N <= 100
1 <= Ai <= 1000

Example:
Input:
2
6
16 17 4 3 5 2
4
2 3 1 9

Output:
17 5 5 5 2 -1
9 9 9 -1

Explanation:
Testcase1: For 16 the greatest element on its right is 17. For 17 it's 5. For 4 it's 5. For 3 it's 5. For 5 it's 2. For 2 it's -1(no element to its right). So the answer is 17 5 5 5 2 -1

*/

Code:

int rem=0;
int rev=0;
   while(n>0)
   {
       rem=n%10;
       if(rem==0)
        rem=5;
      rev=(rev*10)+rem;
      n=n/10;
   }
   n=rev;
   rev=0;
   while(n>0)
   {
       rem=n%10;
      rev=(rev*10)+rem;
      n=n/10;
   }
  return rev;
 

