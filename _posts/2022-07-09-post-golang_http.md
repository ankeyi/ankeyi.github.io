# src: golang Document
## Overview
package http provides HTTP client and server implementations
Get、Head、Post and postForm make HTTP(or HTTPS) requests:
```go
respon, err :=http.Get("https://likeni.org")

resp, err := http.Post("http://example.com/upload", "image/jpeg", &buf)

resp, err := http.PostForm("http://example.com/form", url.Values{"key": {"Value"}, "id": {"123"}})
// path = /usr/local/go/src/net/http/client.go 
// 阅读http.Get源码发现该函数调用并返回client.go文件中默认定义的 DefaultClient结构体变量中的Get方法，
func Get(url string) (resp *Response, err error) {
	return DefaultClient.Get(url)
}
//  DefaultClient结构体变量是



```
