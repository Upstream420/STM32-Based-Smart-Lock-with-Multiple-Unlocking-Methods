# 智能门禁网页维护说明

当前页面是纯静态工程，直接打开 `preview.html` 即可预览。

## 文件职责

- `preview.html`：页面结构入口，只保留主要区域和资源引用。
- `assets/css/styles.css`：页面样式、颜色变量、响应式布局。
- `assets/js/data.js`：页面展示数据配置，包括导航、指标卡、状态行、按钮、日志和设备列表。
- `assets/js/app.js`：渲染逻辑和按钮交互逻辑。

## 常见修改

- 修改页面文案或初始状态：编辑 `assets/js/data.js`。
- 增删设备模块：编辑 `devices` 数组。
- 增删开锁记录：编辑 `logs` 数组。
- 接入摄像头视频流：把 `camera.streamUrl` 改成摄像头地址，例如 `http://192.168.1.100:81/stream`。
- 调整颜色、间距、圆角：优先修改 `assets/css/styles.css` 顶部的 CSS 变量。
