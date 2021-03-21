# smsJumpToMicroAPP

> 本项目同时发布到【[码云](https://gitee.com/zhaoquan/sms-jump-to-microapp)】和【[GitHub](https://github.com/chatterzhao/smsJumptoMicroAPP)】，但是主要维护码云，GitHub 上只保证 develop 分支与码云的 develop 分支同步

## 介绍

本项目是实现从短信、邮件等信息内容中的链接打开小程序

以下示例主要是从短信内容通过 H5 网页中转打开微信小程序，用 H5 中转是因为安卓手机不能正确的识别 Url Scheme。

体验网址：[https://zhaoquan.gitee.io/sms-jump-to-microapp/](https://zhaoquan.gitee.io/sms-jump-to-microapp/)，网址短化后：[https://dwz.cn/pF85DVgh](https://dwz.cn/pF85DVgh) (这里用的是百度的 dwz.cn，每月 100 次免费跳转，如果跳转不正常，请自己复制原网址到其它平台短化之后测试使用。请在非微信环境测试，如手机自带的浏览器中。注意：在微信聊天信息是无法打开的，百度手机 APP 也不可以正常打开)

## 本项目特点

- 只使用一个代码文件：index.html
- 只用修改 let scheme="XXXX"（有两个地方）即可使用
- 使用[码云](https://www.gitee.com)平台的 Gitee Pages 免费快速即可发布测试网站
- 使用一个网址短化平台将网址短化就可以比较方便的在群发短信中使用这个网址

## 项目使用

- clone（克隆）或下载或复制代码到本地

clone 的话在命令行执行命令： `git clone https://gitee.com/zhaoquan/sms-jump-to-microapp`

本项目有 3 个分支，master 是稳定的分支，develop 是开发分支，show 是 master 发布到网站的分支。你想要哪个分支，就在命令行，执行命令： `git checkout 分支名`，或者直接在网站上点击分支名进行切换。

- 在你想使用的分支替换 index.html 页面中两个位置的 let scheme = ""

scheme 可以登录自己的小程序后台：[mp.weixin.qq.com](mp.weixin.qq.com)，点击右上角的工具-生成 Url Scheme 获得。另外也可以通过接口获得。

- 将 index.html 上传到网站服务器，推荐码云的 pages

在码云打开本项目页面，点页面右上角的【服务】，点下面的 Gitee Pages， 我这里是发布 show 分支，部署分支选择 show，勾选强制使用 HTTPS，点发布或更新，过一会儿，点击 Gitee 分配的域名即可访问。

- 网址短化

短信按字数分条数收费，网址字数比较多，复制上一步的网址，使用短网址平台把网址短化一下，可以使用百度[https://dwz.cn/](https://dwz.cn/)(需要企业认证后才可以使用，收费：每月 100 点免费，免费额度每月最多可创建 5 个长期短链接，创建 1 年有效消耗 1 点，长期有效消耗 2 点，每跳转一次消耗 1 个点，购买基础套餐 10 元 10000 点左右)，或[https://4m.cn/](https://4m.cn/)进行短化，然后在短信里使用即可
