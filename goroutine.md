以下程序的输出是什么？
```go
import "fmt"

func main() {
	for i := 0; i < 10; i++ {
		go func() {
			fmt.Println(i)
		}()
	}
}
```

答案：
不会有任何内容被打印出来。

解释参见：[go语句及其执行规则（上）](https://time.geekbang.org/column/article/39841)