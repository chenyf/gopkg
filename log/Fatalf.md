## func Fatalf(format string, v ...interface{})

参数列表：

- format 输出格式
- v 带输出参数列表

返回值：

- 无

功能说明：

按格式输出日志，并退出。相当于调用Printf()并调用os.Exit(1)

代码实例：

	package main

	import(
		"log"
	)

	func main(){

		//log.Fatalf("%s", "hello")

		name := "golang"
		log.Fatalf("%8d,%8s", 23, name) //2013/03/10 16:08:49       23,  golang
	}

