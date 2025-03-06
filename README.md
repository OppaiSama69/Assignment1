# Assignment1

1(a). For the outer loop, it starts with n/2, until n with 1 as increment.
So, total iterations= n - n/2 = n/2
Thus, time complexity for the outer loop is O(n). //We ignore the division by 2.

For the inner loop, it starts with 2, until and including n with doubling the value of j with each iteration.
for 1st iteration- 2 times.
For 2nd iteration- 4 times.
For 3rd iteration- 8 times.
...
For kth iteration (assuming where we reach n)- 2^k
Now, 2^k = n;
     k = log(base2)n   //Taking log on both sides
Thus, time complexity for the inner loop is O(logn). //Ignoring the 2 base of the log

So, total time complexity = O(nlogn). //We multiply



1(b). First, it initializes x, which is O(1).
Now for the method,
It checks (x == 0 || x == 1) and returns x if it satisfies the condition. This is also done in constant time.
The initialization of i and result also takes constant time O(1).

Now for the while loop, i starts as 1 from the initialization, but is made to be 2 by the increment inside the loop.
1st iteration- i = 2; result = 2^2;
2nd iteration- i = 3; result = 3^2;
...
kth iteration(assuming where we reach x)- i = k; result = k^2;
Now, k^2 = x;
     k = sqrt(x);

So, time complexity = O(sqrt(x)).


2. For the coding problem with the container with most water. I assumed that the number and size of the lines are given according to the problem in leetcode. I created an ArrayList with those lines first and then compared each and every line with the others to find the combination that could hold the maximum amount of water. (Yes, it would have been done simply by using regular Array. I did not find the proper use of ArrayList here.)

