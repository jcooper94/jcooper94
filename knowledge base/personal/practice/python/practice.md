### Tuple:
- **Explanation:** A tuple is an immutable, ordered collection of elements. Once created, you cannot modify its contents.
- **Example:**
  ```python
  my_tuple = (1, 2, 'hello')
  ```
- **Problem:**
  Create a tuple named `coordinates` with the values (3, 4, 5). Print the second element.

### Set:
- **Explanation:** A set is an unordered collection of unique elements.
- **Example:**
  ```python
  my_set = {1, 2, 3}
  ```
- **Problem:**
  Create two sets, `set1` and `set2`, with some common elements. Print the intersection of these sets.

### ARGS and KWARGS:
- **Explanation:** They are used to pass a variable number of arguments to a function. `*args` is used for positional arguments, and `**kwargs` is used for keyword arguments.
- **Example:**
  ```python
  def example_function(arg1, *args, kwarg1='default'):
      print(arg1)
      print(args)
      print(kwarg1)
  ```
- **Problem:**
  Create a function `print_info` that takes a name as the first argument, followed by any number of hobbies, and a country as a keyword argument. Print the name, hobbies, and country.

### Lambda:
- **Explanation:** A lambda function is a small anonymous function defined with the `lambda` keyword.
- **Example:**
  ```python
  square = lambda x: x**2
  ```
- **Problem:**
  Create a lambda function `double` that doubles the given number. Use it to double the value of 7.

### Writing a Test in Python:
- **Explanation:** Tests in Python are often written using the `unittest` module.
- **Example:**
  ```python
  import unittest

  def add(a, b):
      return a + b

  class TestAddFunction(unittest.TestCase):
      def test_add_positive_numbers(self):
          self.assertEqual(add(2, 3), 5)

  if __name__ == '__main__':
      unittest.main()
  ```
- **Problem:**
  Write a test case for the `print_info` function from the ARGS and KWARGS example. Test it with a name, hobbies, and a specified country.