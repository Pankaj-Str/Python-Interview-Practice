# Python List Exercise 

1. Python program to interchange first and last elements in a list:

```python
# codeswithpankaj.com
def interchange_first_last(lst):
    lst[0], lst[-1] = lst[-1], lst[0]
    return lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
result_list = interchange_first_last(my_list)
print(result_list)
```

2. Python program to swap two elements in a list:

```python
# codeswithpankaj.com
def swap_elements(lst, pos1, pos2):
    lst[pos1], lst[pos2] = lst[pos2], lst[pos1]
    return lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
result_list = swap_elements(my_list, 1, 3)
print(result_list)
```

3. Python – Swap elements in String list:

```python
# codeswithpankaj.com
def swap_elements_string_list(lst, str1, str2):
    index1, index2 = lst.index(str1), lst.index(str2)
    lst[index1], lst[index2] = lst[index2], lst[index1]
    return lst

# Example usage:
my_list = ['apple', 'banana', 'cherry', 'date']
result_list = swap_elements_string_list(my_list, 'banana', 'cherry')
print(result_list)
```

4. Python | Ways to find length of list:

```python
# codeswithpankaj.com
def find_length_of_list(lst):
    length = len(lst)
    return length

# Example usage:
my_list = [1, 2, 3, 4, 5]
length = find_length_of_list(my_list)
print(length)
```

5. Maximum of two numbers in Python:

```python
# codeswithpankaj.com
def find_maximum(a, b):
    return max(a, b)

# Example usage:
num1 = 10
num2 = 20
max_num = find_maximum(num1, num2)
print(max_num)
```

6. Minimum of two numbers in Python:

```python
# codeswithpankaj.com
def find_minimum(a, b):
    return min(a, b)

# Example usage:
num1 = 10
num2 = 20
min_num = find_minimum(num1, num2)
print(min_num)
```

7. Python | Ways to check if an element exists in a list:

```python
# codeswithpankaj.com
def check_element_exists(lst, element):
    return element in lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
element_to_check = 3
exists = check_element_exists(my_list, element_to_check)
print(exists)
```

8. Different ways to clear a list in Python:

```python
# codeswithpankaj.com
def clear_list(lst):
    lst.clear()
    return lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
cleared_list = clear_list(my_list)
print(cleared_list)
```

9. Python | Reversing a List:

```python
# codeswithpankaj.com
def reverse_list(lst):
    lst.reverse()
    return lst

# Example usage:
my_list = [1, 2, 3, 4, 5]
reversed_list = reverse_list(my_list)
print(reversed_list)
```

10. Python | Cloning or Copying a list:

```python
# codeswithpankaj.com
def clone_list(lst):
    cloned_list = lst.copy()
    return cloned_list

# Example usage:
my_list = [1, 2, 3, 4, 5]
cloned_list = clone_list(my_list)
print(cloned_list)
```

11. Python | Count occurrences of an element in a list:

```python
# codeswithpankaj.com
def count_occurrences(lst, element):
    return lst.count(element)

# Example usage:
my_list = [1, 2, 3, 4, 2, 5, 2]
element_to_count = 2
occurrences = count_occurrences(my_list, element_to_count)
print(occurrences)
```

12. Python Program to find sum and average of List in Python:

```python
# codeswithpankaj.com
def calculate_sum_and_average(lst):
    total_sum = sum(lst)
    average = total_sum / len(lst)
    return total_sum, average

# Example usage:
my_list = [1, 2, 3, 4, 5]
sum_result, average_result = calculate_sum_and_average(my_list)
print(f"Sum: {sum_result}, Average: {average_result}")
```

13. Python | Sum of number digits in List:

```python
# codeswithpankaj.com
def sum_of_digits_in_list(lst):
    return sum(int(digit) for number in lst for digit in str(abs(number)))

# Example usage:
my_list = [12, 34, 56, 78]
result = sum_of_digits_in_list(my_list)
print(result)
```

14. Python | Multiply all numbers in the list:

```python
# codeswithpankaj.com
def multiply_numbers(lst):
    result = 1
    for number in lst:
        result *= number
    return result

# Example usage:
my_list = [1, 2, 3, 4, 5]
product = multiply_numbers(my_list)
print(product)
```

15. Python program to find smallest number in a list:

```python
# codeswithpankaj.com
def find_smallest_number(lst):
    return min(lst)

# Example usage:
my_list = [5, 2, 8, 1, 6]
smallest_num = find_smallest_number(my_list)
print(smallest_num)
```

16. Python program to find largest number in a list:

```python
# codeswithpankaj.com
def find_largest_number(lst):
    return max(lst)

# Example usage:
my_list = [5, 2, 8, 1, 6]
largest_num = find_largest_number(my_list)
print(largest_num)
```

17. Python program to find second largest number in a list:

```python
# codeswithpankaj.com
def find_second_largest_number(lst):
    sorted_list = sorted(set(lst), reverse=True)
    return sorted_list[1]

# Example usage:
my_list = [5, 2, 8, 1, 6]
second_largest_num = find_second_largest_number(my_list)
print(second_largest_num)
```

18. Python program to print even numbers in a list:

```python
# codeswithpankaj.com
def print_even_numbers(lst):
    even_numbers = [num for num in lst if num % 2 == 0]
    return even_numbers

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
even_nums = print_even_numbers(my_list)
print(even_nums)
```

19. Python program to print odd numbers in a List:

```python
# codeswithpankaj.com
def print_odd_numbers(lst):
    odd_numbers = [num for num in lst if num % 2 != 0]
    return odd_numbers

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
odd_nums = print_odd_numbers(my_list)
print(odd_nums)
```

20. Python program to print all even numbers in a range:

```python
# codeswithpankaj.com
def print_even_numbers_in_range(start, end):
    even_numbers = [num for num in range(start, end + 1) if num % 2 == 0]
    return even_numbers

# Example usage:
start_range = 1
end_range = 10
even_nums_range = print_even_numbers_in_range(start_range, end_range)
print(even_nums_range)
```

21. Python program to print all odd numbers in a range:

```python
# codeswithpankaj.com
def print_odd_numbers_in_range(start, end):
    odd_numbers = [num for num in range(start, end + 1) if num % 2 != 0]
    return odd_numbers

# Example usage:
start_range = 1
end_range = 10
odd_nums_range = print_odd_numbers_in_range(start_range, end_range)
print(odd_nums_range)
```

22. Python program to count Even and Odd numbers in a List:

```python
# codeswithpankaj.com
def count_even_odd_numbers(lst):
    even_count = sum(1 for num in lst if num % 2 == 0)
    odd_count = sum(1 for num in lst if num % 2 != 0)
    return even_count, odd_count

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
even_count, odd_count = count_even_odd_numbers(my_list)
print(f"Even Count: {even_count}, Odd Count: {odd_count}")
```

23. Python program to print all even numbers in a range:

```python
# codeswithpankaj.com
def print_even_numbers_in_range(start, end):
    even_numbers = [num for num in range(start, end + 1) if num % 2 == 0]
    return even_numbers

# Example usage:
start_range = 1
end_range = 10
even_nums_range = print_even_numbers_in_range(start_range, end_range)
print(even_nums_range)
```

24. Python program to print all odd numbers in a range:

```python
# codeswithpankaj.com
def print_odd_numbers_in_range(start, end):
    odd_numbers = [num for num in range(start, end + 1) if num % 2 != 0]
    return odd_numbers

# Example usage:
start_range = 1
end_range = 10
odd_nums_range = print_odd_numbers_in_range(start_range, end_range)
print(odd_nums_range)
```

25. Python program to count Even and Odd numbers in a List:

```python
# codeswithpankaj.com
def count_even_odd_numbers(lst):
    even_count = sum(1 for num in lst if num % 2 == 0)
    odd_count = sum(1 for num in lst if num % 2 != 0)
    return even_count, odd_count

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
even_count, odd_count = count_even_odd_numbers(my_list)
print(f"Even Count: {even_count}, Odd Count: {odd_count}")
```

26. Python program to print positive numbers in a list:

```python
# codeswithpankaj.com
def print_positive_numbers(lst):
    positive_numbers = [num for num in lst if num > 0]
    return positive_numbers

# Example usage:
my_list = [-1, 2, -3, 4, -5, 6]
positive_nums = print_positive_numbers(my_list)
print(positive_nums)
```

27. Python program to print negative numbers in a list:

```python
# codeswithpankaj.com
def print_negative_numbers(lst):
    negative_numbers = [num for num in lst if num < 0]
    return negative_numbers

# Example usage:
my_list = [-1, 2, -3, 4, -5, 6]
negative_nums = print_negative_numbers(my_list)
print(negative_nums)
```

28. Python program to print all positive numbers in a range:

```python
# codeswithpankaj.com
def print_positive_numbers_in_range(start, end):
    positive_numbers = [num for num in range(start, end + 1) if num > 0]
    return positive_numbers

# Example usage:
start_range = -5
end_range = 5
positive_nums_range = print_positive_numbers_in_range(start_range, end_range)
print(positive_nums_range)
```

29. Python program to print all negative numbers in a range:

```python
# codeswithpankaj.com
def print_negative_numbers_in_range(start, end):
    negative_numbers = [num for num in range(start, end + 1) if num < 0]
    return negative_numbers

# Example usage:
start_range = -5
end_range = 5
negative_nums_range = print_negative_numbers_in_range(start_range, end_range)
print(negative_nums_range)
```

30. Python program to count positive and negative numbers in a list:

```python
# codeswithpankaj.com
def count_positive_negative_numbers(lst):
    positive_count = sum(1 for num in lst if num > 0)
    negative_count = sum(1 for num in lst if num < 0)
    return positive_count, negative_count

# Example usage:
my_list = [-1, 2, -3, 4, -5, 6]
positive_count, negative_count = count_positive_negative_numbers(my_list)
print(f"Positive Count: {positive_count}, Negative Count: {negative_count}")
```

31. Remove multiple elements from a list in Python:

```python
# codeswithpankaj.com
def remove_multiple_elements(lst, elements_to_remove):
    updated_list = [ele for ele in lst if ele not in elements_to_remove]
    return updated_list

# Example usage:
my_list = [1, 2, 3, 4, 5, 6]
elements_to_remove = [2, 4]
result_list = remove_multiple_elements(my_list, elements_to_remove)
print(result_list)
```

32. Python | Remove empty tuples from a list:

```python
# codeswithpankaj.com
def remove_empty_tuples(lst):
    updated_list = [tup for tup in lst if tup]
    return updated_list

# Example usage:
my_list = [(), (1, 2), (), (3, 4), (), (5, 6)]
result_list = remove_empty_tuples(my_list)
print(result_list)
```

33. Python | Program to print duplicates from a list of integers:

```python
# codeswithpankaj.com
def find_duplicates(lst):
    seen = set()
    duplicates = set(num for num in lst if num in seen or seen.add(num))
    return list(duplicates)

# Example usage:
my_list = [1, 2, 2, 3, 4, 5, 5, 6]
duplicates_list = find_duplicates(my_list)
print(duplicates_list)
```

34. Remove empty List from List:

```python
# codeswithpankaj.com
def remove_empty_lists(lst):
    updated_list = [sublist for sublist in lst if sublist]
    return updated_list

# Example usage:
my_list = [[], [1, 2], [], [3, 4], [], [5, 6]]
result_list = remove_empty_lists(my_list)
print(result_list)
```

35. Python – Convert List to List of dictionaries:

```python
# codeswithpankaj.com
def convert_list_to_dict(lst):
    dict_list = [{'value': item} for item in lst]
    return dict_list

# Example usage:
my_list = [1, 2, 3, 4, 5]
dict_list = convert_list_to_dict(my_list)
print(dict_list)
```

36. Python – Convert Lists of List to Dictionary:

```python
# codeswithpankaj.com
def convert_lists_of_list_to_dict(lists_of_list):
    dict_list = {sublist[0]: sublist[1:] for sublist in lists_of_list}
    return dict_list

# Example usage:
my_lists_of_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
dict_list = convert_lists_of_list_to_dict(my_lists_of_list)
print(dict_list)
```

37. Python | Uncommon elements in Lists of List:

```python
# codeswithpankaj.com
def uncommon_elements_in_lists_of_list(lists_of_list):
    all_elements = [item for sublist in lists_of_list for item in sublist]
    uncommon_elements = [ele for ele in all_elements if all_elements.count(ele) == 1]
    return uncommon_elements

# Example usage:
my_lists_of_list = [[1, 2, 3], [3, 4, 5], [5, 6, 7]]
uncommon_elements = uncommon_elements_in_lists_of_list(my_lists_of_list)
print(uncommon_elements)
```

38. Python program to select Random value from list of lists:

```python
import random

# codeswithpankaj.com
def select_random_value(list_of_lists):
    random_list = random.choice(list_of_lists)
    random_value = random.choice(random_list)
    return random_value

# Example usage:
my_list_of_lists = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
random_value = select_random_value(my_list_of_lists)
print(random_value)
```

39. Python – Reverse Row sort in Lists of List:

```python
# codeswithpankaj.com
def reverse_row_sort(lists_of_list):
    sorted_lists = [sorted(sublist, reverse=True) for sublist in lists_of_list]
    return sorted_lists

# Example usage:
my_lists_of_list = [[3, 2, 1], [6, 5, 4], [9, 8, 7]]
sorted_lists = reverse_row_sort(my_lists_of_list)
print(sorted_lists)
```

40. Python – Pair elements with Rear element in Matrix Row:

```python
# codeswithpankaj.com
def pair_elements_with_rear(matrix):
    paired_matrix = [[(matrix[row][col], matrix[row][col + 1]) for col in range(len(matrix[row]) - 1)] for row in range(len(matrix))]
    return paired_matrix

# Example usage:
my_matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
paired_matrix = pair_elements_with_rear(my_matrix)
print(paired_matrix)
```

41. Python Program to count unique values inside a list:

```python
# codeswithpankaj.com
def count_unique_values(lst):
    unique_values = len(set(lst))
    return unique_values

# Example usage:
my_list = [1, 2, 3, 1, 2, 4, 5]
unique_count = count_unique_values(my_list)
print(unique_count)
```

42. Python – List product excluding duplicates:

```python
# codeswithpankaj.com
def product_excluding_duplicates(lst):
    unique_values = list(set(lst))
    product_result = 1
    for value in unique_values:
        product_result *= value
    return product_result

# Example usage:
my_list = [1, 2, 3, 2, 4, 5]
result = product_excluding_duplicates(my_list)
print(result)
```

43. Python – Extract elements with Frequency greater than K:

```python
# codeswithpankaj.com
from collections import Counter

def extract_elements_with_frequency(lst, k):
    frequency_counter = Counter(lst)
    extracted_elements = [ele for ele, count in frequency_counter.items() if count > k]
    return extracted_elements

# Example usage:
my_list = [1, 2, 3, 2, 4, 5, 2]
k_value = 1
result = extract_elements_with_frequency(my_list, k_value)
print(result)
```

44. Python – Test if List contains elements in Range:

```python
# codeswithpankaj.com
def test_list_contains_elements_in_range(lst, start, end):
    return all(start <= ele <= end for ele in lst)

# Example usage:
my_list = [1, 2, 3, 4, 5]
start_range = 1
end_range = 5
contains_elements_in_range = test_list_contains_elements_in_range(my_list, start_range, end_range)
print(contains_elements_in_range)
```

45. Python program to check if the list contains three consecutive common numbers in Python:

```python
# codeswithpankaj.com
def has_three_consecutive_common(lst):
    return any(lst[i] == lst[i+1] == lst[i+2] for i in range(len(lst)-2))

# Example usage:
my_list = [1, 2, 2, 3, 3, 3, 4]
has_consecutive_common = has_three_consecutive_common(my_list)
print(has_consecutive_common)
```

46. Python program to find the Strongest Neighbour:

```python
# codeswithpankaj.com
def find_strongest_neighbour(lst):
    n = len(lst)
    strongest_neighbours = [max(lst[i - 1], lst[i + 1]) for i in range(1, n - 1)]
    return strongest_neighbours

# Example usage:
my_list = [4, 5, 1, 2, 10]
result = find_strongest_neighbour(my_list)
print(result)
```

47. Python Program to print all Possible Combinations from the three Digits:

```python
# codeswithpankaj.com
from itertools import permutations

def print_all_combinations_three_digits():
    digits = [1, 2, 3]
    combinations = list(permutations(digits, 3))
    return combinations

# Example usage:
result = print_all_combinations_three_digits()
print(result)
```

48. Python program to find all the Combinations in the list with the given condition:

```python
# codeswithpankaj.com
from itertools import combinations

def find_combinations_with_condition(lst, k):
    combinations_list = [comb for comb in combinations(lst, k) if sum(comb) == 10]
    return combinations_list

# Example usage:
my_list = [1, 2, 3, 4, 5]
k_value = 3
result = find_combinations_with_condition(my_list, k_value)
print(result)
```

49. Python program to get all unique combinations of two Lists:

```python
# codeswithpankaj.com
from itertools import product

def get_unique_combinations_of_two_lists(list1, list2):
    unique_combinations = list(product(set(list1), set(list2)))
    return unique_combinations

# Example usage:
list1 = [1, 2]
list2 = ['a', 'b']
result = get_unique_combinations_of_two_lists(list1, list2)
print(result)
```

50. Python program to remove all occurrences of an element from a list:

```python
# codeswithpankaj.com
def remove_all_occurrences(lst, element_to_remove):
    updated_list = [ele for ele in lst if ele != element_to_remove]
    return updated_list

# Example usage:
my_list = [1, 2, 3, 2, 4, 2, 5]
element_to_remove = 2
result_list = remove_all_occurrences(my_list, element_to_remove)
print(result_list)
```

51. Python – Remove Consecutive K element records:

```python
# codeswithpankaj.com
def remove_consecutive_k_element_records(lst, k):
    updated_list = [ele for ele, count in zip(lst, lst[1:] + [None]) if count != k]
    return updated_list

# Example usage:
my_list = [1, 1, 2, 2, 2, 3, 4, 4, 5]
k_value = 2
result_list = remove_consecutive_k_element_records(my_list, k_value)
print(result_list)
```

52. Python – Replace index elements with elements in Other List:

```python
# codeswithpankaj.com
def replace_index_elements_with_other_list(lst1, lst2):
    for index, ele in enumerate(lst2):
        if index < len(lst1):
            lst1[index] = ele
    return lst1

# Example usage:
list1 = [1, 2, 3, 4, 5]
list2 = ['a', 'b', 'c']
result_list = replace_index_elements_with_other_list(list1, list2)
print(result_list)
```

53. Python Program to Retain records with N occurrences of K:

```python
# codeswithpankaj.com
from collections import Counter

def retain_records_with_n_occurrences(lst, k, n):
    frequency_counter = Counter(lst)
    retained_records = [ele for ele in lst if frequency_counter[ele] == n]
    return retained_records

# Example usage:
my_list = [1, 2, 3, 1, 2, 4, 5, 2]
element_to_retain = 2
occurrences_to_retain = 2
result = retain_records_with_n_occurrences(my_list, element_to_retain, occurrences_to_retain)
print(result)
```

54. Python Program to Sort the list according to the column using lambda:

```python
# codeswithpankaj.com
def sort_list_by_column(lst, column):
    sorted_list = sorted(lst, key=lambda x: x[column])
    return sorted_list



