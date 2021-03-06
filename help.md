## 软件功能
本软件主要功能为使用鼠标框选屏幕上的内容，并进行OCR识别或进行翻译，可以选择将截图/识别内容/翻译结果自动复制到剪贴板
### 截图
* 使用鼠标框选即可截图
* 用户可以在设置中勾选组合键，只有当按下的键与设置相符时才会触发截图
### OCR识别
* 软件调用的是百度的通用OCR识别接口，需要连接网络
* 接口每日上限50000次，软件已经设置了默认的api_key和secret_key，用户可以自行在百度申请并填入设置界面中
* 识别的图片最短边不能小于15像素，最长边不能大于4096像素，若需要识别文字请注意框选范围
### 翻译
* 软件将先进行OCR识别，再调用百度的翻译接口进行翻译
* 用户可以在设置界面选择翻译的源语言和目标语言
### 悬浮窗模式
* 非悬浮窗模式下，点击关闭窗口软件即会退出，若最小化窗口则自动隐藏到托盘中，点击托盘图标可以恢复
* 悬浮窗模式下，主窗口将会一直悬浮在桌面顶层，此时关闭窗口软件不会退出，点击托盘图标可以再次弹出
* 用户可以在设置中调整悬浮窗的透明度
### 其他设置项
* `自动复制结果`：若勾选则会将截图/OCR结果/翻译结果自动复制到剪贴板
* `拦截鼠标事件`：若勾选，则在框选时阻拦鼠标事件传递到下方的应用中产生误触，只在组合键被正确按下时才会拦截
  > 注意：若不设置组合键并勾选拦截，鼠标右键将会失效
  
## 问题处理
* 若发现**软件无法响应框选操作**，请尝试重启软件
* 若发现**悬浮窗模式下看不到悬浮窗**，请检查设置中的浮窗不透明度
* 若有其他问题，请删除软件目录下的`conf.ini`文件（重置软件）并重新打开软件，若仍然发生，希望您可以[向我们反馈](https://support.qq.com/product/172973)

