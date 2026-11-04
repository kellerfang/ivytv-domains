# ivytv-domains

IvyTV APK 的域名热更新清单。

APK 冷启动时按顺序尝试以下地址读取 `domains.json`：

1. `https://cdn.jsdelivr.net/gh/kellerfang/ivytv-domains@main/domains.json`
2. `https://raw.githubusercontent.com/kellerfang/ivytv-domains/main/domains.json`

读取成功后会缓存 6 小时；三条都读不到时退回 APK 内置的域名列表。

## 怎么用

- **换主域**：把新域名放到数组第一位，commit 即可
- **加备胎**：追加到数组末尾
- **彻底弃用某个域名**：从数组里删掉
- 只能写 `https://` 开头的裸域名，不要带路径

改完不用发版，用户下次打开 App 自动生效。
