# Day 4

1. `a = ['a', 'b', 'c', 'd'], b = [1, 2, 3, 4], print(zip(a, b))` 的结果是什么？

2. 如果`c = [('a', 1), ('b', 2), ('c', 3), ('d', 4)]`，那么如何用zip函数将其拆分？

3. Enumerate函数会返回元组，这些元组包含列表的哪两部分？

4. 如下代码

   ```python
   for i in enumerate('udacity'):
       print(i)
   ```

   的结果是什么？

5. 如下代码

   ```python
   a = 10
   b = 3.5
   my_str = ...?
   print(my_str)
   ```

   期望的输出是：`My 'A' is 10 and my 'B' is 3.5`，...部分怎么填？

6. `a = ['a', 'b', 'c', 'd'], b = [1, 2, 3, 4]`，请用for循环和zip函数实现输出：`['a', 1], ['b', 2], ['c', 3]`

7. `a = ['a', 'b', 'c', 'd'], b = [1, 2, 3, 4], 请采用dict和zip函数实现将两个列表组合成字典。

8. 如下代码

   ```python
   s = [x+2 for x in range(10) if x % 2 == 0 else x + 1]
   print(s)
   ```

   结果是？

9. `a = [1, 2, 3], b = [2, 3], c = list(zip(a, b))`，简单解释c

10. `a = ['a', 'b', 'c', 'd'],  b = [1, 2, 3, 4]`写一段代码，希望得到输出：`[('A', 1), ('B', 2), ('C', 3), ('D', 4)]`

11. `elements = {"hydrogen": 1, "helium": 2, "carbon": 6}`，请根据元素在周期表中的位置，输出位置大于4的元素。

12. 该列表推导式的作用是什么？

    ```python
    vowels = "aeiou"
    sentence = "I am a student"
    nonvowels = ''.join([letter for letter in sentence if not letter in vowels])
    ```

13. 请使用列表推导式，找到100以内可以整除3的数字。

14. `names = ["Rick Sanchez", "Morty Smith", "Summer Smith"]`，请使用split函数提取出每个人的姓氏，以列表形式输出。

15. 请利用列表推导式修改下述代码，实现相同功能

    ```python
    a = [1, 2, 3, 4, 5]
    b = []
    for i in range(len(a)):
        b.append(a[i])
        print(b)
    ```

16. `my_list = ['a', 'b', 'c', 'd', 'e', 'f', 'g']`，取出`my_list`中，所有奇数索引位置的数，放入`list_2`中。

17. Enumerate函数默认起始的索引值为0,如果想要制定起始索引，应该怎么做？

18. Enumerate和zip返回的对象类型分别是什么？