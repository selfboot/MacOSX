# [1Password](https://agilebits.com/onepassword)

`付费`

摘要：

> 1Password 就是一款跨平台的，提供了一键自动填表登录浏览器扩展的帐号密码管理软件，所有的用户密码数据保存在本地，用户可以自主选择使用 Dropbox 进行网络同步。用户密码数据均以AES算法加密，安全性高，跨平台通用。缺点是收费且价格高。

你是不是在许多网站用同一个密码，或者是用123456、abc123作为你的密码？那么你的这些账户和没有密码毫无区别。但是谁也不能记住许多类似这样的密码：`(8hGMFyZo^JRJ6`。那么问题来了？该怎么管理那么多该死的密码呢？

所以，1password来了！正如它的名字一样，你只需要一个密码就可以对那些该死的复杂密码们说拜拜了。来张截图：

![1password密码][1]

1password是`跨平台`的(Windows，Mac，Android，iPhone，iPad)，可以随时随地帮你管理密码。

注册网站时，可以使用它来生成一个强大的随机密码，然后完全忘掉这个该死的密码吧。再次登录时，1password会帮你搞定一切。担心你的密码会被1password泄露？可能性肯定比从你自己这里泄露要少很多！

## 为什么要1password

如果不用1password，你得遵守以下的密码保护原则：

1. 避免在多个不同场合使用相同的一组密码。
2. 经常改换自己的密码。
3. 避免相同一组密码先后重复使用，避免新修改的密码使用之前用过的。
4. 避免使用一些可预测的词汇或数字号码，例如，重复的字，可查到的某个词的拼音缩写，身份证号，驾照号，某人生日，某个纪念日，亲朋或宠物的名字，个人偏好的事物等等。
5. 最好创建随机密码，降低人为猜中的几率。密码位数至少 12 位。(国内许多服务或网站支持最高16位，国外多数支持 32 位以上)
6. 密码中最好包括数字，符号和字母。如果支持大小写识别，最好大小写并用。

然而大部分人并没有这样做，爆出的密码库就说明了这一点。来看CSDN使用最多的10个密码吧：

次数  | 密码
---|---
235012 |123456789
212749 |12345678
76346 |11111111
46053 |dearbook
34952 |00000000
19986 |123123123
17790 |1234567890
15033 |88888888
6995 |111111111
5965 |147258369
5553 |987654321

要保证所有地方的密码都毫不重复并且牢记他们还不能混淆，再加上经常改换它们，而且还有诸多注意事项。果然是`密码虐我千百遍，我待密码如初见`啊。

所以选择1password吧。

## 使用

首先得为1password设计一个`超级强大`的主密码，还要经常更改，因为主密码是你进入1password的凭证。如果别人获得你的主密码，那么就可以登录你的1password，查看你保存的所有网站的密码，后果很严重。

当你需要使用一个密码的时候，只需要打开1password的密码生成器，然后设置生成密码的要求。可以设置密码长度，密码中字符和数字的个数，比如说设置一个长度为10的密码，包含3个数字，4个符号（剩下的全部是字母），那么就会生成类似以下的一些密码：

* Y]8L8;3;j>
* n9J^3;.2/d
* 3%6sF^$+A4

完全没有规律可言。

注册网站时，生成密码后，甚至不需要我们复制、粘贴密码到表单中，直接点1password中的填充，然后1password会自动填写密码、确认密码表单。之后，会将该网站的登录地址、用户名、密码保存在`登录信息`中。

登录网站时，如果登录信息中有保存该网站信息，那么会自动出现在密码生成器前面，只需要点击就会自动填写登录表单（有时候需要手动输入验证码）并跳转到登录后页面，如图：

![已保存网站登录][2]

从上图我们知道v2ex的登陆地址为 [http://v2ex.com/signin](http://v2ex.com/signin)，以及保存的该网站的用户名、密码等信息。 

如果登录网站时1password没有保存该网站信息，那么只需要输入一次密码，1password会自动保存，下次就可以自动登录。

## 1password安全问题

既然 1Password 掌握了几乎所有个人信息，若是它本身不安全，岂不是`祸起萧墙`！既然大家都在用，说明它还是很安全的，那么它是如何保证用户密码安全的呢？

* 1Passwowrd 采用 AES(advanced encryption standard )256 位加密用户的密码信息，这个加密标准本身的安全性是很高的。
* 用户的密码信息都由且只由一个主密码(Master Password)看管，除了设置这个主密码的人，任何人都无法开启，包括应用程序开发商。
* 1Password 保存的所有数据都在本地，它提供的网络云同步数据也是加密后之后才同步。
* 假如 iCloud 或者 Dropbox 有什么意外，这些用户数据也都是AES加密的，只能被主密码(Master Password)开启。


参考  
[CSDN 前 100 常用密码](http://www.guokr.com/post/81254/)  
[1Password真的安全吗？](http://iphone.91.com/tutorial/syjc/140422/21679992_all.html)


[1]: http://xuelangzf-github.qiniudn.com/2014-11-11_1password.png
[2]: http://xuelangzf-github.qiniudn.com/apps_onepassword_login.png

---
<ul style="list-style:none; width:100px; margin:0 auto;">
<li style="float:left"><a href="http://zhaofei.tk/MacOSX"><img src="../resource/home.png" ></a></li>
<li style="float:left"><a href="https://github.com/xuelangZF/MacOSX/blob/gh-pages/os-x/os-x_summary.md"><img src="../resource/os-x.png" ></a></li>
<li style="float:left"><a href="https://github.com/xuelangZF/MacOSX/blob/gh-pages/apps/apps_summary.md"><img src="../resource/apps.png" ></a></li>
</ul> </div>