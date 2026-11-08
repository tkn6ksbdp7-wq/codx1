# 一间小站 · codx1

中文响应式静态网站，包含个人介绍、商品分类与搜索、可调整数量且在浏览器保存的购物袋、利润计算器。

## 预览

在本项目目录运行 `python3 -m http.server 8080 --directory dist`，打开 http://localhost:8080 。也可以直接在浏览器打开 dist/index.html。

## 自定义

- `dist/index.html`：个人介绍和页面内容。
- `dist/style.css`：配色与布局。
- `dist/app.js`：示例商品、购物袋、利润计算逻辑。

商品为演示数据，未接入支付、订单和真实库存。购物袋只保存在当前浏览器。利润计算未计入税费、推广费和退款；零收入时利润率显示为破折号。字体无法联网加载时自动使用系统字体。

发布到静态托管时将 dist 作为站点根目录。Sites 托管身份写在 .openai/hosting.json；它不包含密钥。
