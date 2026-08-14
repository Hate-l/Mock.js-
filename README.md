# Mock.js 学习演示项目

基于 [Mock.js](http://mockjs.com/) + [axios](https://axios-http.com/) 的前端数据模拟学习项目，通过 13 个由浅入深的 Demo 演示 Mock.js 的核心用法。

> 所有依赖通过 CDN 引入，**无需安装**，双击 `test.html` 即可运行。

## 目录结构

```
mock/
├── test.html       # 13 个 Demo 的完整演示页面
├── testmock.js     # 预留脚本文件
├── package.json    # 项目元信息（含本地服务器启动脚本）
├── .gitignore
└── README.md
```

## 运行方式

### 方式一：直接打开（最简单）

双击 `test.html`，在浏览器中即可使用。

### 方式二：启动本地服务器（推荐）

部分 Demo（如相对路径请求）在 `file://` 协议下可能受限，建议用本地服务器：

```bash
npm run serve
# 或
npx serve .
```

浏览器访问终端输出的地址（通常是 `http://localhost:3000`）。

## Demo 列表

| #  | 主题 | 说明 |
|----|------|------|
| 1  | Mock.mock() 基础 | 拦截 GET 请求并返回模拟数据 |
| 2  | 数据模板 7 种规则 | 固定数量、范围数量、布尔概率、整数/小数范围、自增步长、对象属性个数 |
| 3  | Mock.Random 工具类 | 随机姓名、邮箱、日期、城市、图片 URL 等 |
| 4  | 常用占位符大全 | 15+ 占位符：姓名、邮箱、网址、IP、省市区、手机号、GUID 等 |
| 5  | POST 拦截 + 请求体 | 模拟登录接口，根据请求体返回不同结果 |
| 6  | Mock.setup() 模拟延迟 | 设置 500~1000ms 响应延迟 |
| 7  | 正则生成数据 | 手机号、身份证、车牌号、十六进制颜色、QQ、微信号 |
| 8  | @image 图片占位 | 生成占位图片 URL 并预览 |
| 9  | 分页数据模拟 | 根据页码返回分页列表 |
| 10 | Random.extend 扩展 | 自定义省份、emoji、产品名生成器 |
| 11 | RESTful URL 拦截 | 正则匹配 `/api/book/:id`，支持 GET/PUT/DELETE |
| 12 | 文件上传模拟 | 拦截 multipart 上传请求，返回文件 URL 与元信息 |
| 13 | Mock.valid & toJSONSchema | 数据校验与模板转 JSON Schema |

## 技术栈

- Mock.js 1.1.0（CDN）
- axios（CDN）
- 原生 JavaScript

## License

MIT
