# node
node.js
==原生js没有consloe.log()==

---

##### 自动加载的内置模块：
- console
- gloabal
- model
- process

---
##### 本地化存储5种方式：
- local storage
- session storage
- cookie
- 

```
local storage和session storage所存储的数据长度远远大于cookie
cookie可以携带数据与服务器进行。。。而另外两个不可以

```

---
##### 软刷新VS硬刷新
软刷新F5

硬刷新CTRL+F5

如何检验--哈希值

---
##### ES6面试必问

---
##### 回调函数事件循环队列
###### 调用时间循环队列条件：
- 当前进程空闲
- 满足触发条件：

```
时间条件，
磁盘I/O，
网络I/O，
自定义事件
```

---
==基于对象，面向对象==

---
##### http协议四大关键字：
get  
post

put    

delete
###### get VS post:
get最多传送4096个字节；

```
1 byte = 8 bit;
1 int = 2 4 8 byte(取决于电脑配置)
```
---
##### 使用http创建webserver（request、response）：
PHP：Apache、Niger

java：Tomcat、

---
##### 数据包：
包头+包体

---
##### 三码一体：
- 文件编码：

```
ANSI 
unicode 
utf-8
```

- 浏览器解码

```
gbk
gb2312
gb18030
```

- 数据库编码

---
- ==Function与Object互为子集==

---
- ==function都有原型链prototype==

---
- ==eval()可以将string变成object==

---
- ==前端安全问题，跨栈攻击==

---

- ==输入过滤，输出过滤==

---

- ==JSON.parse所构造的字符串必须外面单引里面双引，stringfy也是，而eval不用==

---

- ==promise解决容错问题（比如两条验证短信）==

---

- ====异步逻辑叠加过多时会出现回调深渊问题，解决回调深渊可以用async包====

---

- ==回调函数可以是同步的，也可以是异步的==

---

- ==require可以把文件变成模块==

---
##### 直接赋值VS引用赋值:
- 弱类型语言不同于强类型，不能

---
##### （将方法公布于外部）module.exports VS exports:
- module.exports 初始值为一个空对象 {}
- exports 是指向的 module.exports 的引用
- require() 返回的是 module.exports 而不是 exports
- 

---
#### 前端抓包分析
- ==user-agent：==

```
User Agent中文名为用户代理，简称 UA，它是一个特殊字符串头，使得服务器能够识别客户使用的操作系统及版本、CPU 类型、浏览器及版本、浏览器渲染引擎、浏览器语言、浏览器插件等。
多数网站从而借此获取用户喜好
```

- ==referer：==

```
HTTP中的Referer是header的一部分，当浏览器向web服务器发送请求的时候，一般会带上Referer，告诉服务器我是从哪个页面链接过来的，服务器基此可以获得一些信息用于处理。 
简而言之，HTTP 
Referer是header的一部分，当浏览器向web服务器发送请求的时候，一般会带上Referer，告诉服务器我是从哪个页面链接过来的，服务器藉此可以获得一些信息用于处理。比如从我主页上链接到一个朋友那里，他的服务器就能够从HTTP 
Referer中统计出每天有多少用户点击我主页上的链接访问他的网站。
```

---
==IP地址转十进制==

---
##### mime头：
409种文件格式

---
##### 
1. server读取文件到内存  
--处理路径？URL
2. 把内存数据变成数据包
3. 发送数据包并结包

---
##### get
1. url
2. a标签href  --href属性
3. iframe            src
4. form get
5. $.get
6. curl

---
##### post
1. from post
2. $.post
3. curl


---
##### get和post均可的：
- request
- 

---
##### 跨域
###### 同源策略：
- 协议相同
- 域名相同
- 端口号
- （三者中有一个不同就跨域）
###### 跨域：
- 前端跨域

```
（1）iframe跨域
（2）posemessage()
 (3)getJson()
```

```
cookie（name，value，expire，'/'，'www.baidu.com'，false，true）
httponly = true
```

- 后端跨域

```
（1）Alllow-origin 4项配置
（2）cors跨域
```

---
##### node.js模块
- 内置系统模块
- 

---
##### node.js的好处
- 做中间层处理
- 解决高并发问题
- 将前后端较好的分离
- 代码不耦合，开发效率降低
###### 缺点：
- 新增加的一层使传输效率降低--如何改善：通过UDP做服务器改善处理(官网dgram数据报---内置系统模块)

---

1. 十二个文档必看
1. 面向对象+语法专题必看（定时器） 

---
##### buffer模块
浏览器转码
- urlencode---浏览器url转码
- iconv---ajax转码
- json_encode---json转码
- base64_encode---base64转码
- buffer---十六进制---utf-8,gbk

---
##### child_process
- supervisor----热更新
- pm2(包)

---
##### cluster
- 集群

---
##### console---控制台
- console.count--全局计数


---
##### 加密crypto

 常见方式：
 
- md5----加密后的密文等长
- rc6
- (单项不可逆)
- sha1,sha265
- rsa

---
##### dgram---udp服务器


---
##### dns

---
##### Error

---
##### events----继承

---
##### fs

```
rename
stats
readfile
```
---
##### global

---
##### http

---
##### https

ssl

---
##### module

---
##### net
- tcp服务器
- 关键字

---
##### OS操作系统

---
##### path
- join---静态资源管理器

---
##### process

---
##### querystring

---
##### readline,repl(基本不考)

---
##### url

---
##### util
- inherit


---

##### stream(不考)


---
##### Apache
创建文件要创建到

---
###### formidable
node文件上传

---
###### pipe管道流
既可写入，也可读出

---
###### 异步的两个条件：

异步，回调重点，waterfall

---
###### 加载顺序async
解决异步核心js下的promise
- 解决异步回调用async:
- 三个主要方法：waterfall，

---
==如果本地缓存把cookie禁用，session失效==
- session-id永远保持不变
- session服务器端，cookie存在于客户端


---
#### 项目创建：
1. 新建文件，安装相关。。。
2. 进入文件
3. 进行文件改造
4. 

---
###### 
-save会自动将所安装包写到dependensice下


---
##### 数据库的四种基本操作：

- 


---
###### 密码加密处理crypto

---
###### socket.io
node实时服务框架

- app.use----建立全局函数
- app.set----建立全局变量
- express的数据要建立成对象进行传递
- express渲染模板：ejs,jade,template
- json_encode();---php通过此方法将数组转化成对象字符串；
- 响应方法不一样就不需要担心冲突


#PHP

##### PHP数据类型
- 4种标量类型：

```
int 
float
string 
bool
```
- 2种复合类型：

```
array
object
```

- 2种特殊类型：

```
null 
resource
```
##### 几种输出类型：

```
echo
print_r
var_dump
```
###### 前端渲染
- 前端渲染是将数据和模板在前端完成打包处理
- 后端渲染是在后端完成这项
- 前端渲染的好处是模板一次打包传回，而数据可以进行多次渲染，如Vue，但可能因网速问题出现卡白现象

###### PHP源码输出：

```
echo "</pre>";
```
###### PHP中可以嵌入HTML和JavaScript，HTML也可以嵌入PHP，但是JavaScript不能嵌入PHP

###### NULL+1 = 1
但数据库是例外，数据库中等于字符串，不能相加

###### CI--MVC框架
- Model---
- Controller---
- View---
- URL辅助函数site_url
- autoload下配置的内容全局生效

```
graph LR
view-->controller
```
###### get:
1. a标签
2. form
3. ajax    get
4. url
5. iframe
6. curl
###### post
1. form
2. ajax    post
3. curl
###### get接收：
1. $_GET
2. $this->input->get
3. $this->uri->segment()
###### post接收：
1. $_POST
2. $this->input->post()

```
graph LR
controller-->view
```
1. $this->load->view('页面名',$data);
2. $this->session->userdata()
3. $this->load-vars(变量名)

```
graph LR
controller-->model 
```
？
1. $this->load->model(model名)
2. $this->model名->model方法

```
graph LR
A-->B
```
==有return的叫方法，没renturn的叫过程==
1. return   $query->->row()
2. return   $query->result()
###### model:
- 需求翻译成SQL语句
- select
- delete
- update
- insert

==看underscore库==

---
###### PHP的几种方法：
- $_POST
- $_SESSION
- $_COOKIE
- $_GET
- $_SEVER
- $_ENV
- $_FILES
- $_REQUEST



