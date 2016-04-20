### 项目简介 ###
由于众所周知的原因，在中国大陆想要访问部分国外网站需要通过某些特殊途径，其实修改hosts文件便能够访问部分被封的网站，此法应该可以满足大多数国人的需求。另外，hosts文件中的地址并非永久有效，随时都有可能被屏蔽，如遇相关情况请及时更新文件，也可暂时采取其他方式访问相关网站。
这里提供了最新可用的hosts文件列表，具体功能包括：
  * 优化 Google 访问 (可选北京服务器及美国服务器）
  * 可访问 Google+
  * 可访问 Facebook
  * 可访问 twitter (仅IPv6支持访问)
  * 可访问 YouTube (视频播放仅支持IPv6)
  * 可访问Wiki
  * 屏蔽 Adobe 激活服务器 (支持CC)
  * 屏蔽 Parallels Desktop 7 激活服务器
  * 屏蔽 Altium Designer 10 激活服务器
  * 加速 Google Drive 服务访问
  * 加速 Flickr 与 Dropbox 服务访问
  * 提供 Steam 服务器解析 (适用于非电信网络)

```
特别说明：替换hosts文件后，访问 facebook 和 twitter（仅IPv6）请使用https，即通过
Facebook：https://www.facebook.com/
Twitter：https://twitter.com/
分别进行访问，否则依旧无法访问；若想完美使用请在 facebook 和 twitter 中设置使用https安全访问。
Twitter 目前在 IPv4 环境下仅能通过后台API进行访问。
```

### Hosts Setup Utility v1.9.8-SE-beta.5（2014年3月5日发布） ###
```
2014年3月5日更新说明：
客户端更新 1.9.8 第二版 (Second Edition)：
    * 由于近期在大陆地区本工具各镜像站点的常规访问方式均遭到屏蔽，并且项目主页的域名遭到 DNS 污染，所以主要针对数据文件获取问题，发布此次紧急更新。
    * 采用加密链接获取 GoogleCode, Github 以及主站数据文件更新。
    * 更换 SourceForge 镜像服务器数据获取地址。

数据文件更新至 1.4.5 版本：
    * 提高诸如 Google, facebook 等站点在国内的访问效率。
    * 增加部分用于 Android 系统的 hosts 条目。
    * 增加本项目各镜像站点条目以应对 DNS 被污染带来的访问问题。

已知问题：
    * 当前我们不提供独立 hosts 文件下载，但是可以使用 Hosts Setup Utility (v1.9.7或更新版本)导出独立 hosts 文件以
    供移动设备使用。
    * 由于 py2app 的 locale 问题，Mac 下的应用可能无法正常识别系统语言环境，用户需要手动选择界面语言。
```
| **版本** | **文件名** | **下载链接** |
|:-------|:--------|:---------|
| Hosts Setup Utility for Windows(32位) | HostsTool-win-gpl-1.9.8-SE-x86.zip | [下载](https://huhamhire-hosts.googlecode.com/git-history/gh-pages/release/HostsTool-win-gpl-1.9.8-SE-x86.zip) |
| Hosts Setup Utility for Windows(64位) | HostsTool-win-gpl-1.9.8-SE-x64.zip | [下载](https://huhamhire-hosts.googlecode.com/git-history/gh-pages/release/HostsTool-win-gpl-1.9.8-SE-x64.zip) |
| Hosts Setup Utility Python 源码(用户) | HostsTool-x11-gpl-1.9.8-SE.tar.gz | [下载](https://huhamhire-hosts.googlecode.com/git-history/gh-pages/release/HostsTool-x11-gpl-1.9.8-SE.tar.gz) |
| Hosts Setup Utility Python 源码(开发) | HostsTool-source-gpl-1.9.8-SE.tar.gz | [下载](https://huhamhire-hosts.googlecode.com/git-history/gh-pages/release/HostsTool-source-gpl-1.9.8-SE.tar.gz) |
| Hosts Setup Utility for OS X | HostsTool-mac-gpl-1.9.8-SE.dmg | [下载](https://huhamhire-hosts.googlecode.com/git-history/gh-pages/release/HostsTool-mac-gpl-1.9.8-SE.dmg) |

如果您喜欢本项目，猛击介个按钮吧:-)

**下载说明：**
  1. 用户可根据自己所使用的系统平台选择下载相应的发行版本。
  1. 此程序由于修改了 hosts 文件，可能会导致360等软件的误报，希望各位予以忽视。
  1. 如果您的 Linux 属于 Ubuntu, OpenSUSE 这类原生提供 QT 环境支持的发行版，本程序源代码可在相关平台下直接运行；如果系统中缺少相关组件，则可能需要自行配置 Python 2.7 以及 PyQT4 的运行环境。例如在 Debian 中可以使用：` apt-get install python-qt4 ` 来安装 pyqt4 的相关文件。
  1. 开发版本的源码包与普通用户版本的源码包区别在于开发版本提供了相关工程项目文件以及资源文件。
  1. Windows 在安装了 Python 解释器以及 PyQT 组件后也可以直接运行 Python 程序代码。推荐使用 Python 2.7 + PyQT4 的运行环境。

> 更多关于 Python 内容请访问：http://www.python.org/
> 关于 PyQT 的内容请访问：http://www.riverbankcomputing.co.uk/software/pyqt/intro

**使用说明：**
> 由于修改系统 hosts 文件需要较高的系统文件读写权限，所以使用本工具时请务必提升操作权限以进行相关操作。
  * 使用 Windows Vista 及更新版本 Windows 的用户需以“管理员身份”运行 hoststool.exe。
  * Linux 用户需要使用 root 权限执行 hoststool.py。
  * Mac OS X 用户在启动应用时输入用户密码即可获得权限。
  * 使用字符界面模式时仅需在启动时使用 -t 参数，即` python hoststool.py -t `或者 Windows 下使用` hoststool_tui.exe -t `。
  * 新版本已经支持用户自定义 hosts 列表，只需在程序工作目录下建立 custom.hosts 文件，并向其中添加自己需要的内容，即可在生成 hosts 文件时使用这一部分条目。
> 更多详细说明请参阅开发文档（英语）: https://hosts.huhamhire.com/document/

### 相关截图 ###
  * Hosts Setup Utility:
> > ![http://wiki.huhamhire-hosts.googlecode.com/git/images/Win-GUI.png](http://wiki.huhamhire-hosts.googlecode.com/git/images/Win-GUI.png)

  * 字符界面:
> > ![http://wiki.huhamhire-hosts.googlecode.com/git/images/Linux-TUI.png](http://wiki.huhamhire-hosts.googlecode.com/git/images/Linux-TUI.png)

### 历史版本跟新说明： ###
  * 2014年3月5日更新说明：采用加密链接获取 GoogleCode, Github 以及主站数据文件更新。更换 SourceForge 镜像服务器数据获取地址。
  * 2014年1月24日更新说明：提供新的 Curses 界面模式以支持诸如 Linux 服务器等不具备图形界面的设备。提供新的自定义模块支持，允许用户定义独立模块"custom.hosts"，来向 hosts 文件中增加自定义内容。修正部分 Linux 发行版中 hosts 文件元数据修改权限问题。修正 OS X 10.9.x 下的部分兼容性问题。重新定义 Hosts Setup Utility 代码结构。提供开发文档（英语）支持 https://hosts.huhamhire.com/document/。
  * 2013年12月2日更新说明：采用全新设计的黑色界面主题，为各平台提供一致的用户体验。改进了 hosts 文件写权限判定机制，已符合最小权限原则。对功能选择菜单提供了进一步本地化说明。修复其他一些小问题。
  * 2013年8月5日更新说明：增加 hosts 文件导出功能。导出 hosts 文件时可选择 ANSI/UTF-8 编码方式以适应不同设备。hosts 列表修复 IPv4 环境下 Facebook 的访问问题。修复 raw.github.com 的访问问题。增加相关模块以支持 hosts 文件导出。
  * 2013年7月28日更新说明：使用 Python 与 QT 重新设计了新客户端程序 Hosts Setup Utility，兼容 Windows, Linux, Mac OS X 三大桌面平台。客户端程序开始提供有限的国际化语言支持。使用 SQLite 数据库存储新的 hosts 数据包，提供更高级的 hosts 功能选择。启用重新设计的数据包推送方案。针对 Google 服务器提供 北京/美国 服务器选择。增加 Altium Designer 10 激活服务器屏蔽功能。增加 Steam 美国服务器解析 (适用于非电信网络)。修复 Flickr 访问登录。修复 IMDB 图片显示。去除因苹果启用国内 CDN 服务器而不再需要的相关苹果服务条目。广告服务器屏蔽功能由默认转为可选安装。
  * 2013年2月1日更新说明：更新Facebook服务器，修复图片上传，在网络条件较好的情况下可使用在线聊天功能。推出Windows版HostsPanel在线更新工具第一个版本的测试版本（建议用户初次使用前阅读相关说明）。
  * 2012年11月18日版更新说明：Google IPv4站点的解析指向Google北京服务器的新地址，提高访问速度与可靠性。
  * 2012年11月10日版更新说明：修复部分Google IPv4服务器访问不稳定的问题，修复Facebook服务器地址变更造成的访问问题，修复IPv4网络对YouTube的页面访问问题，调整部分广告屏蔽。
  * 2012年10月28日版更新说明：为迎接十八大召开，使用Google美国服务器更换被屏蔽的Google中国服务器地址；修复之前版本造成的Skype可能无法正常工作的问题，解除对迅雷软件下载网站的不必要屏蔽，解除部分网址导航跳转内容的屏蔽，修复Ipv6无法访问射手字幕站点的问题。
  * 2012年10月13日版更新说明：修复因Facebook服务器地址变更造成的访问问题，修复通过后台API无法访问Twitter的问题，更新广告及恶意网站屏蔽，全面支持Windows 8 RTM。
  * 2012年8月1日版更新说明：增加Adobe CS6激活认证服务器屏蔽，增加Parallels Desktop 7激活认证服务器屏蔽。新增Huhamhrie-hosts主页指向。修复部分国内网站被拦截的bug。
  * 2012年5月28日版更新说明：修复5月Facebook地址失效问题。规范Localhost地址指向。
  * 2012年5月8日版更新说明：修复Mac下5月1日版之后可能出现的编码错误的问题。更新`PyHosts`，增加扩展功能，可使用控制台参数选择下载服务器。
  * 2012年5月6日版更新说明：修复5月6日被屏蔽的Google部分服务器，发布跨平台在线更新工具。
  * 2012年5月1日版更新说明：修复4月Facebook被封问题，增加Google Drive加速服务，优化广告过滤，修复无法可能导致无法登陆百度的Bug，全面升级Windows版的安装程序，规范化hosts文件编码。
  * 2012年3月2日版更新说明：更新IPv6版hosts（教育网用户等有需求用户可下载相应版本使用），更新部分Google服务器地址，支持Windows 8 Consumer Preview。
  * 2012年1月28日版更新说明：更新Google服务器地址，使用新的Google+国内服务器地址，解决之前版本Twitter地址被屏蔽的问题，更新Facebook服务器地址，加速Flickr与Dropbox服务。
  * 2011年10月4日版更新说明：修复九月中旬被屏蔽的Google+相关地址，新增加速苹果服务访问功能。
  * 2011年8月15日版更新说明：可玩Google+，完美使用包括最新游戏功能，Facebook和twitter正常https访问，`YouTube`可访问但无法播放部分视频。
  * 2011年8月9日版更新说明：添加Wiki，屏蔽Adobe激活服务器，增加恶意的网站和病毒网站的屏蔽。

### 项目主页 ###
  * Huhamhire hosts主页：http://hosts.huhamhire.com/


### 代码托管平台 ###
  * Google Code: http://code.google.com/p/huhamhire-hosts/
  * `SourceForge`: http://sourceforge.net/p/huhamhirehosts
  * `GitHub`: https://github.com/huhamhire/huhamhire-hosts

### 鸣谢 ###

> smarthosts, hostsx, ipv6-hosts, mwsl, yoyo, ATGFW, mvps and hpHosts

本程序最终解释权归“huhamhire-hosts Team”所有。
huhamhire-hosts Team©2011-2014