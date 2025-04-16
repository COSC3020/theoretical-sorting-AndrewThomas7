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

# Answer 

The best way to verify if the claim for time complexity true or not is to directly compare the time it takes for the algorithm to sort an arbitrary list against it's theoretical bounds. We could easily construct an ideal graph for a general sorting algoritm of $O(n)$ mathematically and plot it. Then we create a timer function and run the black-box algorithm against all permuations for some given list ensuring the best case worst case and average cases can be tested. We can then look at the output and see how closely it follows to our theoretical bound. The way we would be able to tell if confirms or deny's what we are looking for it to look directly at the time output of the black-box and comparing that with the perdicted time for the theoretical bound, which would be calcuated mathematically. If it perfectly matches or got close to the bound then this would be good evidence towards the claim, if not then that's evidence against it.

However based on what we talked about in class related to the sterling approximation we already know that the lowest possible bound for the sorting problem is $\Omega(nlog(n))$. This directly contradicts the idea of the algorithm working in the first place. Therefore I find that this general sorting algorithm is likely impossible. Unless there comes some huge revisions in the mathematics we currently use, then this general sorting algorithm  of $O(n)$ would not be possible.
