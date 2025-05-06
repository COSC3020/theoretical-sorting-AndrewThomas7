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

“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”-Andrew Thomas

Sources
#1-https://github.com/COSC3020/theoretical-sorting-DJReflexive- Looked here to figure out what my answer should look like and took some insperation from it in my answer

# Answer 

In order to undertand this grand claim, we would have to subject the black box algorithm to a series of careful tests and comparsions. The first thing we would want to do before verifying the time complexity is to see that the algorithm gives us expected results for sorting. That is we want to make sure it even sorts before going any further. So we would unit test the crap out of it,comparing it against the outputs of known sorting algorithms. If it passed all of these then we could begin to consider time complexity. At this stage we would create a timing algorithm, aka a function that measures how fast an algorithm takes to complete, its operations and we would run it against known soring algorithm. We would run this against all permutations for some list, to ensure we get the best, worst and average cases tested. If the output of these timings is linear then we know it matches the claim and if not then it fails to meet what was boasted. And the linearity we refer to is just some sort of straight line, could be steep or not steep, the outputs just need to be some sort of straight line on a graph in order to meet the criteria.

However based on what we talked about in class related to the sterling approximation we already know that the lowest possible bound for the sorting problem is $\Omega(nlog(n))$. This directly contradicts the idea of the algorithm working in the first place. Therefore I find that this general sorting algorithm is likely impossible. Unless there comes some huge revisions in the mathematics we currently use, then this general sorting algorithm  of $O(n)$ would not be possible.
