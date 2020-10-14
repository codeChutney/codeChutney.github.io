---
title: Example 2 | Add two numbers
parent: Golang
---

# Add two numbers

Simple program to add two numbers in Go. This is just to learn the syntax etc. and not good practices etc.

You can also open this in playground by clicking on [Go](https://play.golang.org/p/k1mk-M5MUNA){:target="_blank"}.

```go
package main

import (
	"fmt"
)

func add(a, b int) int {
	//lets also print out the types
	fmt.Printf("%T, %v \n", a, a)
	fmt.Printf("%T, %v \n", b, b)
	return a + b
}

func main() {
	fmt.Println("Hey, this is a simple example of how to write a method to add two integers.")

	//lets add 2 numbers
	result := add(7, 6)
	fmt.Printf("the sum of the 2 numbers is %v and the type is %T", result, result)
}
```

Taken from [here](https://gobyexample.com/functions){:target="_blank"}.
