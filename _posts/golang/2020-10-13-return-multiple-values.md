---
title: Example 2 | Return multiple values
parent: Golang
---

You can also open this in playground by clicking on [Go](https://play.golang.org/p/yGzI8v1dMYr){:target="_blank"}.

```go
package main

import (
	"fmt"
)

func multipleOut(a, b int) (float64, int, int) {
	return float64(a), b, 370000
}

func main() {
	fmt.Println("Hey, this is a simple example of how to write a method with multiple return values.")

	res1, res2, res3 := multipleOut(7, 6)
	fmt.Printf("the first return value has value %v and type %T\n", res1, res1)
	fmt.Printf("the second return value has value %v and type %T\n", res2, res2)
	fmt.Printf("the third return value has value %v and type %T\n", res3, res3)
		
	//saw, in this case we only care about the second return value
	//note that because we are using the underscore, the compiler does not complaint
	//if you replace the _ with res5 for example you would get './prog.go:20:2: res5 declared but not used'
	
	_, _, res4 := multipleOut(7, 698)
	fmt.Printf("[case 2]the third return value has value %v and type %T\n", res4, res4)
}
```


Taken from [here](https://gobyexample.com/multiple-return-values){:target="_blank"}.
