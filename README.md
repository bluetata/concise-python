# concise-python


## 0x00 如何开始 (doing)


## 0x01 基础语法说明 (doing)


### 1.2 常量和变量

#### 1.2.1 常量
#### 1.2.2 变量

在Python中，变量的类型是动态的，可以根据所赋的值自动推断类型。此外，变量名通常**使用小写字母，并可以包含字母、数字和下划线**。

1. 直接赋值：通过使用等号`=`将一个值赋给变量。

```python
variable = 10
```

2. 类型推断赋值：在赋值的同时，根据所赋的值来推断变量的类型。

```python
variable = "Hello, World!"
```

3. 多重赋值：同时给多个变量赋值，可以在一行中为多个变量指定不同的值。

```python
a, b, c = 1, 2, 3
```

4. 解包赋值：将可迭代对象的元素解包到多个变量中。

```python
x, y, z = [10, 20, 30]
```

5. 默认值赋值：在定义变量时，可以为其指定默认值。

```python
variable = None
```

6. 全局变量：在函数内部使用`global`关键字将变量声明为全局变量。

```python
global_var = 100

def my_function():
    global global_var
    global_var += 1
```

### 集合


#### Map 集合


在Python中，可以使用字典（Dictionary）来表示 Map（映射）的数据结构。字典是一种无序的键值对（Key-Value）集合。

以下是在Python中定义字典（Map）的几种常见方法：

> 需要注意的是，字典中的键是唯一的，如果重复使用同一个键，则后面的键值对会覆盖前面的。


1. 使用大括号{}来定义字典，并用冒号将键和值进行分隔，每个键值对之间使用逗号分隔：

```python
my_map = {'key1': 'value1', 'key2': 'value2', 'key3': 'value3'}
```



2. 使用dict()函数创建一个空字典，然后使用[]操作符添加键值对：


```python
my_map = dict()
my_map['key1'] = 'value1'
my_map['key2'] = 'value2'
my_map['key3'] = 'value3'
```

3. 使用dict()函数和包含键值对的可迭代对象（如列表、元组等）来创建字典：


```python
my_map = dict([('key1', 'value1'), ('key2', 'value2'), ('key3', 'value3')])
```


4. 使用字典推导式（Dictionary Comprehension）来创建字典：

```python
my_map = {x: x**2 for x in range(1, 6)}
```


5. 嵌套字典

有的时候可能会出现多个map嵌套在一起，被称为：嵌套字典

比如：

```python
my_map = {'key1': 'value1', 'cols': ["ins_c1","ins_c2","ins_c3"], 'rename': {"re_ins_c1":"v1","re_ins_c2":"v2","re_ins_c3":"v3",}}
```

解释：

* `my_map`是变量名，它是一个字典类型的变量。   
* 字典使用大括号`{}`来表示，其中的键值对使用冒号分隔，键与值之间使用逗号分隔。   
* `key1`是字典的一个键，对应的值是`value1`。   
* `cols`是另一个键，对应的值是一个包含字符串的列表（List）`["ins_c1","ins_c2","ins_c3"]`。
* `rename`是另一个键，对应的值是一个嵌套字典（Nested Dictionary）。嵌套字典中的键是字符串，对应的值也是字符串。   
    * "re_ins_c1"是嵌套字典中的一个键，对应的值是"v1"。   
    * "re_ins_c2"是另一个键，对应的值是"v2"。   
    * "re_ins_c3"是第三个键，对应的值是"v3"。   

这个字典变量my_map包含了不同类型的键值对，包括字符串、列表和嵌套字典。你可以通过使用键来访问字典中的值，例如`my_map['key1']`将返回`'value1'`。同样地，`my_map['cols']`将返回`["ins_c1","ins_c2","ins_c3"]`，`my_map['rename']`将返回`{"re_ins_c1":"v1","re_ins_c2":"v2","re_ins_c3":"v3"}`。

```python

```