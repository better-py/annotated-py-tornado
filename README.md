# tornado-annotated

- tornado 源码 注解

## 1. 项目说明:

1. 对 tornado 框架 源码,添加学习注释
2. 目前选择的版本:
    - 1.0.0    这是 tornado 的第一版,代码应该是最简洁的
    - 4.2.1    简单对github 上 使用 tornado 框架的 版本,进行初步统计,发现使用该版本的项目最多.
    - 故不再选择 2.x, 3.x 的版本 学习注解
     

## 2. 本项目结构:

- 会包含tornado框架的结构剖析.
    - 包括 思维导图等工具制作的笔记
    - 参考阅读文档
    - tornado 核心模块源码重点剖析
    


## 3. tornado 源码版本:


- [releases](https://github.com/tornadoweb/tornado/releases)
- 版本规律:
    - v1.x, v2.x, v3.x, v4.x, 当大版本更新时, 代码增长量, 比较多
    - v1.x 的 小版本更新时, 通常是修复 bug, 代码增长量, 比较少.
    - 选择阅读版本技巧:
        - 选定 某个大版本号, 如 v2.1
        - 选择该大版本号号下, 最后一个小版本, 如 v2.1.10


## 4. 各版本代码统计对比:

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

