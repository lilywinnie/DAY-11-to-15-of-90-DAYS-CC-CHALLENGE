# DAY-11-to-15-of-90-DAYS-CC-CHALLENGE

# DAY-11

# 1. Approximate Answer


You are solving a problem whose correct answer is the integer Y.
The answer you obtained, however, is the integer X.

Your answer will be considered correct if the difference between X and Y is at most K.
In other words, your answer is considered correct if and only if:∣X−Y∣≤K
Given the values of X, Y, and K, determine whether your answer X is correct or not.

Note that 

∣x∣ denotes the absolute value of x.
For example, 
∣12∣=12,∣−15∣=15, and ∣0∣=0.

Input Format

The first and only line of input will contain three space-separated integers X, Y and K — your answer, the correct answer, and the the maximum allowed difference, respectively.


Output Format

Output the answer on a single line: "Yes" if your answer is considered correct, and "No" otherwise (without quotes).

Each letter of the output may be printed in either uppercase or lowercase, i.e, the strings NO, no, No, and nO will all be treated as equivalent.

Constraints

1≤X,Y,K≤20

Sample 1:

Input

10 5 4

Output

No

Explanation: ∣X−Y∣=∣10−5∣=5, while K=4.
Since |X−Y ∣>K, the answer is not considered correct.

Sample 2:

Input

10 5 5

Output

Yes

Explanation:

∣X−Y∣=∣10−5∣=5, while K=5.
Since ∣X−Y∣≤K, the answer is considered correct.



#include <stdio.h>
#include <stdlib.h>

int main() {

     int X,Y,K; 
     scanf("%d %d %d", &X, &Y, &K);
     
     if(abs(X-Y) <= K)
     printf("Yes\n");
     
     else 
     printf("No\n");
}


# 2.Coldplay Tickets


You want to go to the Coldplay concert along with N of your friends. You are buying tickets for everyone.

Each ticket costs 5000 INR. Calculate the total amount you need to pay (in INR).


Input Format

The first and only line of input contains N — the number of friends you have.


Output Format

For each test case, output on a new line the total cost of all tickets for yourself and your friends.

Constraints

1≤N≤5

Sample 1:

Input

1

Output

10000

Explanation:
You are buying tickets for yourself and one friend of yours. Thus, the cost is 2⋅5000=10000.

Sample 2:

Input

5

Output

30000


#include <bits/stdc++.h>

using namespace std;

int main() {
    int N; 
    cin >> N;
     
    cout << (N + 1) * 5000 << endl;
     
    return 0;
}



# 3. 