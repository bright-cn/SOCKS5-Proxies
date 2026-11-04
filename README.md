# Bright Data SOCKS5 代理

[![推广](https://github.com/bright-cn/SOCKS5-Proxies/blob/main/first-deposit-banner.PNG)](https://www.bright.cn/solutions/socks5-proxies) 

## 概述
使用 Bright Data 的代理管理发送 SOCKS5 代理服务器请求，并借助专为多功能性、匿名性和卓越性能而设计的 Bright Data [SOCKS5 代理](https://brightdata.com/proxy-types/socks5-proxies)，享受流畅、高速的抓取体验。

- **支持 TCP 和 UDP 流量**
- **采用 SOCKS5 协议，实现最佳兼容性**
- **99.99% 的成功率**
- **免费地理位置定位（国家/地区、城市、州、邮政编码）**

## 主要功能
- **全球覆盖**：SOCKS5 代理覆盖 [195 个国家/地区](https://www.bright.cn/locations)。
- **高成功率**：抓取和数据采集成功率高达 99.99%。
- **快速响应**：连接可靠，延迟极低。
- **协议用途广泛**：适用于 HTTP、HTTPS、FTP 等协议。
- **无限扩展**：并发会话数量不受限制。

## SOCKS5 代理定价

### 住宅代理

- **按量付费**：$8/GB，无需按月承诺。
- **月度订阅**：
  - **71 GB**：$7/GB，每月 $499。
  - **166 GB**：$6/GB，每月 $999。
  - **399 GB**：$5/GB，每月 $1999。
  - **企业套餐**：为大规模运营提供定制定价和解决方案。

 ### ISP 代理

- **按量付费**：$1.8/IP，无需按月承诺。
- **月度订阅**：
  - **10 个 IP**：$1.8/IP，每月 $18。
  - **100 个 IP**：$1.45/IP，每月 $145。
  - **500 个 IP**：$1.4/IP，每月 $700。
  - **1,000 个 IP**：$1.3/IP，每月 $1,300。
  - **企业套餐**：为需要 1,000 个以上 IP 的运营提供定制定价和解决方案。
 
### 数据中心代理

- **按量付费**：$1.40/IP，无需按月承诺。
- **月度订阅**：
  - **10 个 IP**：$1.40/IP，每月 $14。
  - **100 个 IP**：$1.00/IP，每月 $100。
  - **500 个 IP**：$0.95/IP，每月 $475。
  - **1,000 个 IP**：$0.90/IP，每月 $900。
  - **企业套餐**：为需要 1,000 个以上 IP 的运营提供定制定价和解决方案。

注册后首次充值可获得等额赠金，最高 $500！

## SOCKS5 代理入门
1. **开始免费试用**：无需信用卡。
2. **集成**：使用 Bright Data 代理管理或 API 管理 SOCKS5 代理。
3. **支持的平台**：可在 Python、Node.js、cURL 等平台中轻松配置 SOCKS5 代理。

## 代码示例

### Python

```python
import requests

proxy = {
    "http": "socks5h://[your username]:[your password]@brd.superproxy.io:22228",
    "https": "socks5h://[your username]:[your password]@brd.superproxy.io:22228"
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
     "https://geo.brdtest.com/mygeo.json"
```

## 使用场景
探索 SOCKS5 代理在各行业中的广泛用途：

- [**电子商务**](https://www.bright.cn/use-cases/ecommerce)：追踪多个地区的产品价格、评论和库存情况。
- [**社交媒体**](https://www.bright.cn/use-cases/social-media-for-marketing)：匿名监控趋势、互动情况和竞争对手活动。
- [**旅游**](https://www.bright.cn/use-cases/travel)：通过精准的地理位置定位，比较不同国家和地区的旅游优惠。
- [**金融服务**](https://www.bright.cn/use-cases/financial)：安全采集实时市场数据并分析趋势。

---

## 常见问题

### 什么是 SOCKS5 代理协议？
SOCKS5 是一种用途广泛的代理协议，可通过代理在客户端与服务器之间路由网络数据包。它同时支持 TCP 和 UDP 连接，适用于网页爬虫、绕过限制和增强匿名性等多种应用。

### SOCKS5 与 HTTP 代理有何不同？
SOCKS5 的运行层级低于 HTTP 代理，因此可以处理更广泛的流量类型，包括 HTTP、HTTPS、FTP 和 SMTP。它不会修改网络数据包，因此还能提供更高的匿名性。

### 如何将 SOCKS5 代理与 Bright Data 服务搭配使用？
Bright Data 的住宅代理、数据中心代理和 ISP 代理网络均支持 SOCKS5。要使用 SOCKS5：
1. 将你的应用程序配置为通过端口 `22228` 使用 `brd.superproxy.io`。
2. 使用你的 Bright Data 凭据进行身份验证。
3. 确保通过 `socks5h://` 协议进行远程 DNS 解析。

### SOCKS5 代理的默认端口是什么？
Bright Data 的默认 SOCKS5 代理端口为 `22228`。请注意，HTTP (`22225`) 和 HTTPS (`22226`) 的标准端口不适用于 SOCKS5 连接。

### 使用 SOCKS5 代理有哪些优势？
SOCKS5 代理具备以下优势：
- **高度匿名**：隐藏你的 IP，确保连接安全且私密。
- **用途广泛**：可处理多种流量类型，包括 HTTP、HTTPS、FTP 等。
- **绕过限制**：突破地理封锁、防火墙和审查限制。
- **支持 TCP 和 UDP**：适用于各种使用场景。
- **性能可靠**：凭借 Bright Data 强大的基础设施，实现高可用性和低延迟。

### 如何确保 SOCKS5 代理达到最佳性能？
要优化性能：
1. 使用域名而非 IP 作为目标。
2. 通过 `socks5h://` 协议配置远程 DNS 解析。
3. 使用 [Bright Data 的代理管理](https://www.bright.cn/products/proxy-manager)，获取 IP 轮换和请求优化等高级功能。

### 可以使用 SOCKS5 代理进行地理位置定位吗？
可以，Bright Data 的 SOCKS5 代理支持精准的地理位置定位。你可以修改用户名来定位特定国家/地区、城市、州、邮政编码和 ASN（例如，使用 `username-country-us` 定位美国）。

### SOCKS5 代理是否符合 Bright Data 的政策？
是的，Bright Data 的 SOCKS5 代理遵守 GDPR 和 CCPA 法规，确保合规且合乎道德地使用数据。请遵循所有相关准则，以保持合规。

### 使用 SOCKS5 代理有哪些限制？
- **IP 限制**：仅支持域名；直接向 IP 发出的请求会被阻止。
- **端口限制**：SOCKS5 连接必须使用端口 `22228`。
- **远程 DNS 解析**：为确保合规，必须使用 `socks5h://` 协议。
- **目标端口**：仅支持高于 `1024` 的端口。
