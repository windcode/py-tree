# py-tree
一个 python 的练习树。

这里是我练习 python 的地方，提供有各种用来练手的 python 小项目。

希望自己像一个 little monkey 一样 **爬上 python 大树的顶端**。

## 使用方法
1. clone 代码到本地
```
git clone https://github.com/WangHaizhen/py-tree.git
```
2. 编写对应题目代码，命名规则为 **项目编号.py**  
栗子：  
第二题代码文件 ---> 1_1.py

3. 编写完成，push 到 github
```
git add .
git commit -m 'update 1_1.py'
git push origin master
```

**说明**：题号为 x_x 表示还没想好题号。

## 项目清单

### 1.剔除一个字符串中的所有空格
#### 功能描述：
对字符串变量 s 进行处理，剔除字符串中的所有空格，并输出。

#### 输入：
```
s = '    123  4567    8   '
```
#### 输出：
```
'12345678'
```

### 1_1.IP地址拼接
#### 功能描述：
IP 地址由四个 0~255 的数字组成，比如：192.168.12.34，现在只给你四个数字，你需要将他们拼接起来，组成 IP 地址的形式，并输出。

要求对每个数字进行检测，每个数字的范围为 0~255，通过检测，输出拼接后的形式。

没有通过检测，输出提示 **'[Error]: cannot compose IP address.'**

#### 输入：
```

192 168 12 34

0 0 0 0

234 345 456 567

-1 -1 -1 -1

```
#### 输出：
```

192.168.12.34

0.0.0.0

[Error]: cannot compose IP address.

[Error]: cannot compose IP address.

```

### 1_2.URL地址拼接
#### 功能描述：
URL 地址又称 **Uniform Resoure Locator，即 统一资源定位器** ，是万维网上定位资源（比如html页面）的方式，它通常的组成是：

**protocol:// hostname[:port] / path /** ，即  
**协议://主机[:端口号]/路径/**
([] 表示可选)

举个栗子：
>**http://www.test.com:8000/index.html**  
**http://www.test.com:8080/login.php**  
**ftp://45.67.89.01:21/test.jpg**

我们把这个问题简化，现在有一个网络资源 **love.png** ，给你找到它的 **协议、组成主机IP的四个数字、端口号**，你需要把他们拼接成 URL 格式，并输出。

**特殊要求**：拼接 IP 地址要调用 1_1 中写的模块。

#### 输入：
```
ftp 45 67 89 01 21 love.png
ftp 456 678 890 012 21 love.png
```
#### 输出：
```
ftp://45.67.89.01:21/love.png
[Error]: cannot compose IP address.
```

### 1_3.转换IP地址为二进制形式
#### 功能描述：
给你一个IP地址，你要将它转换为二进制形式，并输出

如果转换之后的IP地址不符合格式，即每个字段数字范围不在 0~255 之间，则输出：**'[Error]: Not an IP address.'**

**特殊要求**：将检测IP地址的功能封装为一个模块，可以供其它文件调用。

#### 输入：
```
0.0.0.0
1.1.1.1
5.6.5.6
192.168.10.15
251.165.145.167
```

#### 输入：
```
0.0.0.0
1.1.1.1
101.110.101.110
11000000.10101000.1010.1111
11111011.10100101.10010001.10100111
```

### x_x.电影名净化器
#### 功能描述：
我们下载电影到本地后，名字通常会带有网站的广告标记，你需要将其中的广告部分净化掉。看看栗子你就明白了~

使用场景：双击运行净化器，同一文件夹下的电影文件的名字会被净化。

带广告标记的电影文件我已经准备好啦！快去净化它们吧。

#### 输入：
```
[电影天堂 www.dytt8.net]海上钢琴师.mp4
【电影天堂 www.dytt8.net】.肖申克的救赎.mp4
【飘花电影】 -你的名字 新海诚.avi
千与千寻 宫崎骏【飘花电影 www.piaohua.com】.rmvb
```
#### 输出：
```
海上钢琴师.mp4
肖申克的救赎.mp4
你的名字 新海诚.avi
千与千寻 宫崎骏.rmvb
```


施工中……

