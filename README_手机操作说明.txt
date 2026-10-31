华为手机 ChatGPT 网页封装 APK 项目
================================

重要说明
--------
这是一个第三方 WebView 封装应用，打开的是 https://chatgpt.com/。
它不是 OpenAI 官方发布的 APK，也不包含 ChatGPT 模型或账号系统。
登录与聊天由 ChatGPT 官方网站处理。请只在 https://chatgpt.com/ 登录。

手机端生成 APK（不需要电脑）
----------------------------
1. 用手机浏览器打开 https://github.com/ 并登录你的 GitHub 账户。
2. 创建一个 Public 仓库，仓库名可用 Qtx。
3. 进入仓库，选择 Add file -> Upload files。
4. 解压本 ZIP，把里面所有文件和文件夹上传到仓库根目录（注意 .github 文件夹也要上传）。
5. 点击 Commit changes。
6. 打开仓库顶部的 Actions。
7. 如果出现提示，点击 I understand my workflows, go ahead and enable them。
8. 选择 Build ChatGPT APK，再点 Run workflow -> Run workflow。
9. 等待运行结束，进入成功的运行记录页面，在 Artifacts 下载 ChatGPT-Huawei-debug-APK。
10. 解压下载的 artifact，里面的 app-debug.apk 就是安装包。

安装
----
在华为手机文件管理器中找到 app-debug.apk，点开安装。
若系统提示禁止安装，请只对当前使用的浏览器或文件管理器允许“安装未知应用”，安装后可关闭该权限。

注意事项
--------
- 手机必须能访问 GitHub 和 chatgpt.com。
- 需要华为系统内置 Android System WebView 正常可用。
- 某些 OpenAI 登录流程可能不允许在内嵌 WebView 中完成；若登录失败，不要反复输入密码或尝试非官方登录页，改用系统浏览器访问 https://chatgpt.com/。
- 这是未签名发布版的 debug APK；不要把 APK 分享给陌生人。GitHub Actions 的构建产物默认仅保留 7 天。
- 这个项目不会绕过地区、网络或账号限制。
