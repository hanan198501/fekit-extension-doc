FEKIT DOC
=====================

生成指定js文件的api文档，基于jsdoc（<http://usejsdoc.org/>）。


##安装##

首先全局安装扩展：

    npm install -g fekit-extension-doc

在安装的fekit-extension-doc的目录中，执行：

    node scripts/postinstall.js

然后再命令行输入fekit，就可以看到doc指令了。


##用法##

修改fekit.config文件，增加"docs"字段，用来指定需要生成文档的js列表，js路径的根目录为当前项目的src目录，例如：

    "docs": [
        "Popup.js",
        "scripts/common/base/QClass.js"
    ]

命令行执行：

    fekit doc

即可在docs目录下生成api文档。

也可以指定文档生成目录：

    fekit doc -d mydocs

即可在mydocs目录下生成api文档。

