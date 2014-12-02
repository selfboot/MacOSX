# [iTerm2](http://iterm2.com/)

`免费`

作为命令行工具，强大的快捷键支持才是最基本的要素，iTerm2在这一点上做的非常好。下面看一下他的快捷键支持吧！

**功能快捷键**

* ⌘ + 数字: 切换标签页，⌘ + 方向键 按方向切换标签页
* ⌘ + enter: 切换全屏
* ⌘ + f: 查找功能，支持正则，其中查找的内容会被自动复制，省去了再去⌘+c的步骤。键入搜索关键词，然后用shift-tab或者tab左右自动补全。
* ⌘ + d: 垂直分屏，⌘ + shift + d: 水平分屏。使用⌘ + ]和⌘ + [在最近使用的分屏直接切换，而⌘ + opt + 方向键切换到指定位置的分屏。
* ⌘ + t : 新的标签页
* ⌘ + w : 关闭当前标签页
* `⌘ + ；`: 自动补全历史命令
* `⌘ + shift + h`: 剪贴板历史
* ⌘ + r: 清屏，其实是滚到新的一屏，并没有清空。
* ⌘ + u: 启用、禁用背景透明度。

**输入快捷键**

* ctrl + u: 清空当前行，mac默认的Ctrl+u为清除当前光标至行首的内容，在iTerm2中则直接清除本行。
* `ctrl + k`: 当前位置删除到文本末尾
* ctrl + a: 到行首
* ctrl + e: 行末
* ctrl + f/b: 前进后退，相当于左右方向键，但是显然比移开手按方向键更快；
* ctrl + p: 上一条命令，相当于方向键上
* ctrl + r: 搜索命令历史
* ctrl + d: 删除当前字符；ctrl + h: 删除之前的字符；
* `ctrl + t`: 交换光标处和光标前面位置的字符；
* `ctrl + w`: 删除光标前面的单词；
* **_alt + d_**: 删除光标后面的单词；
* **_alt + f/b_**: 向前/后移动一个单词；

为了能像在bash中一样使用alt进行文本编辑，比如`alt + d/f/b`等，必须进行下面配置：

![配置示意][2]


iTerm2还有很多特色功能，招人喜爱：

* `选中即复制`；
* 窗口分割；
* 屏幕快照：
	* ⌘ + shift + s: 保存当前窗口快照；
	* ⌘ + opt + b: 快照回放，可以对所有操作根据时间轴进行回放。
* 系统热键：设置好系统热键之后，将在正常的浏览器或者编辑器等窗口的上面，以半透明窗口形式直接调出iterm2 shell。按下同样的系统热键之后，将自动隐藏。

屏幕快照有时候会特别有用，不过我最喜欢的还是系统热键带来的方便啦，展示一下系统热键的效果吧：

![iTerm2系统热键][1]

系统热键需要稍微配置一下，在Keys-Hotkey里可以设置系统热键的快捷方式。

iTerm2的配置文件在

	~/Library/Preferences/com.googlecode.iterm2.plist

可以备份自己的配置文件。此外，还可以在以下两个地方创建任意的按键组合来完成任意操作:

* Preferences > Keys 设置全局的快捷键, 会影响所有配置文件；
* Preferences > Profiles > Keys 设置单个配置文件中的快捷键。

还有一些隐藏的配置可以在[Hidden Settings](http://iterm2.com/documentation-hidden-settings.html)找到。

参考：    
[iTerm2新手应知特色功能  ](http://www.yangzhiping.com/tech/iterm2.html)  
[我在用的mac软件(1)--终端环境之iTerm2](http://www.cnblogs.com/noTice520/p/3190529.html)  
[Shortcuts to Move Faster in Bash Command Line](http://teohm.com/blog/2012/01/04/shortcuts-to-move-faster-in-bash-command-line/)    



[1]: http://xuelangzf-github.qiniudn.com/2014-11-11_iTerm2.png
[2]: http://xuelangzf-github.qiniudn.com/apps_iterm2_bash_etc.png

---
<ul style="list-style:none; width:100px; margin:0 auto;">
<li style="float:left"><a href="http://zhaofei.tk/MacOSX"><img src="../resource/home.png" ></a></li>
<li style="float:left"><a href="https://github.com/xuelangZF/MacOSX/blob/gh-pages/os-x/os-x_summary.md"><img src="../resource/os-x.png" ></a></li>
<li style="float:left"><a href="https://github.com/xuelangZF/MacOSX/blob/gh-pages/apps/apps_summary.md"><img src="../resource/apps.png" ></a></li>
</ul> </div>