# Day 3



1. `while` 语句执行的流程是怎样的?

2. 若 `x = 2`
    ```python
    if(x > 3): 
        print("True")
    else: 
        print("False")
    ```

    则该段代码的执行结果是?

3. 输出两个列表之间的不同元素,如: `[1, 2, 3], [2, 3, 'a'] `则输出`['a', 1]`

4. 该段代码的输出结果为?
    ```python
    x = None
    y = 1
    z = 3
    if not (x and y or z): 
        print("False")
    else: 
        print("True")
    ```

5. 该段代码的输出结果是?
    ```python
    x = 0
    y = 1
    if x and y:
        print("False")
    elif x or y:
        print("True")
    ```

6. 请在空白处填写合适的代码,
    ```python
    cities = ['Beijing', 'Shanghai', 'Shenzhen', 'Guangzhou']
    city=[]
    for i in range(len(cities)):
        city.______
    ```
    利用cities 中的元素创建一个 city 列表。

7. 该段代码的输出结果是?
    ```python
    x = 0
    if x:
        print("False")
    else:
        print("True")
    ```

8. `cities = ['Beijing', 'Shanghai', 'Shenzhen', 'Guangzhou']`,请使用 for语句遍历 cities,输出 cities 中的元素。

9. `print(list(range(1,12,3)))`的结果是?

10. 请倒序打印`['Beijing', 'Shanghai', 'Shenzhen', 'Guangzhou']`

11. 若是想要输出“False”,则 x 可以取哪些整数?
    ```python
    if (x > 5):
        print("True")
    elif x > 0 and x < 5:
        print("False") 
    else: 
        print("Error")
    ```

12. 该段代码的输出结果是?
    ```python
    x = 0
    if not x: 
        print("True")
    else: 
        print("False")
    ```

13. 如下代码
    ```python
    cities = ['Beijing', 'Shanghai', 'Shenzhen', 'Guangzhou']
    for i in range(len(cities)-1): 
        print(cities[i])
    ```
    的输出结果是?

14. 能不能只利用字典和循环，统计`a,b,c`在`m`中分别出现了几次？
    ```python
    m = ['a', 'b', 'b', 'c', 'a', 'b', 'b', 'c']
    dic = {}
    for item in m:
    if item not in dic.keys():
    #TODO
    else:
    #TODO
    ```

15. 请用代码计算 `1 + 3 + 5 + ... + 99 + 101`

16. `if-else`语句执行的流程是怎样的?

17. `L=[1,2,3,4,5], list[range(len(L))]`的结果是?

18. 如下代码
    ```python
    x = [3, 1, 6, 5, 19, 2, 4]
    y = []
    i = 0
    while(x[i] < 10):
        y.append(x[i])
        print(y)
        i += 1
    ```
    y 的最终输出结果是?