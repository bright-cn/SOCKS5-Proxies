# Bright Data SOCKS5 代理

[![促销](https://github.com/bright-cn/SOCKS5-Proxies/blob/main/first-deposit-banner.PNG)](https://www.bright.cn/solutions/socks5-proxies)

## 概述
使用 Bright Data 的 Proxy Manager 发送 SOCKS5 代理服务器请求，凭借 Bright Data 的[SOCKS5 代理](https://www.bright.cn/proxy-types/socks5-proxies)享受无缝、极速的抓取体验。该产品兼具多功能、强匿名与卓越性能。

- 支持 TCP 与 UDP 流量
- 采用 SOCKS5 协议，兼容性强
- 99.99% 成功率
- 免费地理定向（国家、城市、州/省、邮编）

## 关键特性
- 全球覆盖：在[195 个国家/地区](https://www.bright.cn/locations)提供 SOCKS5 代理。
- 高成功率：抓取与数据采集成功率可达 99.99%。
- 响应迅速：连接可靠，延迟低。
- 协议通用性强：适用于 HTTP、HTTPS、FTP 等多种协议。
- 无限扩展：并发会话数量不受限制。

## SOCKS5 代理定价

### 住宅代理（Residential Proxies）

- 按量付费：$8.4/GB，无需月度承诺。
- 月度订阅：
- 69 GB：$7.14/GB，$499/月
- 158 GB：$6.3/GB，$999/月
- 339 GB：$5.88/GB，$1999/月
- 企业方案：为大规模业务提供定制价格与专属解决方案

### ISP 代理

- 按量付费：$1.8/IP，无需月度承诺。
- 月度订阅：
- 10 IP：$1.8/IP，$18/月
- 100 IP：$1.45/IP，$145/月
- 500 IP：$1.4/IP，$700/月
- 1,000 IP：$1.3/IP，$1,300/月
- 企业方案：超过 1,000 IP 的业务可提供定制价格与方案

### 数据中心代理（Datacenter Proxies）

- 按量付费：$1.40/IP，无需月度承诺。
- 月度订阅：
- 10 IP：$1.40/IP，$14/月
- 100 IP：$1.00/IP，$100/月
- 500 IP：$0.95/IP，$475/月
- 1,000 IP：$0.90/IP，$900/月
- 企业方案：超过 1,000 IP 的业务可提供定制价格与方案

注册并在首次充值获得等额赠送，最高 $500！

## SOCKS5 代理快速开始
1. 开始免费试用：无需信用卡。
2. 集成：使用 Bright Data Proxy Manager 或 API 管理 SOCKS5 代理。
3. 支持平台：可在 Python、Node.js、cURL 等中轻松配置 SOCKS5 代理。

## 代码示例

### Python

```python
import requests

proxy = {
http: "socks5h://[your username]:[your password]@brd.superproxy.io:22228",
https: "socks5h://[your username]:[your password]@brd.superproxy.io:22228"
}

response = requests.get("https://geo.brdtest.com/mygeo.json", proxies=proxy)
print(response.json())
```

### Node.js

```node.js
const request = require("request-promise");

const options = {
url: "https://geo.brdtest.com/mygeo.json",
proxy: "socks5h://[your username]:[your password]@brd.superproxy.io:22228",
};

request(options)
.then(function (response) {
console.log(response);
})
.catch(function (err) {
console.error(err);
});
```

### cURL

```shell
curl -x socks5h://brd.superproxy.io:22228 \
--proxy-user [your username]:[your password] \
https://geo.brdtest.com/mygeo.json
```

## 使用场景
探索 SOCKS5 代理在各行业的多样化用途：

- [电商](https://www.bright.cn/use-cases/ecommerce)：跟踪跨区域的商品价格、评价与库存。
- [社交媒体](https://www.bright.cn/use-cases/social-media-for-marketing)：匿名监测趋势、互动与竞品动态。
- [旅游](https://www.bright.cn/use-cases/travel)：通过精准地理定向对比各国及各地区的旅行优惠。
- [金融服务](https://www.bright.cn/use-cases/financial)：安全采集实时市场数据并进行趋势分析。

---

## 常见问题

### 什么是 SOCKS5 代理协议？
SOCKS5 是一种通用的代理协议，可通过代理在客户端与服务器之间转发网络数据包。它同时支持 TCP 与 UDP 连接，适用于网页抓取、绕过限制与增强匿名性等多种应用场景。

### SOCKS5 与 HTTP 代理有何不同？
SOCKS5 相比 HTTP 代理在更低的网络层工作，可处理更广泛的流量类型，包括 HTTP、HTTPS、FTP、SMTP 等。同时，SOCKS5 不会修改网络数据包，匿名性更高。

### 如何在 Bright Data 服务中使用 SOCKS5 代理？
Bright Data 在住宅、数据中心与 ISP 代理网络中均支持 SOCKS5。使用步骤：
1. 将应用配置为使用 brd.superproxy.io，端口 22228。
2. 使用你的 Bright Data 凭证进行身份验证。
3. 采用 socks5h:// 协议，确保远程 DNS 解析。

### SOCKS5 代理的默认端口是什么？
Bright Data 的 SOCKS5 代理默认端口为 22228。注意，HTTP（22225）与 HTTPS（22226）的标准端口不适用于 SOCKS5 连接。

### 使用 SOCKS5 代理有哪些优势？
- 高匿名性：隐藏你的 IP，连接更安全私密。
- 多功能性：可处理 HTTP、HTTPS、FTP 等多种流量类型。
- 绕过限制：跨越地域封锁、防火墙与审查。
- 支持 TCP 与 UDP：覆盖更广泛的用例。
- 稳定高效：依托 Bright Data 的强大基础设施，具备高可用与低延迟。

### 如何确保 SOCKS5 代理达到最佳性能？
- 使用域名作为目标而非 IP。
- 使用 socks5h:// 协议以启用远程 DNS 解析。
- 使用 [Bright Data 的 Proxy Manager](https://www.bright.cn/products/proxy-manager) 获取 IP 轮换与请求优化等高级功能。

### SOCKS5 代理是否支持地理定向？
支持。Bright Data 的 SOCKS5 代理可进行精确的地理定向。你可以通过修改用户名来指定国家、城市、州/省、邮编与 ASN（如：username-country-us 代表美国）。

### SOCKS5 代理是否符合 Bright Data 的合规政策？
是的。Bright Data 的 SOCKS5 代理遵循 GDPR 与 CCPA 规范，确保合规与道德使用数据。请按照相关指南操作以保持合规。

### 使用 SOCKS5 代理有哪些限制？
- IP 限制：仅支持以域名为目标；直接访问目标 IP 会被阻止。
- 端口限制：SOCKS5 连接必须使用 22228 端口。
- 远程 DNS：需要使用 socks5h:// 协议以实现合规的远程 DNS 解析。
- 目标端口：仅支持大于 1024 的端口。
