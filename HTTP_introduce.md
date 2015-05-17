title: HTTP Insroduce
speaker: 元悲
url: https://github.com/ksky521/nodePPT
transition: cards
files: /js/demo.js,/css/moon.css

[slide]

# HTTP 协议简介
## 演讲者：元悲

[slide]

##
   3.1 HTTP 协议初探
    用户在地址栏中输入URL，到页面最终被加载完成。将会经历以下几个过程。
    1. parse URL.
    2. init REQUEST MESSAGE.
    3. send request message to server.[DNS resolve, TCP three way handshake]
    4. recieve first RESPONSE MESSAGE from server.
    5. parse html as mainframe.
    6. send subresource requests which parsed from step 5.
    7. build DOM,CSSOM,BOM.
    9. render the page. [Layout,Paint,Event Route]

[slide]

##
  URI, URL, URN
  URI: URI是以某种统一的（标准化的）方式标识资源的简单字符串,英文全称为（Uniform
Resource Indentifier, URI).
  URL:
  URN:
  *URL, URN是URI的两种不同的实现形式。*
[slide]

[slide]
## URL 的构成

[slide]

## request message && response message

[slide]

## HTTP Status Code

[slide]

   3.2 History
   3.3 HTTP 协议重要的组成部分
   3.3.1 Cache
       3.3.1 cache control 用的关键组件
       3.3.2 缓存验证过程（简要介绍）
       3.3.3 Refresh && Reload ，地址栏回车, Forward, Backword
       3.3.4 Chromium 缓存组成部分（HTTP 缓存，web kit 缓存，差异）
  3.3.2.连接管理
          Origin: <protocol ,scheme, port>
          Chromium  Socket Manager &&  Socket pool
          并行连接
          持久化连接 keep alive
          管道化连接

  3.3.3代理

  3.3.4 cookie
  3.4 HTTP/2
       3.4.1 History && Spdy
       3.4.2 HTTP协议要解决的主要问题
       3.4.3 协议介绍（图解)
       3.4.4 连接复用(one Origin one connect)
       3.4.5 请求优先级
       3.4.6 首部压缩
       3.4.7 Server Push

 3.5 参考资料
      HTTP 权威指南
      hpbn
