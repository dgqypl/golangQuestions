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