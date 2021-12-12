## Go基础

### Go 语言主要特征

#### 思想

Less can be more 大道至简，小而蕴真。让事情变得简单复杂很容，变得简单才难，深刻的工程文化

#### 优点

自带GC

静态编译编译好后，扔服务器直接运行。

简单的思想，没有继承、多态、类等。丰富的库和详细的开发文档。

语法层支持并发和拥有同步并发的 `channel` 类型，使得并发开发变得很简单。

#### 主要特征

1. 自动立即回收
2. 丰富的内置类型
3. 函数多返回值
4. 错误处理
5. 匿名函数和闭包
6. 类型和接口
7. 并发编程
8. 反射
9. 语言交互性

#### 25个关键字

`break` `default`  `func` `interface`  `select` `case` `defer` `go` `map` `struct` `chan` `else` `goto` `package` `switch` `const`  `fallthrough` `if` `range` `type` `continue` `for` `import` `return` `var`

#### 37保留字

Constants: `true` `false` `iota` `nil`

Types: `int` `int8` `int16` `int32` `int64` `uint` `uint8` `uint16` `uint32` `uint64` `uintptr` `float32` `float64` `complex128` `complex64` `bool` `byte` `rune` `string` `error`

Functions: `make` `len` `cap` `new` `append` `copy` `close` `delete` `complex` `real` `imag` `painc` `recover`

### Go内置类型和函数

###### 内置类型：

`bool`

`int(32 or 64)` `int8` `int16` `int32` `int64` 

`uint(32 or 64)` `uint8` `uint16` `uint32` `uint64` 

`float32` `float64`

`string`

`complex64` `complex128`

`array` -- 固定长度数组

###### 引用类型（指针类型）

`slice` -- 序列数组

`map`     -- 映射

`chan`   -- 管道

###### 内置函数

`append`                 -- 追加元素到数组、slice中，返回修改后的数组、slice 

`close`                   -- 主要用来关闭channel

`delete`                 -- 从map中删除key对应的value值

`panic`                   -- 停止常规的goroutine （panic和recover用来做错误处理）

`recover`               -- 允许程序定义goroutine的panic动作

`real`                     -- 返回complex的实部 （complex、real、imag：用于创建和操作复数）

`imag`                     -- 返回complex的虚部

`make`                     -- 用来分配内存，返回type本身（只能用于slice、map、channel） 

`new`                       -- 用来分配内存，主要用来分配值类型，比如int、struct，返回指向type的指针

`cap`                       -- capacity 是容量的意思，用于返回某个类型的最大容量（只用于切片和map）

`copy`                      -- 用于复制和连接slice，返回复制的数目

`len `                        -- 求长度 比如 string、slice、array、map、channel

`print` / `println`  -- 底层打印函数
