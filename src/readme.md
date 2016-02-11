
## tornado 源码版本:


- [releases](https://github.com/tornadoweb/tornado/releases)


### 1.0.0 版本:

- on 23 Jul 2010

## 注解进度:

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


### 4.2.0 版本:

- on 27 May 2015

## 注解进度:

- 待更新



## 版本源码文件对比:


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
