# random-question-vue

### 简介

        这个一个全平台的随机出题的题库, 有单选, 多选, 判断题三种题型, 暂无错题回顾等等需要数据库的功能,为了兼容全平台,基于html, 数据库直接使用json本地文件.这导致了一个缺点: 数据库很容易泄漏, 使用于不怕题库泄漏的情况.

        有win-exe, html,apk,ipa版本

### 前言

+ 本项目基于https://github.com/fanmingfei/random-question-vue

+ 由于项目是基于vue前端框架, ie11不支持, 推荐使用非ie浏览器打开

+ exe由于不能使用系统的IE的接口内核使用的是 wke

+ apk/ipa 使用的是H5Buider的云打包, 方便快捷, 也可以使用其他的在线云打包, 很方便.默认的图标和配置, 没有修改

+ apk/ipa 也可以使用其他的反编译工具进行反编译替换问题数据库

  

### 数据库

+ 是一个questions.js的文件, 位于js文件中中 也可以说是一个json

+ 原作者在tool文件夹中有aaa.js用于处理a.txt

+ 由于a.txt的格式过于苛刻, 做了一个转换工具JsonTool.exe

#### JsonTool.exe 使用

+ 打开Model.xlsx, 分三个插页,单选, 多选, 判断题, 编辑完后拖入JsonTool.exe, 依次选择对应插页和类型进行导入,

  然后点击生成, 会生成一个带时间的.js的文件, 可以选择是否直接替换替换js/questions.js

  

### 使用方法

1. 参考数据库部分,生成自己的数据库后替换questions.js

2. 可以直接用非IE浏览器(如edge, chrome,360)打开.或者放服务器上

3. 需要exe的找exe文件夹,apk找apk文件夹


