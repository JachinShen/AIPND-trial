# Day 2

1. 什么叫可变对象？什么叫不可变对象？Python中哪些对象是可变的？哪些是不可变的？

   - 可变对象：在原有数据基础上可以进行修改（增删改），修改后内存存储地址不变。
   - 不可变对象：在原有数据基础上不可以做修改。
   - 如a=1,然后再a=2；相当于新建了一个整型数据，原来a指向存储1的内存空间，现在a指向存储2的内存空间，内存地址发生了变化。
   - Python中的可变对象：列表、集合、字典（list, set, dict）
   - Python中的不可变对象：数字、字符串、元组（int, str, tuple）

2. 列表索引是从下标几开始?给定列表 `L=[1,2,3,4,5],print(L[0:3])`的输出结果是什么?

3. `L=[1,2,3,4,5], print(L[5])`的结果是什么?为什么?如果要取出最后一个元素,应该如何输出?

   - print(L[5])报错，原因是列表索引地址越界
   - 取最后一个元素print(L[-1])

4. `sentence1 = ["I", "wish", "to", "register", "a", "complaint", "."]`请分别取出["I","wish"]和["complaint","."]。

   ```python
   sentence1 = ["I", "wish", "to", "register", "a", "complaint", "."]
   cut_1 = sentence_1[:2]
   cut_2 = sentence_1[-2:]
   print(cut_1,
         cut_2)
   ```

   

5. `my_tuple = (1, 2, 10)`，如何从`my_tuple`中取出第二个值？`my_set = {1, 2, 4}`，可以从中取出第二个值吗？

   - my_tuple[1]
   - 不可以，集合是无序的

6. `sentence1 = "I wish to register a complaint."`请分别写出 `sentence1[30] `和`sentence1[-11]`的结果。

   - `sentence1[30] = '.'`
   - `sentence1[-11] = ' '`

7. `L=["former", "latter", "starboard"]`,请完成:为 L 在末端添加一个元素`“port”`。

8. `L1=[1,2,3,4,5], L2=["star","moon"], L3=[1,2,"star"]`,运用 max 函数,输出最长的列表。

   ```python
   L1 = [1, 2, 3, 4, 5]
   L2 = ["star", "moon"]
   L3 = [1, 2, "star"]
   max_length = max(len(L1), len(L2), len(L3))
   if (max_length == len(L1)):
       print(L1)
   elif (max_length == len(L2)):
       print(L2)
   else:
       print(L3)
   ```

   ```python
   L1 = [1, 2, 3, 4, 5]
   L2 = ["star", "moon"]
   L3 = [1, 2, "star"]
   all_L = [L1, L2, L3]
   print(sorted(all_L, key = lambda x: len(x), reverse = True)[0])
   ```

   

9. 设一个立方体的 `length, width, height = 40, 40, 40`,请写一条输出语句输出立方体的体积。(要求输出形式为:The volume is .)

   ```python
   length = 40
   width = 40
   height = 40
   print("The volume is {}".format(length * width * height))
   ```

   

10. `L=["Car","Carl","Care","Coco","Bar"] `,执行 sorted(L)进行排序,试着总结sorted 按什么规则对列表中字符串进行排序?

    - 先比较首字母
    - 首字母相同再比较第二个
    - 以此类推

11. `a=(2,3)`,试着用 append 方法将 1 添加进 a 的末端,可以成功运行么?如果令 `a=[2,3]`或者` a="2,3"`,能成功运行么?请分别解释原因。

    - 只有 [2,3]可以,因为列表可以用append添加项目
    - 而字符串并没有append方法，同时字符串也是不可变对象

12. `a=(2,3,1,4,5),b=2,3,1,4,5`, a 和 b 表达的含义相同么?请输出 a 中的第一个元素,b 中最后一个元素,以及 b 的长度。

    - 相同
    - `a[0] = 2`
    - `b[-1] = 5`
    - `len(b) = 5`

13. `L=[1,2,3,4,1,4,5,6]`,请完成:

    1. 删除列表中的重复元素并输出一个集合
    2. 将7 随机添加到集合中
    3. 随机从集合中删除一个元素。

    ```python
    L = [1, 2, 3, 4, 1, 4, 5, 6]
    L = set(L)
    print(L)
    L.add(7)
    print(L)
    L.pop()
    print(L)
    ```

    

14. 将字典变为两个元素一一对应的列表,一个只含有关键字,另一个只含有值。

    如:`{'a': 1, 'b': 2}`变为`['a', 'b'], [1, 2]`

    - `dict = {'a': 1, 'b': 2}`
    - `dict.keys()`
    - `dict.values()`

15. `my_list = ['name', 'age', 105, 12.5]`，创建一个新的列表`new_list`，包含`my_list`中的前三个元素

    ```python
    my_list = ['name', 'age', 105, 12.5]
    new_list = my_list[:3]
    print(new_list)
    ```

16. 字典 `elements = {"hydrogen": 1, "helium": 2, "carbon": 6}`中,哪些是键?哪些是值?键的类型可以有哪些?请输出“carbon”对应的值。

    - key有"hydrogen","helium","carbon"
    - value有1,2,6
    - 键的类型可以是任何不可变类型，例如整数或元组，而不仅仅是字符串
    - "carbon"对应6

17. cube:length:40,width:40,height:40。请创建一个字典,包括 cube 的
    所有信息,并输出 cube 的 width 值。

    ```python
    cube = {"length":40, "width":40, "height":40}
    print(cube["width"])
    ```

18. cube:length:40,width:40,height:40, 请创建一个字典,包括 cube 的所
    有信息,并向字典中添加条目“color”和对应值"red"。

    ```python
    cube = {'length':40,'width':40,'height':40}
    cube['color'] = 'red'
    print(cube)
    ```

    