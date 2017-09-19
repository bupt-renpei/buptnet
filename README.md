# 介绍

`buptnet` ，方便北邮校园网登录的 chrome 插件，基于 `Bootstrap3` 风格，采用 `jQuery` 和 `Highchart` 两个js库，主要功能有
* 多账号记录保存，多账号切换
* 打开浏览器，自动登录首选账号
* 剩余、使用流量占比可视化
* 动态校外流量速度曲线
* 账户网络、资费信息详情表格
> 注意：本插件未收集任何用户信息，用户账号和密码都是存于浏览器中的，可以查看 manifest.json文件的 permissions 配置进行确认

# 安装

1. 安装之前确保你电脑上存在 chrome 内核的浏览器，否则无法安装
2. 下载最新的release版本的插件打包文件，即 `crx` 文件
3. 下载完毕后，双击下载的crx文件即可安装，此时支持 chrome 内核的默认浏览器插件栏应该新增本插件
4. 或者打开 chrome 内核浏览器的插件管理页面 (chrome://extensions/)，将crx文件拖放到该页面即可进行安装
> 注意：版本较高的 chrome 浏览器会安装失败，这时候可以将 crx 文件当做压缩包解压，打开 `chrome` 的插件管理页面，勾选开发者模式，选择加载已解压的扩展程序，这时候选择已解压出来的文件夹即可

# 使用

* 点击插件图标会弹出界面，如果是登录界面则表明当前设备未登录校园网
* 如弹出主视图界面可以点击注销，跳转到登录界面进行账户的录入
* 填完账户和密码后直接点击登录不会记录账户密码
* 点击登录按钮内右侧的下拉箭头可以进行当前填写账号的管理，首选账号为默认填充账号、自动登录的账号，记录的账号在右侧的下拉列表进行切换
* 基本页面里的转标签也可以将插件页面转为普通浏览器标签页，方便实时信息的查看和其他操作
* 实时界面提供5秒段校外流量曲线图，仅供测试参考，请不要常开此页面，以减轻学校服务器压力
* 信息界面里提供一些关于设备和账号的信息，其中账号名可能不准
* 设置里面可以进行自动登录的设置，自动登录原理为，当设备接入校园网时，一般浏览器会自动弹出登录界面，插件监听到这个页面并进行登录状态的判断，如果未登录则根据首选账号进行自动登录
* 关于界面里面提供一些常用导航和作者信息
* 插件的图标提供不太准确的是否登录信息，绿色为已登录，灰色为未登录
