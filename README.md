<div align="center">
<h1>PikPak-Invitation</h1>
<p>PikPak自动邀请程序。</p>
<hr>
</div>

## 这是什么
这是一个使用Python编写的PikPak自动邀请程序，修改自[B站-纸鸢花的花语](https://paperkiteblog.xyz/)编写的[PikPak自动化邀请程序](https://paperkiteblog.xyz/index.php/archives/9/)。   
原理是PikPak的邀请领会员机制，通过邀请新人来领取5天会员，上限为50个人。

## 使用
你可以直接在[releases](https://github.com/rong6/PikPak-Invitation/releases)内下载已构建版本（仅支持Windows）。   

或者直接运行python文件，克隆源码：
``` bash
git clone https://github.com/rong6/PikPak-Invitation.git
```

前往mypikpak.com获取你的邀请码（纯数字），然后短效正式邮箱（即Outlook、Hotmail、QQ、@126、Gmail、@163、Yahoo...），需支持、启用Pop3协议，购买自行使用搜索引擎搜索`短效邮箱购买`，或查看原作者推荐的短效邮箱平台：[戳我](https://paperkiteblog.xyz/index.php/archives/9/#cl-6)。   

然后在`main.py`同目录下创建一个`mail.txt`文件，里面以`<mail@example.com>----<password>`格式一行一个放置邮箱及其密码。   

确保导入的库已全部安装，运行：
``` bash
python main.py
```

按提示输入即可，注意：
- 用过的邮箱将会自动在`mail.txt`内删除，在`mail_used.txt`放置，方便后续查找。
- 第一次输入邀请码将会储存在`invite_code.txt`内，下次无需输入。
- 当前代码没有添加代理池功能，运行时请注意手动更换IP。