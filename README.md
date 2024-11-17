# README

> 此專案使用 [hexo](https://hexo.io) 搭建，主要是寫 `賈胖` 的個人心情抒發日誌 blog，另外有一個 `賈胖` 的技術 blog [https://blog.jiapan.tw](https://blog.jiapan.tw)

## Dependencies

- hexo-theme-next 7.1.2: https://github.com/theme-next/hexo-theme-next/
  - 前身 (<= 6.0.0): https://github.com/iissnan/hexo-theme-next

## dev

```sh
# local server
# hexo server -p 4000
npm start

# new post
# hexo new <title>
npm run post -- <title>

# deploy to github
# hexo deploy -g
npm run public

# 升級 theme
cd themes/next
git pull
```
