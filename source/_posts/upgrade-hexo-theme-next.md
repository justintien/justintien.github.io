---
title: upgrade-hexo-theme-next
date: 2019-06-26 21:38:09
tags:
- 個人
- personal
---

# 心血來潮升級一下 next 主題

> 原先用的是 hexo-theme-next 6.x.y 忘了實際版號，目前升級至 [7.1.2](https://github.com/theme-next/hexo-theme-next/), 它的前身是 https://github.com/iissnan/hexo-theme-next (6.0.0 以下的版號)

## 主要原因

- 看到新的樣式有一些有趣
- 我在舊版本的作法上有一些不妥 (直接修改 themes/next/_config.yml 這會導致每次升級都要重新處理 conflict)
- 升級過程以及其遇到的小問題:

```sh
mv themes/next themex/next.old # 這個是個人習慣, 先備份舊的檔

# https://github.com/theme-next/hexo-theme-next/blob/master/docs/zh-CN/DATA-FILES.md
# 我採用了方法一 (改動最小)
# 选择 1：override: false（默认）：

# 检查默认 NexT 配置中的 override 选项，必须设置为 false。
# 在 next.yml 文件中，也要设置为 false，或者不定义此选项。
# 从站点的 _config.yml 与主题的 _config.yml 中复制你需要的选项到 hexo/source/_data/next.yml 中。
mkdir -p source/_data/

# 拉最新版本的 hexo-theme-next
git clone https://github.com/theme-next/hexo-theme-next/ themes/next

# 比對舊的 _config.yml 我有設定過的選項 (若你不是升級的不用做這一步)
git diff themes/next

# 想要覆蓋的 next _config.yml 都在這裡寫
vim source/_data/next.yml

# 以為一切都完成，結果發現 css 樣式沒有更新，才發現漏了這個流程
hexo clean && hexo g -d && hexo s

# hexo clean 清除緩存文件 db.json 和已生成的靜態静態文件 public
# hexo g = hexo generate 生成網站靜態文件到默認設置的 public
# hexo s = hexo server 啟動本地服務器，用於預覽主題，默認 http://localhost:4000/
```
