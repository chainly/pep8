# pep8
> - https://www.python.org/dev/peps/pep-0008/
  - readable
  - explicit
  - compatibility
## 代码结构
### 缩进
  - 一级4空格
  - 参数过多的
    * 不换行，的与前一行列对齐
    * 换行的，添加一级与下一行有所区分
  - 有brace(大括号)，bracket(中括号), parenthesis(括号),注释的可不用
### 空格或制表符
  - 设置制表符为4空格
### 行最大字符数
  - 79 for all
  - 72 for 注释，文档说明
### 分行时，操作符在行首还是行尾
  - 均可，选择可读性高者
### 空行
  - 全局函数，类：2空行
  - 类方法：1空行
  - 区分一组逻辑代码：1空行
### 文件编码
  - UTF-8
  - 标准库 ASCII
### 导入
  > - 隐式导入(import yourmodule) --> 相对导入（import .yourmodule）
    - 通配符导入，或导致潜在问题（变量/方法/类覆盖）
  - 一行 一个或同一模块导入多个
  - 顺序
    * #coding: utf-8
    * """docstring""" or # comment
    * __future__
    * dunders(?文档属性) __xx__
    * 标准库
    * 三方库
    * 自定义库
    * 全局变量
    * 本地变量
    * function/class
### 引号
  - 个人双引号优先
### 空格
  - spam(ham[1], {eggs: 2}) # , : 
  - foo = (0,) # ,）
  - if x == 4: print x, y; x, y = y, x # ; 
  - ham[lower+offset : upper+offset][:: step_fn(x)][1:9:] # 作为操作符\
    要求左右相同数目的空格，表明优先级
  - spam(1)
  - dct['key'] = lst[index]
  - 避免尾空格
  - 操作符两边空格
  - 省略空格以区分优先级
  - 默认参数时，操作符旁省略空格
  - 函数解释（Function annotations） def munge(sep: AnyStr = None) -> AnyStr:
  - one_line
### 尾逗号
  - FILES = ('setup.cfg',)
### 注释,文档
  - # Xx( xx unless it shouldn't)
  - yy  # Xx
  - """Do what and return what."""
  - """The summary line(for index).
  
    Keyword arguments:
    x - y (default 0)
    z - z (https://www.python.org/dev/peps/pep-0257/)
    """
### 命名
  - 常量 MAX_INT
  - 变量 
  - 函数名 xx_yy or xxYy
  - 类实例作为参数（self）, 类作为参数（cls）
  - 类 
    * 共有 xx/xx_
    * 私有属性 __xx
    * 特殊属性 __xx__
