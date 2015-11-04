# use_python

## Windows

### 安装
* (个人最推荐)使用[Winpython],自带了很多基础的包以及IDE，安装其它包也方便，而且是绿色版，这意味着你的电脑上可以同时共存不同版本的Python.
* [官方版][Python]


[Winpython]: https://winpython.github.io/
[Python]: https://www.python.org/

### 安装第三方库
* 推荐到[这个第三方网站][www.lfd.uci.edu]下载预编译好的包(注意Python版本，以及numpy建议用mkl版本)
* 如果上面这个网站搜不到，可以去[github]试试，见安装方法3.


[www.lfd.uci.edu]: http://www.lfd.uci.edu/~gohlke/pythonlibs/
[github]: https://github.com/
### 安装方法
1 (Winpython专有方法)找到你安装(解压)Winpython的目录，下面有个__WinPython Control Panel.exe__,直接把下载到的包文件(上面那个网站的.whl或者github上下到的.zip源码)拖进去点Install就好,少数情况会失败，可以使用方法2.

2 (使用pip安装.whl文件)在__CMD__里打开你的Python根目录，进入`\Scripts\`目录，确定里面有个__pip.exe__.(Winpython直接打开根目录下的__WinPython Command Prompt.exe__),执行如下代码:
``` shell
>>>pip install wheel
>>>pip install XXX.whl 
```
PS: 强烈不建议使用pip直接安装numpy等库，建议从上面提到的第三方网站下载预编译版本.

3 (使用github上发布的源码安装)github上一般项目主页都会写清楚安装方式，以下是常见情况
以[Pyserial]为例，打开主页，点击右侧Download ZIP下载源码(一般情况下不同python版本使用同一套代码)，在本地解压后，按照2.中的说明，找到需要安装python版本的根目录，执行:
``` shell
>>>python setup.py
```

[Pyserial]: https://github.com/pyserial/pyserial
## Linux
使用Linux的人应该不需要我比比了.



