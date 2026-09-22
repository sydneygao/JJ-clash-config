# JJ-clash-config
iOS Clash (Hako) 的配置文件。

## 1. `JJ-config_full.yaml`，含机场的配置文件

### Step 1. 下载配置文件

**Original link 🔗:**

<img width="150" height="150" alt="JJ-clash-config-full-url-qr" src="https://github.com/user-attachments/assets/7971494d-1a41-4286-b44a-e26f787afbe5" />

```text
https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config_full.yaml
```
**China acceleration 🚀:**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/JJ-config_full.yaml
```
```text
https://git.yylx.win/raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config_full.yaml
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

### Step 1. Clash首页-配置-添加配置-链接导入，填写以下链接。

**Original link 🔗:**

<img width="150" height="150" alt="JJ-clash-config-url-qr" src="https://github.com/user-attachments/assets/5f927645-9c1f-4bb1-88a4-72d833b4fc2d" />

```text
https://raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config.yaml
```

**China acceleration 🚀:**
```text
https://cdn.jsdelivr.net/gh/sydneygao/JJ-clash-config@main/JJ-config.yaml
```
```text
https://git.yylx.win/raw.githubusercontent.com/sydneygao/JJ-clash-config/main/JJ-config.yaml
```
### Step 2.✈️ 机场订阅与配置分离，机场订阅可通过 App首页-覆写-资源-代理来源 进行添加。
