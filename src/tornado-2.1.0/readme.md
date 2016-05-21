

## 关于 tornado 2.1.0 说明:

- 这个版本是首次添加 gen.py 模块, 所以,已此版本为准,进行源码注解.
- 2.x.x 系列版本, gen.py 文件变化不大.





## 原 readme 内容:


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
of Tornado, you need to have PycURL and (for Python 2.5 only) simplejson
installed.

On Mac OS X 10.6, you can install the packages with:

    sudo easy_install pycurl

On Ubuntu Linux, you can install the packages with:

    # Python 2.6
    sudo apt-get install python-pycurl

    # Python 2.5
    sudo apt-get install python-dev python-pycurl python-simplejson

