# JJ-clash-config
iOS Clash (Hako) 的配置文件。

## 1. JJ-clash-config
**下载并找到以下代码，编辑替换订阅地址。**
```text
proxy-providers:
  Airport1:
    type: http
    url: 'https://example.com/your-profile.yaml' # 替换为机场订阅地址
    path: ./providers/Airport1.yaml
    interval: 43200
    filter: '^(?!(?:.*流量.*|.*时间.*|.*到期.*)).*$'
    health-check:
      enable: true
      url: 'https://www.gstatic.com/generate_204'
      interval: 600
      lazy: true
```
### 🔗 Full config download Links 

**Original link:**
```text
https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-clash-config.yaml
```
**China acceleration 🚀:**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/JJ-clash-config.yaml
```
```text
https://git.yylx.win/raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-clash-config.yaml
```

## 2. JJ-clash-config-only
**配置文件不含`proxy-providers`机场订阅信息，需搭配机场订阅使用。**
**机场订阅通过 App首页-覆写-资源-代理来源 进行添加。**
### 🔗 Config （no proxy-providers） download Links 
**Original link:**
```text
https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-clash-config-only.yaml
```
**China acceleration 🚀:**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/JJ-clash-config-only.yaml
```
```text
https://git.yylx.win/raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-clash-config-onnly.yaml
```

