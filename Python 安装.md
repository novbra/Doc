

# Python 安装

## anaconda

>介绍：集成环境。Python的大礼包，大礼包里面都是有用的。
>里面包含python工作环境、工具库

## 命令

### pip install

>若在线下载报错，可到[https://github.com/cgohlke/win_arm64-wheels](https://github.com/cgohlke/win_arm64-wheels)下载whl包
>
>然后可通过 pip install [本地路径]安装
>
>如 *.whl文件存在于[本地路径]
>cd [本地路径]
>执行命令pip install *.whl

### conda install

>与pip下载的位置不同，不推荐使用

# Python干啥

- 基础编程开发（效率低）
- Web开发（Java太猛了人很多，python还进去就炸）
- 运维开发（√）
- 机器学习（√）
- 深度学习（√）
- 计算机视觉与自然语言处理（√）
- 数据挖掘（√）
- Spark大数据系列（√）
- 。。。

# Python与Java的区别

- 缩进来区分代码行而非分号，也可以写分号但Python的生态里不必写
- 无须指明变量类型，可直接赋值，可自动识别类型
- 没有double. **Python中float可表示双精度浮点数**
- bool类型中取值**True和False都是第一个字母需要大写**
- 字符串操作可拼接+法，也可乘法即复制多少个字符串

### 类型

- int

- float

- str

  >输出是带引号‘’的

- bool

- list

- 元组tuple 有序不可变序列 并不是Enum枚举

  >元组是一种数据结构，可以将多个不同类型的值组合在一起。在[TypeScript](https://www.baidu.com/s?rsv_dl=re_dqa_generate&sa=re_dqa_generate&wd=TypeScript&rsv_pq=cb3a579d00305fdf&oq=元组就是枚举吗&rsv_t=b55d22oJAr/xp0DUJ8gFEI/lpDaxzwiixF2RTYfnVHLkvhLWe70Ecezt/Een+d0LiwjHPXs&tn=68018901_16_pg&ie=utf-8)、[Swift](https://www.baidu.com/s?rsv_dl=re_dqa_generate&sa=re_dqa_generate&wd=Swift&rsv_pq=cb3a579d00305fdf&oq=元组就是枚举吗&rsv_t=b55d22oJAr/xp0DUJ8gFEI/lpDaxzwiixF2RTYfnVHLkvhLWe70Ecezt/Een+d0LiwjHPXs&tn=68018901_16_pg&ie=utf-8)和[Rust](https://www.baidu.com/s?rsv_dl=re_dqa_generate&sa=re_dqa_generate&wd=Rust&rsv_pq=cb3a579d00305fdf&oq=元组就是枚举吗&rsv_t=b55d22oJAr/xp0DUJ8gFEI/lpDaxzwiixF2RTYfnVHLkvhLWe70Ecezt/Een+d0LiwjHPXs&tn=68018901_16_pg&ie=utf-8)等编程语言中，元组通常用于以下场景：
  >
  >- ‌**固定数量的不同类型的元素的组合**‌：元组可以包含不同类型的数据，例如一个元组可以包含一个整数和一个字符串。
  >- ‌**函数返回多个值**‌：当函数需要返回多个值时，元组可以作为一个单元返回这些值。
  >- ‌**类型安全**‌：元组提供类型安全的数据结构，确保每个元素都有明确的类型。

- dict 无序的键值对集合。 HashMap？

- Set

- None：表示空值或无值

# 数值运算

### print

>```python
>print(1+1)
>```
>
>效果
>
>```python
>2
>```

### +-*/%

>与java相同

### 幂运算**

>```python
>2**3
>```
>
>效果
>
>```python
>8
>```

### 赋值

>与C++、Java不同，无须指明变量类型，可自动识别类型
>
>in
>
>```python
>tang=3
>tang
>```
>
>out
>
>```python
>3
>```
>
>in
>
>```python
>b=True
>b
>```
>
>out
>
>```python
>True
>```

### 比较

>in
>
>```python
>a=3
>1<a<5
>```
>
>out
>
>```python
>True
>```

### 取变量类型type()

>in
>
>```python
>type(tang)
>```
>
>out
>
>```python
>int
>```
>
>in
>
>```python
>tang=1.5
>```
>
>out
>
>```python
>float
>```

### 类型转换

- int()

- float()

- str()

  > 不可用于转换int和float，因为它们是数值

### 运算优先级

- ()
- **
- */%
- +-

### 基本数值操作

- abs()取绝对值

- round()四舍五入

- min()多数取最小值

  >in
  >
  >```python
  >min(2,3,4,5)
  >```
  >
  >out
  >
  >```python
  >2
  >```

- max()多数取最大值

  >in
  >
  >```python
  >max(2,3,4,5)
  >```
  >
  >out
  >
  >```python
  >5
  >```

- 科学计数法 e就相当于10的多少次幂

  >in
  >
  >```python
  >1.3e-5
  >```
  >
  >out
  >
  >```python
  >1.3e-05
  >```

  >in
  >
  >```python
  >1.3e5
  >```
  >
  >out
  >
  >```python
  >130000.0
  >```

- 16进制

  >in
  >
  >```python
  >0xff
  >```
  >
  >out
  >
  >```python
  >255
  >```





# 字符串操作

### 拼接+

>in
>
>```python
>tang='hello'+'python'
>tang
>```
>
>out
>
>```python
>'hellopython'
>```

### 乘法*倍数拼接

>in
>
>```python
>tang*3
>```
>
>out
>
>```python
>'hellopythonhellopythonhellopython'
>```

### len() 取字符串长度

>in
>
>```python
>len(tang)
>```
>
>out
>
>```python
>11
>```

### str.split()分割字符串

>默认情况，以空格为分割符
>
>in
>
>```python
>tang='1 2 3 4 5'
>tang.split()
>```
>
>out
>
>```python
>['1','2','3','4','5']
>```

>不以空格为分隔符
>
>in
>
>```python
>tang='1,2,3,4,5'
>tang=tang.split(',')
>tang
>```
>
>out
>
>```python
>['1','2','3','4','5']
>```
>
>上面的结果其实是字符串数组，可以使用下面join函数重新拼回去

### str.join(iterable) 字符拼接器-join函数

>用于可将可迭代对象（如列表、元组等）中的元素连接成一个字符串。它的作用是将多个字符串按照==指定的分隔符==拼接在一起
>
>**但可迭代对象的元素必须是字符串**

>in
>
>```python
>words=['Hello','World','Python']
>result=' '.join(words) # 用空格键连接
>print(result)
>```
>
>out
>
>```python
>Hello World Python
>```
>
>in
>
>```python
>words=['2023','10','15']
>result='-'.join(words) # 用'-'连接
>print(result)
>```
>
>out
>
>```python
>2023-10-15
>```
>
>连接元组中的元素
>
>in
>
>```python
>letters=('a','b','c')
>result=''.join(letters) # 无分隔符
>print(result)
>```
>
>out
>
>```python
>abc
>```
>
>连接集合中的元素
>
>in
>
>```python
>chars={'x','y','z'}
>result=','.join(chars) # 用 ','连接
>print(result)
>```
>
>out
>
>```python
>x,y,z
>```

### str.replace 替换

>in
>
>```python
>tang='hello python'
>tang2=tang.replace('python','world')
>tang2
>```
>
>out
>
>```python
>'hello world'
>```

### str.upper()转换为大写

>in
>
>```python
>tang2.upper()
>```
>
>out
>
>```python
>'HELLO WORLD'
>```

### str.lower()转换为小写

>in
>
>```python
>tang2='HELLO WORLD'
>tang2.lower()
>```
>
>out
>
>```python
>'hello world'
>```

