title: HTTP Insroduce
speaker: 元悲
url: https://github.com/ksky521/nodePPT
transition: cards
files: /js/demo.js,/css/moon.css

[slide]

# HTTP 协议简介
## 演讲者：元悲

[slide]

## HTTP 协议初探
用户在地址栏中输入URL，到页面最终被加载完成。将会经历以下几个过程。

1. Parse URL.
2. Init REQUEST MESSAGE.
3. Send request message to server.[dns resolve, tcp three way handshake]
4. Recieve the first RESPONSE MESSAGE from server.
5. Parse html as mainframe.
6. Send subresource requests which parsed from step 5.
7. Build DOM,CSSOM,BOM.
8. Render the page. [Layout,Paint,Event Route]

[slide]

## URI, URL, URN
  URI: URI是以某种统一的（标准化的）方式标识资源的简单字符串,英文全称为（Uniform
Resource Indentifier, URI).
  URL:
  URN:
  **URL, URN是URI的两种不同的实现形式。**

[slide]
## URL 的构成

[slide]

## REQUEST message && RESPONSE message

[slide]

## HTTP Status Code

[slide]

## History of HTTP

[slide]

## HTTP 协议重要的组成部分
### Cache
1. cache control 用的关键组件
2. 缓存验证过程（简要介绍）
3. Refresh && Reload ，地址栏回车, Forward, Backword
4. Chromium 缓存组成部分（HTTP 缓存，web kit 缓存，差异）

[slide]

## 连接管理
1. Origin (protocol ,scheme, port>
2. Chromium  Socket Manager &&  Socket pool
3. 并行连接
4. 持久化连接 keep alive
5. 管道化连接

[slide]

##代理

[slide]

## Cookie

[slide]

## HTTP/2
1. History && Spdy
2. HTTP协议要解决的主要问题
3. 协议介绍（图解)
4. 连接复用(one Origin one connect)
5. 请求优先级
6. 首部压缩
7. Server Push
8. SSL 是否是必须的？
9. ALPN

[slide]

## 参考资料
1. RFC 
2. HTTP 权威指南
3. [High Perfermance Browser Network](http://chimera.labs.oreilly.com/books/1230000000545/index.html)
4. Chromium Network

[slide]

## Q&A

