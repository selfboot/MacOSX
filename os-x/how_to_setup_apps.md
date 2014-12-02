# Mac 软件安装
---

## Mac App Store

如果你有了Apple ID，那么可以直接在MAC App Store安装应用，整个过程非常简单，只需要点击安装即可（当然付费软件有支付过程）。然后，系统会帮你搞定一切，以后Store里有新版本的话会提示你更新，更新过程也是一键完成，十分简单。

用App Store的一个问题就是，上面的软件是根据你的Apple ID所在的国家或地区提供的，也就是说如果你的账号是美国区的，就无法下载更新中国区的软件，比如QQ，迅雷等。还有就是App Store上面的软件更新比较慢，例如Alfred 2.0已经出了很久，但在 Mac App Store 上还是1.2版本，QQ也是这样的情况。

此外并不是所有的软件都在App Store上架，因为苹果的审核过程十分严格繁琐，所以一些软件并没有上架，有自己专门的官网，这时候就需要去下载dmg安装包，然后手动安装。

## 镜像文件安装

使用镜像文件安装软件时，一般只需要把App的图标拖入到“应用程序”文件夹中即可，像下图一样：

![os_x_][1]

但是并不是所有软件都这样做，许多软件发明了独特的安装方式，让人凌乱不堪！比如Evernote Skitch解压缩之后就是一个App文件，没有然后了。而百度输入法竟然是下一步、下一步的安装方式，一下子穿越到Win上面了。

## Homebrew安装

什么是Homebrew？

> Homebrew is the easiest and most flexible way to install the UNIX tools Apple didn’t include with OS X.

我们能够通过终端方便的使用它安装管理苹果没有自带的UNIX相关工具。Homebrew 会将package安装到独立目录，并将文件软链接至 `/usr/local`。

**安装 Homebrew**

	ruby -e"$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

**如何使用 HomeBrew？**

使用非常简单，当我们在终端输入brew时，就能看到简单的使用提示，下面展示几个常用的使用场景。

1. 搜索、安装、更新、卸载 package

		brew update                 # 更新 formula
		brew search package_name    # 搜索 package
		brew install package_name   # 安装 package
		brew upgrade package_name   # 更新 package
		brew uninstall package_name # 卸载 package

2. 显示已安装package信息

		$ brew info wget
		wget: stable 1.15 (bottled), HEAD
		http://www.gnu.org/software/wget/
		/usr/local/Cellar/wget/1.15_1 (9 files, 908K) *
		...
		==> Dependencies
		Required: openssl✘
		==> Options
		...
 
3. 查看下载的package缓存的位置

		$ brew --cache
		/Library/Caches/Homebrew
		$ ls /Library/Caches/Homebrew
		Formula                                
		mongodb-2.6.0.tar.gz
		tree-1.7.0.mavericks.bottle.tar.gz
		ctags-5.8.tar.gz …… 

## Homebrew-cask安装

Homebrew使得Mac下可以方便快速安装wget等常用包，不过要安装qq，迅雷还得去官网下载或者使用中国区的账号在Mac App Store上面下载，相当繁琐。好在[@caskroom](https://github.com/caskroom)提供了[homebrew-cast](https://github.com/caskroom/homebrew-cask)，简化了软件的安装过程。

homebrew-cask是一套建立在homebrew基础上的Mac软件安装命令行工具，所以使用她之前需要先安装homebrew，此外还需要有安装Xcode。cast安装十分简单，一条命令：

	brew install caskroom/cask/brew-cask

之后就可以使用以下命令快速安装Chrome：

	$ brew cask install google-chrome
	=> Downloading https://dl.google.com/chrome/mac/stable/GGRO/googlechrome.dmg
	=> Success! google-chrome installed to /opt/homebrew-cask/Caskroom/google-chrome/stable-channel
	=> Linking Google Chrome.app to /Users/phinze/Applications/Google Chrome.app

可以看到cast将软件安装在 `/opt/homebrew-cask/Caskroom` 中，然后软链接到 `/Users/phinze/Applications/Google Chrome.app` ，这样就可以快速调用软件了。

**常用命令**

	brew cask search       # 列出所有可以被安装的软件
	brew cask search drop  # 查找所有和 drop 相关的应用
	brew cask info thunder # 查看thunder应用相关的信息
	brew cask uninstall qq # 卸载 qq

软件更新可以选择使用自带的更新功能，或者是：

	brew cask uninstall APP && brew cask install APP

来更新软件。有了Homebres-cask就可以一键装机了，如下：

	brew cask install alfred
	brew cask install qq
	brew cask install thunder
	brew cask install mplayerx
	brew cask install evernote
	brew cask install skitch
	brew cask install dropbox
	brew cask install google-chrome
	brew cask install mou
	brew cask install iterm2
	...

homebrew-cask自带相当多的软件资源，列表在[这里](https://github.com/caskroom/homebrew-cask/tree/master/Casks)，基本够用。不过你可以创建自己的cask，并分享出去，具体方法见[How To Contribute](https://github.com/caskroom/homebrew-cask/blob/master/CONTRIBUTING.md)。homebrew-cast只是帮你从官网下载安装软件，所以说不用担心软件的安全问题。

参考  
[Mac OS X，糟透了的软件安装体验](http://ksmx.me/broken-user-experience-of-installation-applications-on-mac-os-x/)  
[Mac安装软件新方法：Homebrew-cask](http://www.yangzhiping.com/tech/homebrew-cask.html)  
[简洁优雅的Mac OS X软件安装体验 - homebrew-cask](http://ksmx.me/homebrew-cask-cli-workflow-to-install-mac-applications/)  

[1]: http://xuelangzf-github.qiniudn.com/os_x_how_to_setup_app.png

---
<ul style="list-style:none; width:100px; margin:0 auto;">
<li style="float:left"><a href="http://zhaofei.tk/MacOSX"><img src="../resource/home.png" ></a></li>
<li style="float:left"><a href="https://github.com/xuelangZF/MacOSX/blob/gh-pages/os-x/os-x_summary.md"><img src="../resource/os-x.png" ></a></li>
<li style="float:left"><a href="https://github.com/xuelangZF/MacOSX/blob/gh-pages/apps/apps_summary.md"><img src="../resource/apps.png" ></a></li>
</ul> </div>