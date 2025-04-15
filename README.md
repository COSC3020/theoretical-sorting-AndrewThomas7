# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.


# Answer 

- The best way to approach verifying if the algorithm has the time complexity it claims is to run some time tests on the algorithm. It is first important to note that since we  don't have access to the code, we don't have access to the operations the code is running and therefore we cannot explicitly find the time complexity. What we could do instead is compare it against known algorithms in a set of time-series tests to see how close it compares to the alternate algorithms. In practice this would look something like could taking all the permutations of a given list, along with some time function which measures how fast a permutation is sorted and then compraring the outcomes. For example because this specific algorithm claims to have a complexity of $O(n)$ for general elements we could compare it against quicksort which the current fastest algorithm we know of at a best case of $O(nlog(n))$, and see how it compares for best case, worst case and average case. This would give us an idea of how fast the algorithm runs. If it's faster than quicksort then we have evidence towards the claim and if not we can them immediatly disprove the calim. Now in the case that it is faster than quicksort we may want to do further testing by comparing it against a more theoretical bound. As in we could come up with some metrics for how fast something should be sorted if it was going to reach $O(n)$ and then test our time outcomes against this. If were close then this could again be solid evidence to prove the claim and if not then we may want to rerun our time trials to make sure they were solid in the first place. We could then repeat this process with the exception of last part, unless needed. Comparing with different algorithms, would help paint a clearer picture for an accurate time complexity and could give an accurate answer for this problem.
