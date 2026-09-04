# JJ-clash-config
iOS Clash (Hako) 的配置文件。

## 1. `config_full.yaml`，含机场的配置文件

### Step 1.🔗 下载配置文件

**Original link:**
```text
https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/config_full.yaml
```
**China acceleration 🚀:**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/config_full.yaml
```
```text
https://git.yylx.win/raw.githubusercontent.com/sydneygao/JJ-clash-config/main/config_full.yaml
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
**Clash首页-配置-添加配置-文件导入，选择上述修改后的`config_full.yaml`**
** **
## 2. `config.yaml`，不含`proxy-providers`机场订阅信息

### Step 1.🔗 Clash首页-配置-添加配置-链接导入，填写以下链接。

**Original link:**
```text
https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/config.yaml
```
**China acceleration 🚀:**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/config.yaml
```
```text
https://git.yylx.win/raw.githubusercontent.com/sydneygao/JJ-clash-config/main/config.yaml
```
### Step 2.✈️ 机场订阅与配置分离，机场订阅可通过 App首页-覆写-资源-代理来源 进行添加。
