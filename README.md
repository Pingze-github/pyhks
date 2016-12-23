# pyhks
A Python package for hotkey controls. 一个用于热键控制的Python库。

## Installation
Just put the "cprint.py" into your dir ".../Python/Lib", or in your project.

将“cprint.py”放入Python安装目录".../Python/Lib"，或者项目文件夹中。

## Rely on
```
pip install pyHook
pip install pythoncom
pip install pywin32  
```

## Usage
```
from pyhks import pyhks
def foo():
    print('do something')
dic={
    foo: ['F1','Lmenu'] # press left alt and F1 at the same time
}
p = pyhks(dic)
p.start()
```

## 其他
自己用PyQt4开发小软件时，发现使用pyhk会让程序卡死（原因不明），就写了这个。
监听程序运行在单独的线程上。
