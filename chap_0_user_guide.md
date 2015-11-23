#Bottle 文档
版本：Release 0.12.9
作者Marcel Hellkamp
时间：2015-11-15

译者：Tacey Wong
时间：2015-1-

##目录

### 1 、用户指南

+ 1.1 初始教程
+ 1.2 配置（草案）
+ 1.3 请求路由
+ 1.4 简单模板引擎
+ 1.5 API参考
+ 1.6 可用插件列表

###2、 知识库

+ 2.1 基础教程：Todo-List应用（待办事项列表应用）
+ 2.2 异步基础应用
+ 2.3 食谱
+ 2.4 常见问题

###3、 开发于贡献

+ 3.1 发行说明与修改
+ 3.2 贡献者
+ 3.3 开发者笔记
+ 3.4 插件开发指南
+ 3.5 可用插件列表


###4、 许可证

###Python模块索引
###索引

Bottle是一个快速，简单和轻量级Python WSGI微Web框架。它作为一个单一的文件模块分配无依赖性比其他的Python标准库。

+ 路由：请求以支持为干净和动态链接的功能调用映射。
+ 模板：快速和Python的内置模板引擎支持的灰鲭鲨，jinja2和猎豹模板。
+ 工具：方便的访问表数据，文件上传，饼干，标题和其他HTTP相关的元数据。
+ 服务器：内置的HTTP服务器和支持发展为膏，fapws3，Bjoern，谷歌App Engine，CherryPy
或其他HTTP服务器WSGI能够。

***示例***: Bottle的“Hello World”

```python 
from bottle import route, run, template

@route(’/hello/<name>’)
def index(name):
    return template(’<b>Hello {{name}}</b>!’, name=name)

run(host=’localhost’, port=8080)
```
运行这个脚本，或将其粘贴到一个Python控制台。接着从浏览器打开http://localhost:8080/hello/world。你就会看到结果了。

###下载和安装

可以通过PyPI（easy_install -U bottle)）安装最新稳定版本，或者下载bottle.py（不稳定）放置在你的工程目录。























