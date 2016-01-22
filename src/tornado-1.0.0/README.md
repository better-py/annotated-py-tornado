


## 1.0.0 注解备忘:


- 此版本的代码,是python2.x的, 当在pycharm中阅读时,项目环境不要设置成python3.
- 为方便阅读, 删除了 批注源码文件 的 LICENSE 说明, 请注意尊重版权.
- 项目原有模块,函数的英文注释,根据需要,会作中文翻译.
- 本版本 tornado 主体框架 Python 代码行数: `6023` (含注释)
    - 代码量,比想象中的少,很精简,很有必要花时间精读一下
    - 剔除 Demo 示例代码
    - 本版本 单元测试代码,忽略不计
- 统计代码行数命令: find . -name "*.py" | xargs grep -v "^$" | wc -l


- 阅读入口:
    - tornado/web.py









---



# 原项目 Readme 说明:

Tornado
=======
Tornado is an open source version of the scalable, non-blocking web server
and and tools that power FriendFeed. Documentation and downloads are
available at http://www.tornadoweb.org/

Tornado is licensed under the Apache Licence, Version 2.0
(http://www.apache.org/licenses/LICENSE-2.0.html).

Installation
============
To install:

    python setup.py build
    sudo python setup.py install

Tornado has been tested on Python 2.5 and 2.6. To use all of the features
of Tornado, you need to have PycURL and a JSON library like simplejson
installed.

On Mac OS X, you can install the packages with:

    sudo easy_install setuptools pycurl==7.16.2.1 simplejson

On Ubuntu Linux, you can install the packages with:

    sudo apt-get install python-pycurl python-simplejson
