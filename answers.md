# CMPS 2200 Assignment 5
## Answers

**Name:**_Josh McCoy


Place all written answers from `assignment-05.md` here for easier grading.





- **1a.**

The greedy algorithm can be employed by determining the largest power of 2, denoted as 2^k, that is less than the given value N. This step is repeated recursively until reaching a final solution that sums up to N. Due to the fact that all coins have values that are powers of 2, this algorithm guarantees an optimal outcome.

- **1b.**
Work: o(log(n))
Span: o(log(n))




- **2a.**
Let's consider a scenario where we have $15 and the available coin denominations are 2, 5, 8, 10, and 12. If we apply the greedy algorithm, it would initially select the coin with the highest value, which is 12. Then, it would choose 2 twice to complete the sum. However, the optimal solution would be to select 10 first, followed by 5. In this case, we notice that 10 is the second highest denomination. Unlike the previous algorithm, there is no apparent pattern connecting the denominations together, and we cannot assume that the highest denomination always leads to the optimal solution.

- **2b.**
The algorithm I propose begins by considering the highest and second highest denominations. It constructs a tree structure where these nodes serve as the starting point, and their children represent the next and second-next highest denominations, respectively. However, these children are only added if their values do not surpass the target value N. To keep track of progress and find the optimal path, a dictionary is created. This dictionary maps each intermediate difference to the minimum number of steps required to reach that particular difference. As the algorithm progresses, the optimal number of steps is continuously updated. Eventually, the algorithm returns the minimum number of steps necessary to reach the desired value N. The algorithm's complexity in terms of both work and span is O(n).


- **3a.**




- **3b.**






- **3c.**



