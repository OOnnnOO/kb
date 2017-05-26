# curl

## 命令参数

显示输出内容

```
curl http://example.com
```

`-i` 输出响应头信息和内容

```
curl -i http://example.com
```

`--head` `-I` 输出响应头信息

```
curl --head http://example.com
curl -I http://example.com
```

`--header` `-H` 设置请求头信息

```
# 模拟设置请求源域名
curl -H "Origin: http://www.google.com" -X POST -d "page=1" http://example.com
```

`-o` 输出内容到文件，另存为

```
curl http://example.com/hello.txt -o hello.txt
```

`-O` 输出内容到文件，保持原文件名

```
curl -o http://example.com /hello.txt
```

`-d` 设置POST请求中的data

POST请求

```
curl -d "title=hello&&body=hello world" http://
```

`-X` 设置请求方式

put请求

```
curl -X PUT -d "title=hello&&body=hello world" http://
```

`-L` 跟踪跳转（Follow redirects）

```
curl http://google.com
curl -L http://google.com
```

`-u` 文件传输

上传

```
curl -u user@example.com:123456 -T hello.txt ftp://ftp.expample.com
```

下载

```
curl -u user@example.com:123456 -o hello.txt ftp://ftp.expample.com/hello.txt
```

## 参考
https://www.youtube.com/watch?v=7XUibDYw4mc
