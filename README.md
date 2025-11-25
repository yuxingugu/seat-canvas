# Seat Canvas - 高性能座位选择

基于 Canvas 的高性能座位选择组件，支持数千个座位的流畅渲染和交互。

## 特性

- ✅ Canvas 渲染，支持任意数量座位
- ✅ 流畅的拖动和双指缩放
- ✅ 座位点击选择
- ✅ 通过 URL 传递数据
- ✅ 响应式设计

## 使用方法

### 在微信小程序中使用

1. 在小程序后台配置业务域名：`yuxingugu.github.io`

2. 在代码中使用：

```javascript
// 将座位数据存储到 localStorage
uni.setStorageSync('__webview_seat_data__', JSON.stringify(templateData))

// 加载 WebView
this.webviewUrl = 'https://yuxingugu.github.io/seat-canvas/'
```

### 本地开发

```bash
# 启动本地服务器
python -m http.server 8080

# 访问
open http://localhost:8080
```

## 数据格式

座位数据需要包含以下字段：

```json
{
  "version": "2.0",
  "type": "canvas",
  "areas": [...],
  "areaSeats": {...},
  "priceInfo": {...}
}
```

## 部署

本项目使用 GitHub Pages 自动部署。

推送到 main 分支后，访问：
https://yuxingugu.github.io/seat-canvas/

## License

MIT
