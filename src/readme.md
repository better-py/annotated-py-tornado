
## tornado 源码版本:


- [releases](https://github.com/tornadoweb/tornado/releases)
- 版本规律:
    - v1.x, v2.x, v3.x, v4.x, 当大版本更新时, 代码增长量, 比较多
    - v1.x 的 小版本更新时, 通常是修复 bug, 代码增长量, 比较少.
    - 选择阅读版本技巧:
        - 选定 某个大版本号, 如 v2.1
        - 选择该大版本号号下, 最后一个小版本, 如 v2.1.10


### 1. 各版本代码统计对比:

- [v1.0.0](https://github.com/tornadoweb/tornado/releases/tag/v1.0.0): 
    - 代码行数: 6207 (少量测试代码,忽略)
    - date: on 23 Jul 2010 
    - 阅读指数: ✖✖✖✖ (版本过老, 不推荐)
- [v2.1.0](https://github.com/tornadoweb/tornado/releases/tag/v2.1.0):
    - 代码行数: 9981 (含 gen.py 模块)
    - date: on 21 Sep 2011 
    - 阅读指数: ✖✖✖✖ (不推荐)
        - 对比 v2.1.1, 无优势
- [v2.1.1](https://github.com/tornadoweb/tornado/releases/tag/v2.1.1):
    - 代码行数: 12720 - 2721(测试代码) = 9999
    - date: on 5 Oct 2011
    - 阅读指数: ✖✖✖✖ (不推荐)
        - 对比 v2.2.0, 无优势
- [v2.2.0](https://github.com/tornadoweb/tornado/releases/tag/v2.2.0):
    - 代码行数: 13654 - 3202(测试代码) = 10453
    - date: on 31 Jan 2012
    - 阅读指数: ✔✔ (可选)
- [v2.4.1](https://github.com/tornadoweb/tornado/releases/tag/v2.4.1):
    - 代码行数: 15174 - 4145(测试代码) = 11029
    - date: on 25 Nov 2012
    - 阅读指数: ✔✔✔ (可选)
- [v3.1.0](https://github.com/tornadoweb/tornado/releases/tag/v3.1.0): 
    - 代码行数: 21242 - 7377(测试代码) = 13865
    - date: on 16 Jun 2013 
    - 阅读指数: ✖✖✖✖ (不推荐)
        - 对比 v3.2.0, 无优势
- [v3.2.0](https://github.com/tornadoweb/tornado/releases/tag/v3.2.0):
    - 代码行数: 22222 - 7873(测试代码) = 14349
    - 重大更新: 修改了很多文件
    - date: on 14 Jan 2014 
    - 阅读指数: ✖✖✖✖ (不推荐)
        - 对比 v3.2.2, 无优势
- [v3.2.2](https://github.com/tornadoweb/tornado/releases/tag/v3.2.2): 
    - 代码行数: 22680 - 8107(测试代码) = `14573`
    - date: [on 4 Jun 2014]()
    - 阅读指数: ✔✔✔✔ (较推荐)
        - 本版本为 3.x 最后一个版本
            - 本版本 docs 可知有 python 3.4 测试
            - 包含 asyncio 模块: tornado.platform.asyncio
            - [asyncio 参考](http://www.liaoxuefeng.com/wiki/0014316089557264a6b348958f449949df42a6d3a2e542c000/001432090954004980bd351f2cd4cc18c9e6c06d855c498000)
            - asyncio是Python 3.4版本引入的标准库，直接内置了对异步IO的支持
            - asyncio的编程模型就是一个消息循环
        - 下一版本为 4.x 系列
        - 交叉时间对比: 
            - `python 3.4.1 final`: [May 18, 2014](https://www.python.org/dev/peps/pep-0429/#id1)
            - `python 3.4.4 final`: [December 20, 2015](https://www.python.org/dev/peps/pep-0429/#id3)
- v4.2.0:
    - 代码行数: 29851 - 12027(测试代码) = 17824



### 2. 注解版本选择:

#### 2.1 版本 v1.0.0:

##### 注解进度:

- 2016-02-11:
    - tornado 1.0.0 版本的 主要模块代码,基本完成注解.
    - 重要模块:
        - ioloop.py       # 已注解
        - web.py          # 已注解
        - iostream.py     # 部分注解
        - httpserver.py   # 已注解
        - template.py     # 部分注解
        - wsgi.py         # 部分注解
    - 其他非重要模块:
        - auth.py         # 支持第三方登录的模块
        - database.py     # ORM简单实现
        - httputil.py     # http头解析处理

#### 2.2 版本 [v3.2.2](./src/tornado-3.2.2/):
- 2016-08-13:
    - 多版本对比后, 决定重点注解此版本.
    - 后续会更新详细注解, 模块结构剖析图等.


#### 2.3 版本 v4.2.0:

- 待更新




### 3. 版本源码文件对比:


```
#----------------------------------------------
#             1.0.0 版本文件
#----------------------------------------------

# 1.0 版本
staff   637B Jul 22  2010 __init__.py
staff    36K Jul 22  2010 auth.py
staff   3.5K Jan 22 16:58 autoreload.py
staff   3.8K Jul 22  2010 escape.py
staff    29K Jul 22  2010 httpclient.py
staff    17K Jan 22 16:58 httpserver.py
staff   4.4K Jul 22  2010 httputil.py
staff    18K Jan 22 16:58 ioloop.py
staff   8.7K Jul 22  2010 iostream.py
staff    19K Jul 22  2010 locale.py
staff    13K Jul 22  2010 options.py
staff    18K Jul 22  2010 template.py
staff    57K Jan 22 16:58 web.py             # 核心文件
staff    11K Jul 22  2010 wsgi.py

# 4.x 版本中删除
staff   5.8K Jul 22  2010 database.py        -
staff   4.2K Jul 22  2010 win32_support.py   - 
staff   9.4K Jul 22  2010 s3server.py        -



#----------------------------------------------
#             4.2.0 版本文件
#----------------------------------------------

# 相同部分
staff   1.1K Jan 22 16:57 __init__.py
staff    43K Jan 22 16:57 auth.py
staff    12K Jan 22 16:57 autoreload.py
staff    14K Jan 22 16:57 escape.py
staff    26K Jan 22 16:57 httpclient.py
staff    12K Jan 22 16:57 httpserver.py
staff    29K Jan 22 16:57 httputil.py
staff    40K Jan 22 16:57 ioloop.py                  # 核心模块
staff    63K Jan 22 16:57 iostream.py
staff    23K Jan 22 16:57 locale.py
staff    20K Jan 22 16:57 options.py
staff    30K Jan 22 16:57 template.py
staff   122K Jan 22 17:07 web.py                     # 核心模块
staff    40K Jan 22 16:57 websocket.py
staff    13K Jan 22 16:57 wsgi.py


# 新增
staff    18K Jan 22 16:57 concurrent.py              +
staff    21K Jan 22 16:57 curl_httpclient.py         +
staff    36K Jan 22 17:19 gen.py                     + 核心模块
staff    30K Jan 22 16:57 http1connection.py         +
staff    13K Jan 22 16:57 locks.py                   +
staff   9.6K Jan 22 16:57 log.py                     +
staff    20K Jan 22 16:57 netutil.py                 +
staff    12K Jan 22 16:57 process.py                 +
staff   8.9K Jan 22 16:57 queues.py                  +
staff    23K Jan 22 16:57 simple_httpclient.py       +
staff    13K Jan 22 16:57 stack_context.py           +
staff   6.6K Jan 22 16:57 tcpclient.py               +
staff    11K Jan 22 16:57 tcpserver.py               +
staff    26K Jan 22 16:57 testing.py                 +
staff    12K Jan 22 16:57 util.py                    +


    

```
