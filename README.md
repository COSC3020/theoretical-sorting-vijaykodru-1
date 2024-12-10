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


I would begin by testing the black-box implementation of the algorithm with various inputs to verify its ability to sort correctly. These inputs would include reverse-sorted lists, lists with identical or duplicate elements, already sorted arrays, arrays with unique elements, and lists containing different data types such as integers and strings. By doing so, I can evaluate whether the algorithm functions as expected for a wide range of cases.

Next, I would analyze its performance by comparing it to other well-known sorting algorithms. Specifically, I would measure the time it takes to sort arrays of varying sizes and plot the results on a graph, with input size on the x-axis and runtime on the y-axis. A truly $O(n)$ algorithm would produce a straight line on the graph, indicating linear growth, regardless of the input type.

However, the claim of $O(n)$ runtime is unlikely to be valid for general sorting because comparison-based sorting has a theoretical lower bound of $O(nlogn)$. For the algorithm to achieve $O(n)$, it would need to employ a fundamentally different approach, such as a non-comparison-based technique or something else.

If the claim were true, I would expect the following:

- For already sorted lists, the runtime graph would show a straight line.

- For reverse-sorted lists, the graph would also show a straight line, though slightly higher due to the additional work required to sort the elements.

- For other inputs, such as random or duplicate-heavy arrays, the graph would also exhibit linear growth, with variations in the time taken but still maintaining a straight-line trend.

By observing the consistency of linear growth for different input types and scenarios, I would confirm whether the algorithm truly operates in $O(n)$. If the graphs deviate significantly or fail to show linear behavior, it would suggest that the algorithm does not achieve $O(n)$ runtime as claimed.

References: 

I used my previous repository to check for anything I might have missed.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice