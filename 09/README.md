解决在windows下无法打开JackCompiler.bat工具的问题
首先建立一个文件 命名为jc.cmd 输入
```
@echo off
pushd .
call F:\nand2tetris\tools\JackCompiler.bat %cd%\%1
popd
```
保存 将jc.cmd拖到你要执行命令的目录里
假设当前路径下有一个test目录或test.jack

打开命令行 输入
```
jc test
```
即可编译成功

PS: F:\nand2tetris\tools\JackCompiler.bat这个是你工具的路径

