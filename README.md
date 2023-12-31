# Explaining Runtime Testing 
The measure_runtime function in the code tests the runtime of Recursive_Binary_Search for a given input size by repeatedly running the algorthm a large number of times and then calculating the average runtime. The algorithm creates a sorted list. Then, it sets a target element outside of that list giving us our least optimal scenario since it must search the entire list. Finally, it measures the full time it takes for the whole operation to complete and divides the total runtime by the number of total test runs. This shows the average runtime it takes to preform the binary search at each input size. When running the code, as seen in PlotgraphExample.png, the plot shows that the binary seach algorithm's run time is O(log(n)).

# Explaining other testing 

In order to test our program we’d implement the following test cases:

i) The list, A, is empty
# Should return -1, avoids infinite recursive calls

ii) The element is not in list A where |A| is odd and where |A| is even
# Tests if list eventually becomes empty and for both odd and even lengths

iii) The element is the middle element of list A where |A| is odd and even
# If element is first one pointed to and for both odd and even lengths

iv) The element is in the first quarter of list A where |A| is odd and even
# multiple recurisive calls where we return the first half of list A and for both odd and even lengths

v) The element in in the second quarter of list A where |A| is odd and even
# multiple recursive calls where we alternates from returning the first half of list A to the second half and for both odd and even lengths

vi) The element is in the third quarter of list A where |A| is odd and even
# multiple recursive calls where we alternate from returning the second half of list A to the first half and for both odd and even lengths

vii) The element is in the fourth quarter of list A where |A| is odd and even
# multiple recursive calls where we return the second half of the list A for both even and odd lengths

These test cases cover all possibilities and errors the algorithm would run into.
