1. go 切片初始化
```go
var arr = make([]int, 5)
arr = append(arr, 1,2,3)
//输出0，0，0，0，0，1，,2，,3
```

2. map可不可以在遍历的时候调用 `delete` 方法删除
首先问清楚条件边界，map是不是并发执行读写操作。如果是的话，可能会抛出panic，因为map不是线程安全的，如果同时读写的话，会panic。可以通过lock锁，保证线程安全。或者使用sync.map是线程安全。
遍历的时候，也可以会出现删除调的元素，因为不确定是先取到结果，还是先删除。

3. 函数返回值
```go
func sum(x, y int) (total int, error) {
    return x+y, nil
}

// 如果有多个返回值，有1个命名了，必须加括号并且全部命名
```

4. map元素取地址
```go
var data = make(map[string]string)
fmt.Println(&data["key"])

// 编译会报错，无法对map的 key 和 value取地址
// 就算通过 hack 的方式 unsafe 取到地址保存了也是没有用
// 因为一扩容，地址就会变，所以没有意义
```

5. 对比两个map元素是否相等
```go
1. 对比是否为nil，对比深度
2. 对比值key
3. 取值然后json压缩对比值
```
6. init 函数执行顺序
```go
// 执行顺序是，导入包》解析常量》变量》init函数》main
// 可以有多个init函数，但是不保证执行顺序
// 不能有参数和返回值
```