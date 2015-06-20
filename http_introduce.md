title: HTTP Insroduce
speaker: 元悲
url: https://github.com/ksky521/nodePPT
transition: cards
files: /js/demo.js,/css/moon.css

[slide]

# HTTP 协议简介
## 演讲者：元悲

[slide]

## Outline
1. HTTP 协议初探
2. HTTP 协议重要的组成部分
3. HTTP/2 简介 

[slide]

## What is HTTP Protocol?

>  The Hypertext Transfer Protocol (HTTP) is an application-level
   protocol for distributed, collaborative, hypermedia information
   systems. It is a generic, stateless, protocol which can be used for
   many tasks beyond its use for hypertext, such as name servers and
   distributed object management systems, through extension of its
   request methods, error codes and headers [47]. A feature of HTTP is
   the typing and negotiation of data representation, allowing systems
   to be built independently of the data being transferred.

   [rfc2616](https://www.rfc-editor.org/rfc/rfc2616.txt)

[slide]

## HTTP 协议初探
用户在地址栏中输入URL，到页面最终被加载完成。
将会经历以下几个过程。

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
1. URI: URI是以某种统一的（标准化的）方式标识资源的简单字符串
2. 英文全称为（Uniform Resource Indentifier, URI).
3. URL: 统一资源定位符（或称统一资源定位器/定位地址、URL地址)

 ![URL 是怎样与浏览器、客户端、服务器以及服务器文件系统中的位置进行关联的如下图](http://www.ituring.com.cn/figures/2013/HTTP_The%20Definitive%20Guide/06.d02z.01.png)

[slide]

  URN: 统一资源名称（URN）是统一资源标识（URI）的历史名字
  它使用urn:作为URI scheme。

       urn:NID:NSS

       urn:uuid:6e8bc430-9c3a-11d9-9669-0800200c9a66

  **URL, URN是URI的两种不同的实现形式。**

[slide]

## [URL 的构成]

 **scheme://[user:password@]domain:port/path?query_string#fragment_id**

1. scheme: ftp,http,https,file
2. domain: IP(IPV4,IPV6), domain(like uc123.com)
3. query_string: ?first_name=John&last_name=Doe
4. fragment_id: 表明了一个页面的某一个部分

   http://chimera.labs.oreilly.com/books/1230000000545/ch12.html#_brief_history_of_spdy_and_http_2

[slide]

## REQUEST message && RESPONSE message

请求报文和响应报文的格式基本相同，由如下三个部分组成

1. Start line
2. Headers
3. Body

[slide]

**Requset Method -- Request URL -- Client Version**

![request message](http://blog.codenginx.org/images/request_message.png)

[slide]

**Server Version -- Status Code -- Reason Phrase**

![response message](http://blog.codenginx.org/images/response_message.png)

[slide]

## HTTP  Method

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

## Cookie
1. Cookie 的基本构成
2. Path,domain 的作用
3. Set Cookie2
4. Cookie 与缓存

[slide]

##代理
1. 代理的类型
2. 客户端代理与反向代理
3. 

[slide]

## 连接管理
1. Origin (protocol ,scheme, port>
2. Chromium  Socket Manager &&  Socket pool
3. 并行连接
4. 持久化连接 keep alive
5. 管道化连接

[slide]

## HTTP/2
1. History && Spdy
2. HTTP/2协议要解决的主要问题（为什么会有HTTP/2)
3. 协议介绍（图解)
4. 连接复用(one Origin one connect)
5. 请求优先级
6. 首部压缩
7. Server Push
8. SSL 是否是必须的？
9. ALPN
10. HTTP/2的实现

[slide]

## 参考资料
1. RFC 
2. [HTTP 权威指南](http://www.ituring.com.cn/book/844)
3. [High Perfermance Browser Network](http://chimera.labs.oreilly.com/books/1230000000545/index.html)
4. Chromium Network
5. HTTP/2 相关的参考（集合）

[slide]

## Q&A

