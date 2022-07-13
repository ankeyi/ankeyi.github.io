##  Go 语言原始码以纯文字撰写，再编译成机器码并封装成单一独立的可执行文件

## Go一共有三种集合
* 切片
* 数组
* 映射表(map)
切片数组以数字为键(索引),从-1开始计数
map中键的类型可以自订，可以用数字以外的类型查询map值

## var 声明变量
```go
// 类型或值必须存在一个
var <var_name> [var_type] [= value]

// 一次声明多个变量，每行后不需要加逗号
var (
    <var_name_1> [type] [=value1]
    <var_name_2> [type] [=value1]
    <var_name_3> [type] [=value1]
)

// 函数内短变量声明,不可用于声明全局变量
<var_name> := <value>

// 声明多个短变量
<var_name1>, <var_name2> := <value1>, <value2>
```
## 函数返回值
```go
// function return value 可以是多个
func max(value1, value2) (max_value int, value1 int, value2 int) {
    if value1 > value2 {
        max_value := value1
    }   else if {
        value1 < value2 {
        max_value := value2
    } else {
        os.Exit(1)
    }
        return max_value, value1, value2
    }
}
```

## Golang 支持UTF-8，所以可以使用中文命名变量或函数, 不过我觉得要尽量避免这样使用

## Golang 符号
* 算数符号
* 比较符号
* 逻辑符号
* 定址符号
* 位运算符
* 受理算符

## 字符串拼接
```go
filename := "httpd" + ".cfg"
```

## 逻辑运算符(逻辑与、逻辑或、逻辑非)
    &&  ||  !

## zero values(零值)
零值一般值该类型(数据类型)具有的默认值或空值, 比如:
|type|zero value|
|:--:|:--:|
|bool|false|
|int|0|
|string|""|
|指针、函数、介面、切片、通道、映射表|nil|
 