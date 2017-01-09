# Alfred-New-Document
An Alfred workflow to create a new document in the current directory of Finder.

# 说明
源代码来源于锋友 kunkunkao 写的 AppleScript: 
http://bbs.feng.com/read-htm-tid-315552.html  
由于当前的版本下服务不显示在右键菜单了于是我将这个脚本进行了一些修改做成了 Alfred 的 Workflow。

# 使用方法
* 输入关键字 new 即可新建文件，默认文件名为无拓展名的 untitled
* 在 new 后面加空格可以继续输入文件名
* 如果出现重名文件会在文件名后加上下划线和递增的数字

# 已知问题和暂时解决办法：
* 只有全部 Finder 窗口关闭时才会在桌面新建文件，否则会在未关闭的最后打开的窗口目录下新建文件。例如在有 Finder 窗口打开时，无论切换到别的应用或是鼠标点击桌面后，都不会在桌面新建文件，而是在之前的窗口所在目录下新建。
* 目前的方案是使用关键字 dnew 强制在桌面新建文件。
