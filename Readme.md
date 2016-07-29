# 在WebView顶部加入平滑进度条(仿微信)
## 实现效果
![image](https://github.com/yangxu4536/WebViewTopPropress/blob/master/demo.gif)

## 微信效果
![image](https://github.com/yangxu4536/WebViewTopPropress/blob/master/wx_webview.png)

## 实现
- 重写WebChromeClient#onProgressChanged方法
- 当newProgress==100的时候,开启属性动画让水平进度条渐变消失
- 当newProgress<100的时候,开启属性动画让进度平滑递增