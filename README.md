# README

> 这个专案是用 [hexo](https://hexo.io) 搭建的，主要是写`贾胖`的个人心情抒发 blog，另外有一个`贾胖`的技术 blog 写在 [https://blog.jiapan.tw](https://blog.jiapan.tw)

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
