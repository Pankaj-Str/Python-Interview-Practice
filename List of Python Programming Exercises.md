# List of Python Programming Exercises 

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
