

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