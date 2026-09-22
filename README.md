# JJ-clash-config
iOS Clash (Hako) 的配置文件。

## 1. `JJ-config_full.yaml`，含机场的配置文件

### Step 1. 下载配置文件

**主链路（gh-proxy.org｜最快，≤60 秒更新）：**
```text
https://gh-proxy.org/https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config_full.yaml
```

**备链路（gh.idayer.com｜不同链路，实时）：**
```text
https://gh.idayer.com/https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config_full.yaml
```

<p align="left"><img width="180" alt="JJ-config_full.yaml 主链接二维码" src="./assets/qr/JJ-config_full-primary-mirrors.svg" /> <img width="180" alt="JJ-config_full.yaml 备用链接二维码" src="./assets/qr/JJ-config_full-backup-mirrors.svg" /></p>

**兜底链路（cdn.jsdelivr.net｜最稳，接受最长约 12 小时延迟）：**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/JJ-config_full.yaml
```

### Step 2.✈️ 添加机场订阅 
**找到以下代码，补充完整信息**
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
### Step 3.➕ 导入配置
**Clash首页-配置-添加配置-文件导入，选择上述修改后的`JJ-config_full.yaml`**
** **

## 2. `JJ-config.yaml`，不含`proxy-providers`机场订阅信息

### Step 1. Clash首页-配置-添加配置-链接导入，填写以下任一链接。

**主链路（gh-proxy.org｜最快，≤60 秒更新）：**
```text
https://gh-proxy.org/https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config.yaml
```

**备链路（gh.idayer.com｜不同链路，实时）：**
```text
https://gh.idayer.com/https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config.yaml
```

<p align="left"><img width="180" alt="JJ-config.yaml 主链接二维码" src="./assets/qr/JJ-config-primary-mirrors.svg" /> <img width="180" alt="JJ-config.yaml 备用链接二维码" src="./assets/qr/JJ-config-backup-mirrors.svg" /></p>

**兜底链路（cdn.jsdelivr.net｜最稳，接受最长约 12 小时延迟）：**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/JJ-config.yaml
```

### Step 2.✈️ 机场订阅与配置分离，机场订阅可通过 App首页-覆写-资源-代理来源 进行添加。
