https://ydos.ymxer.com/
# 别像弱智一样提问 | Not be YXDS

Stop-Ask-Questions-The-Stupid-Ways & Not-Be-YXDS

## 短域名服务

https://ydos.ymxer.com/

+ https://git.io/how-to-ask
+ https://git.io/asking-question
+ https://git.io/stop-stupid


## 你真的准备好了吗？


> 感谢群友 `for you` 提供

## 避免 xy-problem

+ 参考地址: http://xyproblem.info/

`XY Problem` 表示
1. 提问者想要解决 **原问题 X** ，且觉得解决了 **引申问题 Y** 就能解决 **X** 问题
2. ~~提问者对外提出了解决 **Y** 的的请求~~
3. 回答者帮助提问者解决 **Y** 问题。（浪费了回答者和提问者双方的时间）

> `然而, 最终 Y 问题可能并不是 X 问题的一个合适的解决方法`

因此， 提问者要避免创造这样的修罗场, 需要学会在问题之初就准确描述自己的根本问题。 [学会描述问题](#学会描述问题)

## 提问前你必须需要知道的事情

1. 要知道， `Free` 的正确翻译是 `自由`，而非 **~~`免费`~~**。
1. 要知道，愿意回答问题的人，都是 **可爱** 的人。
1. 要知道，向帮助你的人 `付费` 是一个高尚的行为。即使回答你的人不是为了钱。
1. 要知道，`花钱买时间是一个常识`。如果你不能认同，要么你钱包穷，要么你思想穷。
1. 要知道，给对方发工资的不是你或者你老板。
1. 要知道，提问的时候你才是 **孙子**，帮助你的人是 **大爷**。
1. 要知道，不回答你的问题对其他人没有任何损失。
1. 要知道，`准确描述一件事情`是一项基本生存技能。要学会 [《提问的智慧》](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/master/README-zh_CN.md)
1. 要知道，`搜索`是一项基本生存技能，学不会用 Google 的话，你可能真的不适合你所从事的行业。
1. 要知道，`英文`是一项基本生存技能，不认识英文的话，你可能真的不适合你所从事的行业。

## 幼儿园的小朋友都知道要有礼貌

```
请问
  ...问题描述...
谢谢
```



## 学会描述问题

> 向别人提问的时候，要学会正确的描述问题。
> 把对方当成你的老板，你在给他做报告。要用最精炼的文字和图片，向对方阐述明白一个事情的来龙去脉。

> **要知道，你不是我追的妹子，我没有时间来猜你想要什么。**

> 记住，给别人的条件越多，你的问题解决越快。因为这不是解密游戏。

1. 请问一个关于 `什么` 的问题。
1. 我想要达到 `什么样` 效果，但是我这样做出现了 `什么样` 的问题。
1. 报错日志是 `这样` 的。（要 `学会` 画关键字）
1. 我尝试过 `什么` 方法来解决。
1. 我尝试搜索过了 `什么` 关键字，在里面找到了 `这些 URL` 的回答，尝试了还是没有解决问题。
1. 我用的是 `什么` 操作系统，版本号是多少。
1. 我用的是 `什么` 软件，版本号是多少。
1. 谢谢

> 千万别认为只有别人帮助你之后才需要说 `谢谢`。

### 学会什么时候贴图


像这种，IM 自动转义表情，贴出来的问题全是表情。

### 学会什么时候要圈出重点

千万不要认为别人的频率和你是同步的，然后像这样扔出一张图一个表情就了事了。

在工作中， 你`@`的人可能会多问一句什么情况。 但是在 IM 聊天群里面，就没有这么好运气了。



如下很难吗？

```
@xxx，我这边访问不了 git 仓库。
环境是: 环境是什么。
```


### 学会什么时候贴文字


## 什么是弱智一样的提问


## 萌新滚粗


| 什么鬼？    | 咋回事？  | 怎么办？    | 救命啊！！       |
|-------------|-------------|-------------|------------------|
| 自己 [bing](https://cn.bing.com) | 自己 [google](https://www.google.com) | 自己 baidu | 自己 [yandex](https://yandex.ee) 了吗 |

## YDOS V1.7 源码部分
```
@echo off
setlocal EnableDelayedExpansion

:: 初始化全局变量
set "title=Y-DOS V1.7.3"
set "version=Alpha-1007.2407.10"
set "date=2024/07/10"
set "token=a7a7"
set "licenseKey="
set "kmsServer=kms.03k.org"

:: 菜单选项定义
set "menuOptions=0123456ibdcbeadminfnmsa"
set "proMenuOptions=0123456ibdcbedecbadminfjknm"
set "cmdOptions=helpbacktokentoken"

:: 颜色定义
set "menuColor=06"
set "proColor=07"

:: 颜色字符串输出函数
:colstr
set "colorStr="
for /L %%i in (1,1,%1) do set "colorStr=!colorStr![%~2"
echo !colorStr%!%~3!
exit /b

:: 令牌验证
:token
cls
title [%title%] 【请输入访问密钥】
color f
call:colstr f 1 "请输入访问密钥" 0 1 0
echo.
call:colstr c 1 "TOKEN：%bb%" 0 1 0
set /p cc= %bb%
echo.
if "%cc%"=="%token%" goto :success
goto :31

:: 成功
:success
set "msg=1.YDOS部分源代码由\nChina DOS Union提供\n\n2.本软件为免费软件\n若您不慎下载了非正版\n请进入下列网站进行下载\n\nydos.ymxer.com"
mshta vbscript:msgbox(Replace("%msg%","\n",vbCrLf),6,"       YDOS 声明     ")(window.close)
color a
echo 密钥正确
echo 版本号:%title% 
echo %version%
choice /t 1 /d y /n >nul
goto :menu

:: 高级版密钥
color 9
echo 高级版密钥正确,感谢您对YDOS的支持
echo.
choice /t 2 /d y /n >nul
goto :menu2

:: 密钥错误
:31
color 4f
call:colstr fc 21 "密钥错误" 0 1 0
echo.
echo 点击任意键重试...&pause>nul
cls
goto token

:: 激活系统
:windows
cls
echo 正在激活
slmgr /ipk %licenseKey%
cls
echo 激活1/3
slmgr /skms %kmsServer%
cls
echo 激活2/3
slmgr /ato
cls
echo 激活成功
timeout /t 3
goto menu

:: 网络测试和缓存刷新
:itest
title %title% 请在运行完成前不要关闭 YDOS!!!
ping www.gov.cn
ping ymxer.com
ping gov.cn
ipconfig
ipconfig /release
cls
echo 请不要在此操作前关闭YDOS！！！
ipconfig /renew
netsh winsock reset
ipconfig /flushdns
set msg="缓存刷新完成\nYDOS WIN RESET"
mshta vbscript:msgbox(Replace("%msg%","\n",vbCrLf),6,"NETWORK RESET YDOS")(window.close)
start https://www.gov.cn/
cls
color a
echo 测试完成 以及 成功刷新缓存(可能需要重启)
echo 请看弹出浏览器页面是否成功加载
timeout /t 30
goto menu

:: 网络重置
:yin
cls
echo 请按回车再次确认
timeout /t 90
cls
echo 开始执行,请不要关闭
ipconfig
ipconfig/flushdns
netsh int ip reset
netsh winsock reset
netsh winhttp reset proxy
netsh wlan set tracing mode=no
timeout /t 1
cls
color a
echo 重置成功,请重启电脑解决
echo 是否为您重启电脑
set /p shutdown=  y是的  n不用了我自己有手:
if "%shutdown%"=="y" shutdown -r
if "%shutdown%"=="n" goto :menu
timeout /t 0
goto menu

:: 管理员菜单
:admin
title %title% 管理员菜单
cls
color 4
echo.
call:colstr c 1 "     YDOS 【管理员菜单】" 0 1 0
echo.
echo.
echo ║ [0] 版本号
echo ║ [1] 返回
echo ║ [2] 一键重启
echo ║ [3] 一键关机
echo ║ [4] 一键暂停系统(断电/休眠)
echo ║ [5] 取消重启/关机计划
echo ║ [a] 延迟关机
echo ║ [b] 查看您的IPV4
echo ║ [c] 查看您的IPV6
echo #以下为Starts选项
echo ║ [sa] 自启动项目
echo ║ [sb] Host文件夹
echo ║ [sc] hosts
echo.
set /p admin=  YDOS-ADMIN: 
if "%admin%"=="0" goto :bbh
if "%admin%"=="1" goto :menu
if "%admin%"=="2" shutdown -r -t 0
if "%admin%"=="3" shutdown -p
if "%admin%"=="4" shutdown -h
if "%admin%"=="5" shutdown -a
if "%admin%"=="a" goto :shutdown
if "%admin%"=="sa" Explorer/e,"C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp"
if "%admin%"=="sb" Explorer/e,"C:\windows\system32\drivers\etc"
if "%admin%"=="sc" start C:\windows\system32\drivers\etc\hosts
if "%admin%"=="b" ipconfig | findstr IPv4
if "%admin%"=="c" ipconfig | findstr IPv6
pause
goto admin

:: 版本信息
:bbh
cls
color 2
echo 版本号 %version%
pause
goto admin

:: 主菜单
:menu
cls
title [%title%] [万物基于YDOS] [%date%更新] [版本号 %version%] 主菜单
color %menuColor%
echo.   
call:colstr 3 1 "        YDOS启动菜单" 0 1 0 
echo.
call:colstr c 1 "      (输入选项并回车)" 0 1 0
echo.                            
echo.
for %%i in %menuOptions% do echo ║ [%%i] %%%i%%
echo.
echo.
set /p in=  YDOS:
if "%in%"=="0" goto :starta
if "%in%"=="2" goto :root
if "%in%"=="3" goto :windows
if "%in%"=="b" goto :a123
if "%in%"=="1" goto :stop
if "%in%"=="4" goto :itest
if "%in%"=="5" goto :zhuomiantubiao
if "%in%"=="i" goto :information
if "%in%"=="d" goto :download
if "%in%"=="c" goto :update
if "%in%"=="e" goto :cmd
if "%in%"=="admin" goto :admin
if "%in%"=="f" goto :menu
if "%in%"=="pro" goto :okp
goto :informationa

:: 高级版菜单
:menu2
cls
title [%title%] [YDOS Pro] [%date%更新] [版本号 %version%] 高级版主菜单
color %proColor%
echo.   
call:colstr 3 1 "     YDOS 高级版 启动菜单" 0 1 0 
echo.
call:colstr c 1 "      (输入选项并回车)" 0 1 0
echo.                            
echo.
for %%i in %proMenuOptions% do echo ║ [%%i] %%%i%%
echo.
echo.
set /p inp=  YDOS-Pro:
if "%inp%"=="0" goto :starta
if "%inp%"=="2" goto :root
if "%inp%"=="3" goto :windows
if "%inp%"=="b" goto :a123
if "%inp%"=="1" goto :stop
if "%inp%"=="4" goto :itest
if "%inp%"=="5" goto :zhuomiantubiao
if "%inp%"=="6" goto :hostfix
if "%inp%"=="i" goto :information
if "%inp%"=="d" goto :download
if "%inp%"=="c" goto :update
if "%inp%"=="e" goto :cmd
if "%inp%"=="admin" goto :admin
if "%inp%"=="f" goto :menu
if "%inp%"=="help" goto :cmd1
if "%inp%"=="back" goto :menu
if "%inp%"=="token" goto :token
if "%inp%"=="j" shutdown -r -t 0
if "%inp%"=="k" shutdown -s -t 0
if "%inp%"=="n" shutdown -a
if "%inp%"=="m" goto :shutdown
if "%inp%"=="sa" Explorer/e,"C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp"
if "%inp%"=="sb" Explorer/e,"C:\windows\system32\drivers\etc"
if "%inp%"=="sc" start C:\windows\system32\drivers\etc\hosts
if "%inp%"=="nor" goto:yesp
goto :informationb

:: 延迟关机
:shutdown
set /p shutdown=  多长时间后关机(秒): 
shutdown -r -t %shutdown%
cls
color a
echo 您已经设置 %shutdown%秒 后关机
pause
goto admin
endlocal
```
