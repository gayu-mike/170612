### 基本概念

#### 数据库 database
数据库是一个数据集合（容器），保存着有组织的数据。

#### 表 table
表是特定类型数据的结构化清单，可想象为一个excel表。

每一张表负责存储一类信息，同一个数据库中表的名字是唯一的，

#### 模式 scheme
关于数据库／表的布局和特性的信息。

#### 列 column
列即表中的一个字段，表示表所代表的类的某一属性。

具体把列分解得多细，取决于需求。

#### 数据类型 datatype
每个列都有对应的数据类型，规定了这个列可以存储的数据种类。

不同DBMS都有自己的数据类型分类，但基本的类型是不会变的。

#### 行 row
也称为 记录record。

#### 主键 primary key
每一行用来唯一标识自己独一无二性的 N个列，它要满足：
- 唯一性
- 不允许 null
- 不能修改
- 已经使用过的主键值，即便所在行被删除也不能重用

#### SQL
Structure Query Language，用来和数据库沟通的语言。标准为 ANSI SQL。

### 计算

考虑一下以下情况：
- 数据存储在不同表中
- 列共同检索
- 查询列的值但用不同格式打印
- 求总值
- 求平均值

存储在表中的原始数据不都是我们所需要的，可以检索出来再用编程语言处理，但SQL提供的几乎总是更快的。

这种成为计算字段——由数据库服务器动态计算的，它就是编程常常提到的field，因为对数据库客户端来说是一样的（它们是没办法区分字段和列）。
