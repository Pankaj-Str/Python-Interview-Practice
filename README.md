# Python interview questions along with their answers :

1. **What is Python?**
   - *Answer:* Python is a high-level, interpreted programming language known for its simplicity and readability. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming.

2. **Explain the difference between Python 2 and Python 3.**
   - *Answer:* Python 2 and Python 3 are two major versions of the language. Python 3 is the latest and has backward-incompatible changes. Some key differences include print statement (Python 2) vs. print() function (Python 3), Unicode handling, and division.

3. **What is PEP 8?**
   - *Answer:* PEP 8 (Python Enhancement Proposal 8) is the style guide for Python code. It provides guidelines on how to format code for better readability and consistency.

4. **What is the purpose of the `__init__` method in Python?**
   - *Answer:* The `__init__` method is a special method in Python classes that is called when an object is created. It is used to initialize the object's attributes.

5. **Explain the concept of list comprehension.**
   - *Answer:* List comprehension is a concise way to create lists in Python. It allows you to create a new list by specifying the expression to be evaluated for each item in an existing iterable (e.g., list, tuple) along with optional conditions.

6. **What is the Global Interpreter Lock (GIL) in Python?**
   - *Answer:* The Global Interpreter Lock (GIL) is a mutex that protects access to Python objects, preventing multiple threads from executing Python bytecode at once. This can impact the performance of multi-threaded Python programs.

7. **Explain the differences between a shallow copy and a deep copy.**
   - *Answer:* A shallow copy creates a new object, but does not create copies of nested objects; it only copies references. A deep copy, on the other hand, creates a new object and recursively creates copies of all nested objects.

8. **What is the purpose of the `__str__` method?**
   - *Answer:* The `__str__` method is used to define the "informal" or user-friendly string representation of an object. It is called when the `str()` function is invoked on an object.

9. **How does exception handling work in Python?**
   - *Answer:* Python uses a try-except block for exception handling. Code within the try block is executed, and if an exception occurs, the corresponding except block is executed. This helps in handling errors gracefully.

10. **Explain the use of the `with` statement in Python.**
   - *Answer:* The `with` statement is used for resource management, specifically for dealing with files, sockets, or any object that supports the context management protocol. It ensures proper acquisition and release of resources.

11. **What is a decorator in Python?**
    - *Answer:* A decorator is a design pattern in Python that allows the modification of functions or methods using the `@decorator` syntax. It is often used for aspects like logging, authentication, or modifying behavior without changing the original code.

12. **Explain the use of the `yield` keyword in Python.**
    - *Answer:* The `yield` keyword is used in the context of a generator function to produce a sequence of values iteratively. It allows the function to pause its execution and retain its state, making it memory-efficient for large data sets.

13. **What is the difference between a tuple and a list in Python?**
    - *Answer:* A tuple is immutable (unchangeable), while a list is mutable. Tuples are defined using parentheses `()` and lists using square brackets `[]`. Tuples are generally used for heterogeneous data, and lists for homogeneous data.

14. **What is the purpose of the `__name__` variable in Python?**
    - *Answer:* The `__name__` variable is a special variable that is set to `"__main__"` when the Python script is executed directly. It is often used to determine whether the script is the main program or being imported as a module.

15. **Explain the use of the `super()` function in Python.**
    - *Answer:* The `super()` function is used to call a method from a parent class in an inheritance hierarchy. It is commonly used in the `__init__` method of a subclass to invoke the constructor of the parent class.

16. **What is the purpose of the `*args` and `**kwargs` in function definitions?**
    - *Answer:* `*args` and `**kwargs` allow a function to accept a variable number of arguments. `*args` collects positional arguments into a tuple, and `**kwargs` collects keyword arguments into a dictionary.

17. **Explain the Global Interpreter Lock (GIL) and its impact on multi-threading.**
    - *Answer:* The Global Interpreter Lock (GIL) in CPython prevents multiple native threads from executing Python bytecode in parallel. This can impact the performance of multi-threaded programs as only one thread can execute Python bytecode at a time.

18. **What is the difference between shallow copy and deep copy in Python? Provide examples.**
    - *Answer:* Shallow copy creates a new object but does not create copies of nested objects. Deep copy creates a new object and recursively copies all nested objects. Example:
      ```python
      import copy

      original_list = [1, [2, 3], 4]
      shallow_copy = copy.copy(original_list)
      deep_copy = copy.deepcopy(original_list)
      ```

19. **Explain the purpose of the `__call__` method in Python.**
    - *Answer:* The `__call__` method allows an object to be called as a function. It is executed when the instance is called using the function call syntax. This is useful for creating callable objects.

20. **How does Python's garbage collection work?**
    - *Answer:* Python uses automatic memory management with a garbage collector. The `gc` module provides an interface for garbage collection. The most common form of garbage collection is reference counting, but cyclic garbage collection is also used to detect and collect circular references.

21. **What is a lambda function in Python?**
    - *Answer:* A lambda function is an anonymous function defined using the `lambda` keyword. It is often used for short, simple operations and can take multiple arguments but can only have one expression.

22. **Explain the purpose of the `__init__` and `__new__` methods in Python classes.**
    - *Answer:* The `__init__` method is called after the object has been created to initialize its attributes. The `__new__` method is responsible for creating a new instance of the class and is called before `__init__`.

23. **How can you handle exceptions in Python? Provide examples of try-except blocks.**
    - *Answer:* Exceptions in Python can be handled using try-except blocks. Example:
      ```python
      try:
          result = 10 / 0
      except ZeroDivisionError as e:
          print(f"Error: {e}")
      ```

24. **What is the purpose of the `__slots__` attribute in a Python class?**
    - *Answer:* The `__slots__` attribute is used to explicitly declare data members in a class. It restricts the creation of new attributes at runtime, potentially saving memory and improving performance.

25. **Explain the differences between a set and a frozenset in Python.**
    - *Answer:* A set is mutable and unordered, while a frozenset is immutable and hashable. Sets are defined using curly braces `{}`, and frozensets using the `frozenset()` constructor.

26. **How does Python's `zip()` function work?**
    - *Answer:* The `zip()` function combines multiple iterables element-wise and returns an iterator of tuples. It stops when the shortest input iterable is exhausted. Example:
      ```python
      names = ["Alice", "Bob", "Charlie"]
      ages = [25, 30, 22]
      zipped = zip(names, ages)
      ```

27. **Explain the use of the `__getitem__` and `__setitem__` methods in Python.**
    - *Answer:* The `__getitem__` method allows accessing an item using square bracket notation, and `__setitem__` allows modifying an item. These methods are part of the Python data model and are used in classes that want to emulate sequence behavior.

28. **What is the Global Interpreter Lock (GIL) and how does it affect multiprocessing in Python?**
    - *Answer:* The GIL is a mutex that protects access to Python objects, preventing multiple native threads from executing Python bytecode at once. In multiprocessing, each process has its own Python interpreter and memory space, so the GIL does not affect parallel execution.

29. **Explain the purpose of the `enumerate()` function in Python.**
    - *Answer:* The `enumerate()` function is used to iterate over a sequence while keeping track of the index and the corresponding value. It returns tuples containing the index and the value. Example:
      ```python
      for index, value in enumerate(["apple", "banana", "cherry"]):
          print(index, value)
      ```

30. **How does Python handle default arguments in function definitions?**
    - *Answer:* Default arguments are specified in the function definition and have a default value. If a value is not provided for a default argument, the default value is used. Example:
      ```python
      def greet(name, greeting="Hello"):
          print(f"{greeting}, {name}!")
      ```

31. **Explain the purpose of the `__str__` and `__repr__` methods in Python.**
    - *Answer:* The `__str__` method is used to define the "informal" or user-friendly string representation of an object, while `__repr__` is used for the "formal" or developer-oriented representation. `__repr__` is more for debugging.

32. **What is the purpose of the `*` operator in function arguments?**
    - *Answer:* The `*` operator is used for unpacking iterables in function arguments. It allows passing a variable number of positional arguments to a function. Example:
      ```python
      def sum_values(*args):
          return sum(args)
      ```

33. **Explain the concept of a generator in Python.**
    - *Answer:* A generator is a special type of iterator in Python. It is created using a function with the `yield` keyword, allowing the function to retain its state and produce a sequence of values lazily, improving memory efficiency.

34. **What is the purpose of the `__doc__` attribute in Python?**
    - *Answer:* The `__doc__` attribute is used to access the docstring (documentation string) of a Python object, such as a module, class, or function. It provides information about the object's purpose and usage.

35. **Explain the concept of a context manager in Python.**
    - *Answer:* A context manager in Python is an object that defines the methods `__enter__` and `__exit__`. It is used with the `with` statement to manage resources, such as opening and closing files or acquiring and releasing locks.

36. **How does the `filter()` function work in Python?**
    - *Answer:* The `filter()` function is used to construct an iterator from elements of an iterable for which a function returns true. It takes a function and an iterable and returns an iterator containing only the elements that satisfy the given function. Example:
      ```python
      numbers = [1, 2, 3, 4, 5]
      filtered_numbers = filter(lambda x: x % 2 == 0, numbers)
      ```

37. **What is the purpose of the `async` and `await` keywords in Python?**
    - *Answer:* The `async` and `await` keywords are used in asynchronous programming to define asynchronous functions and to wait for the completion of asynchronous tasks, respectively. They are part of the `asyncio` module.

38. **Explain the purpose of the `collections` module in Python.**
    - *Answer:* The `collections` module provides specialized data structures not available in the built-in types. For example, `Counter` for counting occurrences in a collection, `namedtuple` for creating named tuples, and `deque` for double-ended queues.

39. **How does the `any()` and `all()` functions work in Python?**
    - *Answer:* The `any()` function returns `True` if at least one element in an iterable is true. The `all()` function returns `True` if all elements in an iterable are true. Example:
      ```python
      values = [True, False, True]
      any_result = any(values)
      all_result = all(values)
      ```

40. **Explain the purpose of the `itertools` module in Python.**
    - *Answer:* The `itertools` module provides a collection of fast, memory-efficient tools for working with iterators. It includes functions like `cycle` (endlessly iterates over an iterable), `chain` (concatenates multiple iterables), and `count` (generates an infinite sequence of numbers).

41. **What is the Global Interpreter Lock (GIL), and how does it impact multithreading in Python?**
    - *Answer:* The Global Interpreter Lock (GIL) is a mutex that protects access to Python objects, preventing multiple native threads from executing Python bytecode at once. This can impact the performance of multithreaded Python programs, as only one thread can execute Python bytecode at a time.

42. **Explain the purpose of the `staticmethod` and `classmethod` decorators in Python.**
    - *Answer:* The `staticmethod` decorator is used to define a static method within a class that does not access or modify class or instance state. The `classmethod` decorator is used to define a method that takes the class itself as its first argument, rather than an instance.

43. **How does garbage collection work in Python, and what is the purpose of the `gc` module?**
    - *Answer:* Python uses automatic memory management with a garbage collector. The `gc` module provides an interface for garbage collection, allowing manual control over the garbage collector and providing functions for debugging memory management.

44. **Explain the purpose of the `__next__` method and the `StopIteration` exception in Python iterators.**
    - *Answer:* The `__next__` method is used to retrieve the next item from an iterator. When there are no more items, it should raise the `StopIteration` exception to signal the end of the iteration. In Python 3, the `StopIteration` exception is automatically handled in loops.

45. **What are metaclasses in Python?**
    - *Answer:* Metaclasses are a way to customize class creation in Python. They define how new classes are created and can be thought of as "class of a class." Metaclasses are used less frequently but can be powerful for advanced customization and code generation.

46. **Explain the purpose of the `functools` module in Python.**
    - *Answer:* The `functools` module provides higher-order functions and operations on callable objects. It includes functions like `partial` (creates partially applied functions), `reduce` (applies a binary function successively), and `wraps` (creates well-behaved decorators).

47. **How do you handle file I/O in Python? Provide examples of reading and writing to a file.**
    - *Answer:* File I/O in Python is typically handled using the `open()` function. Example of reading from a file:
      ```python
      with open('example.txt', 'r') as file:
          content = file.read()
      ```
      Example of writing to a file:
      ```python
      with open('output.txt', 'w') as file:
          file.write('Hello, World!')
      ```

48. **Explain the purpose of the `__enter__` and `__exit__` methods in a context manager.**
    - *Answer:* The `__enter__` method is called when entering a `with` block and is responsible for acquiring the necessary resources. The `__exit__` method is called when exiting the block and is responsible for releasing resources. Context managers are often used with the `with` statement.

49. **What is the purpose of the `os` module in Python?**
    - *Answer:* The `os` module in Python provides a way of interacting with the operating system. It includes functions for file and directory manipulation, process management, environment variables, and more.

50. **Explain the differences between shallow copy and deep copy in Python. Provide examples.**
    - *Answer:* Shallow copy creates a new object but does not create copies of nested objects. Deep copy creates a new object and recursively copies all nested objects. Example:
      ```python
      import copy

      original_list = [1, [2, 3], 4]
      shallow_copy = copy.copy(original_list)
      deep_copy = copy.deepcopy(original_list)
      ```

51. **Explain the purpose of the `zip()` function in Python, and provide an example.**
    - *Answer:* The `zip()` function in Python combines multiple iterables element-wise and returns an iterator of tuples. Example:
      ```python
      names = ["Alice", "Bob", "Charlie"]
      ages = [25, 30, 22]
      zipped = zip(names, ages)
      ```

52. **What is a Python decorator, and how is it used? Provide an example.**
    - *Answer:* A decorator is a design pattern in Python that allows the modification of functions or methods using the `@decorator` syntax. Example:
      ```python
      def my_decorator(func):
          def wrapper():
              print("Something is happening before the function is called.")
              func()
              print("Something is happening after the function is called.")
          return wrapper

      @my_decorator
      def say_hello():
          print("Hello!")

      say_hello()
      ```

53. **Explain the purpose of the `map()` function in Python, and provide an example.**
    - *Answer:* The `map()` function applies a given function to all items in an input iterable and returns an iterator of the results. Example:
      ```python
      numbers = [1, 2, 3, 4, 5]
      squared = map(lambda x: x**2, numbers)
      ```

54. **What is the purpose of the `__slots__` attribute in a Python class?**
    - *Answer:* The `__slots__` attribute is used to explicitly declare data members in a class. It restricts the creation of new attributes at runtime, potentially saving memory and improving performance.

55. **Explain the purpose of the `sys` module in Python.**
    - *Answer:* The `sys` module provides access to some variables used or maintained by the Python interpreter, such as command line arguments, the Python path, and the standard input/output streams.

56. **How can you create a virtual environment in Python?**
    - *Answer:* You can create a virtual environment using the `venv` module. Example:
      ```
      python -m venv myenv
      ```

57. **Explain the purpose of the `requests` library in Python.**
    - *Answer:* The `requests` library is used for making HTTP requests in Python. It provides a simple API for sending HTTP/1.1 requests and handling responses.

58. **What is the purpose of the `logging` module in Python?**
    - *Answer:* The `logging` module provides flexible logging of messages in Python applications. It allows developers to configure different log handlers, set log levels, and route log messages to various destinations.

59. **Explain the use of the `filter()` function in Python. Provide an example.**
    - *Answer:* The `filter()` function constructs an iterator from elements of an iterable for which a function returns true. Example:
      ```python
      numbers = [1, 2, 3, 4, 5]
      even_numbers = filter(lambda x: x % 2 == 0, numbers)
      ```

60. **How can you handle exceptions in Python? Provide examples of try-except blocks.**
    - *Answer:* Exceptions in Python can be handled using try-except blocks. Example:
      ```python
      try:
          result = 10 / 0
      except ZeroDivisionError as e:
          print(f"Error: {e}")
      ```

61. **Explain the purpose of the `sorted()` function in Python, and how does it differ from the `sort()` method?**
    - *Answer:* The `sorted()` function returns a new sorted list from the elements of any iterable, while the `sort()` method is an in-place operation that sorts a list. Example:
      ```python
      numbers = [3, 1, 4, 1, 5, 9, 2]
      sorted_numbers = sorted(numbers)
      ```

62. **What is the purpose of the `__str__` and `__repr__` methods in Python?**
    - *Answer:* The `__str__` method is used to define the "informal" or user-friendly string representation of an object, while `__repr__` is used for the "formal" or developer-oriented representation. `__repr__` is more for debugging.

63. **Explain the purpose of the `*args` and `**kwargs` in function definitions.**
    - *Answer:* `*args` and `**kwargs` allow a function to accept a variable number of arguments. `*args` collects positional arguments into a tuple, and `**kwargs` collects keyword arguments into a dictionary.

64. **What is the purpose of the `itertools` module in Python?**
    - *Answer:* The `itertools` module provides a collection of fast, memory-efficient tools for working with iterators. It includes functions like `cycle` (endlessly iterates over an iterable), `chain` (concatenates multiple iterables), and `count` (generates an infinite sequence of numbers).

65. **Explain the purpose of the `json` module in Python.**
    - *Answer:* The `json` module in Python is used for encoding and decoding JSON data. It provides functions like `json.dumps()` to serialize Python objects into a JSON-formatted string and `json.loads()` to deserialize a JSON-formatted string into Python objects.

66. **How can you handle file I/O in Python? Provide examples of reading and writing to a file.**
    - *Answer:* File I/O in Python is typically handled using the `open()` function. Example of reading from a file:
      ```python
      with open('example.txt', 'r') as file:
          content = file.read()
      ```
      Example of writing to a file:
      ```python
      with open('output.txt', 'w') as file:
          file.write('Hello, World!')
      ```

67. **Explain the purpose of the `collections` module in Python.**
    - *Answer:* The `collections` module provides specialized data structures not available in the built-in types. For example, `Counter` for counting occurrences in a collection, `namedtuple` for creating named tuples, and `deque` for double-ended queues.

68. **What is the purpose of the `__init__` method in Python classes?**
    - *Answer:* The `__init__` method is a special method in Python classes that is called when an object is created. It is used to initialize the object's attributes.

69. **Explain the use of the `with` statement in Python.**
    - *Answer:* The `with` statement is used for resource management, specifically for dealing with files, sockets, or any object that supports the context management protocol. It ensures proper acquisition and release of resources.

70. **How does Python's garbage collection work?**
    - *Answer:* Python uses automatic memory management with a garbage collector. The `gc` module provides an interface for garbage collection. The most common form of garbage collection is reference counting, but cyclic garbage collection is also used to detect and collect circular references.

71. **Explain the purpose of the `enumerate()` function in Python.**
    - *Answer:* The `enumerate()` function is used to iterate over a sequence (such as a list) while keeping track of the index and the corresponding value. It returns tuples containing the index and the value. Example:
      ```python
      for index, value in enumerate(["apple", "banana", "cherry"]):
          print(index, value)
      ```

72. **What is a Python decorator, and how is it used? Provide an example.**
    - *Answer:* A decorator is a design pattern in Python that allows the modification of functions or methods using the `@decorator` syntax. Example:
      ```python
      def my_decorator(func):
          def wrapper():
              print("Something is happening before the function is called.")
              func()
              print("Something is happening after the function is called.")
          return wrapper

      @my_decorator
      def say_hello():
          print("Hello!")

      say_hello()
      ```

73. **Explain the purpose of the `__slots__` attribute in a Python class.**
    - *Answer:* The `__slots__` attribute is used to explicitly declare data members in a class. It restricts the creation of new attributes at runtime, potentially saving memory and improving performance.

74. **What is the purpose of the `filter()` function in Python? Provide an example.**
    - *Answer:* The `filter()` function constructs an iterator from elements of an iterable for which a function returns true. Example:
      ```python
      numbers = [1, 2, 3, 4, 5]
      even_numbers = filter(lambda x: x % 2 == 0, numbers)
      ```

75. **Explain the concept of a context manager in Python.**
    - *Answer:* A context manager in Python is an object that defines the methods `__enter__` and `__exit__`. It is used with the `with` statement to manage resources, such as opening and closing files or acquiring and releasing locks.

76. **What is the purpose of the `sys.argv` list in Python?**
    - *Answer:* The `sys.argv` list in Python contains command-line arguments passed to a script. `sys.argv[0]` is the script name, and subsequent elements contain the arguments.

77. **Explain the purpose of the `super()` function in Python.**
    - *Answer:* The `super()` function is used to call a method from a parent class in an inheritance hierarchy. It is commonly used in the `__init__` method of a subclass to invoke the constructor of the parent class.

78. **How does Python handle default arguments in function definitions?**
    - *Answer:* Default arguments are specified in the function definition and have a default value. If a value is not provided for a default argument, the default value is used. Example:
      ```python
      def greet(name, greeting="Hello"):
          print(f"{greeting}, {name}!")
      ```

79. **Explain the purpose of the `async` and `await` keywords in Python.**
    - *Answer:* The `async` and `await` keywords are used in asynchronous programming to define asynchronous functions and to wait for the completion of asynchronous tasks, respectively. They are part of the `asyncio` module.

80. **What is the purpose of the `shutil` module in Python?**
    - *Answer:* The `shutil` module provides a higher-level interface for file operations. It includes functions for file copying, moving, and archiving, as well as utility functions for working with file paths.

81. **Explain the purpose of the `collections.Counter` class in Python.**
    - *Answer:* The `Counter` class in the `collections` module is used to count the occurrences of elements in a collection (e.g., list, tuple, or string). It returns a dictionary-like object where keys are elements, and values are their counts.

82. **What is the purpose of the `contextlib` module in Python?**
    - *Answer:* The `contextlib` module provides utilities for working with context managers. It includes the `contextmanager` decorator for creating context managers using generators.

83. **Explain the Global Interpreter Lock (GIL) and its impact on CPU-bound and I/O-bound tasks.**
    - *Answer:* The GIL is a mutex that protects access to Python objects and prevents multiple native threads from executing Python bytecode at once. It primarily impacts CPU-bound tasks negatively but has a lesser impact on I/O-bound tasks as threads can release the GIL during I/O operations.

84. **What is the purpose of the `__call__` method in Python?**
    - *Answer:* The `__call__` method allows an object to be called as a function. It is executed when the instance is called using the function call syntax. This is useful for creating callable objects.

85. **How can you handle multiple exceptions in a single `except` block in Python?**
    - *Answer:* Multiple exceptions can be handled in a single `except` block by specifying them as a tuple. Example:
      ```python
      try:
          # code that may raise exceptions
      except (TypeError, ValueError) as e:
          # handle both TypeError and ValueError
      ```

86. **Explain the purpose of the `threading` module in Python.**
    - *Answer:* The `threading` module provides a way to create and manage threads in Python. It includes functions for thread creation, synchronization, and communication.

87. **What is the purpose of the `__name__` variable in Python scripts?**
    - *Answer:* The `__name__` variable is a special variable that is set to `"__main__"` when the Python script is executed directly. It is often used to determine whether the script is the main program or being imported as a module.

88. **Explain the purpose of the `random` module in Python.**
    - *Answer:* The `random` module provides functions for generating pseudorandom numbers. It includes functions for random selection, shuffling, and generating random integers and floats.

89. **What is the purpose of the `functools.partial` function in Python?**
    - *Answer:* The `functools.partial` function is used for partial function application. It allows fixing a certain number of arguments of a function and generating a new function with the remaining arguments as parameters.

90. **Explain the purpose of the `repr()` function in Python.**
    - *Answer:* The `repr()` function is used to obtain the formal string representation of an object. It is often used for debugging and development, providing a representation that, if passed to `eval()`, would recreate the object.

91. **Explain the purpose of the `__doc__` attribute in Python.**
    - *Answer:* The `__doc__` attribute is used to access the docstring (documentation string) of a Python object, such as a module, class, or function. It provides information about the object's purpose and usage.

92. **What is the purpose of the `*` operator in unpacking iterables?**
    - *Answer:* The `*` operator is used for unpacking iterables in function arguments and assignments. It allows passing a variable number of elements as arguments or creating new iterables by combining existing ones.

93. **Explain the purpose of the `functools.wraps` decorator in Python.**
    - *Answer:* The `functools.wraps` decorator is used to update a wrapper function to look more like the wrapped function. It copies attributes such as `__name__` and `__doc__` to the wrapper, making it behave more like the original function.

94. **How does the `any()` and `all()` functions work in Python?**
    - *Answer:* The `any()` function returns `True` if at least one element in an iterable is true. The `all()` function returns `True` if all elements in an iterable are true. Example:
      ```python
      values = [True, False, True]
      any_result = any(values)
      all_result = all(values)
      ```

95. **Explain the purpose of the `try`...`except`...`else` block in Python.**
    - *Answer:* The `try`...`except`...`else` block is used to handle exceptions in Python. Code inside the `try` block is executed, and if an exception occurs, the `except` block is executed. If no exception occurs, the `else` block is executed.

96. **What is the purpose of the `is` operator in Python?**
    - *Answer:* The `is` operator is used to test object identity. It returns `True` if two variables reference the same object, and `False` otherwise.

97. **Explain the purpose of the `os.path` module in Python.**
    - *Answer:* The `os.path` module provides a platform-independent way of using operating system-dependent functionality related to file paths. It includes functions for path manipulation, such as joining paths and retrieving directory names and file names.

98. **How can you handle keyboard interrupts (`Ctrl+C`) in a Python script?**
    - *Answer:* Keyboard interrupts can be handled using a `try`...`except` block with the `KeyboardInterrupt` exception. For example:
      ```python
      try:
          # code that may be interrupted
          while True:
              pass
      except KeyboardInterrupt:
          print("Interrupted by user!")
      ```

99. **What is the purpose of the `timeit` module in Python?**
    - *Answer:* The `timeit` module is used for measuring the execution time of small code snippets. It provides a simple interface to measure the execution time of Python statements or functions.

100. **Explain the purpose of the `zip()` function in Python, and how can it be used to unzip a list of tuples?**
    - *Answer:* The `zip()` function combines multiple iterables element-wise and returns an iterator of tuples. To unzip a list of tuples, you can use the `zip(*iterable)` syntax. Example:
      ```python
      names = ["Alice", "Bob", "Charlie"]
      ages = [25, 30, 22]
      zipped = zip(names, ages)

      # Unzip
      unzipped_names, unzipped_ages = zip(*zipped)
      ```

