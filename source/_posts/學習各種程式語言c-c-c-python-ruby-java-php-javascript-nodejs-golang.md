---
title: '學習各種程式語言c,c++,c#,python,ruby,java,php,javascript/nodejs,golang'
categories:
  - 個人
tags:
  - 心得
date: 2020-01-11 10:38:05
---

# 學習各種程式語言c,c++,c#,java,python,ruby,php,javascript/nodejs,golang

最近把現下流行的語言都學了一遍，

其實會發現很多語言的優缺點，都會互相借鏡進步
(例如在 `javascript` ES7 中的 `async/await`，借鏡了 C#5.0、Python3.5中、Hack、Dart以及Kotlin 1.1的一個特性。
[wiki](https://zh.wikipedia.org/wiki/Await))

`c/c+` 用於寫底層效能高 (因為很多 API 是直接 call unix 底層功能實作)
我用 `c` 寫了一個 snake game: https://github.com/justintien/c-snake

有很多巨作都是用 `c` 完成的，例如 [linux](https://github.com/torvalds/linux)、[nginx](https://github.com/nginx/nginx)、[redis](https://github.com/antirez/redis)、[git](https://github.com/git/git)、[jq](https://github.com/stedolan/jq)、[netdata](https://github.com/netdata/netdata)

`c#` 寫遊戲就用它，跟 `unity` 完美的結合，IDE越來越強悍，語法上跟 `java` 還有點像

`java` 有朝一日沒想到我會用上它，工作所需短時間內把它學會，簡單的括說 `no spring no java or no JetBrains no java` 我感覺是 spring 全家桶救了 `java` 還有強大的 IDE 支援 (method reference 跳轉，自動補完自動import自動檢測一大堆強大的功能…讓 `java` 寫起來感覺輕鬆…OS: 你見過有人用 notepad 寫 java 的嗎? 我沒見過，但我以前真的是用 notepad 寫 `php` 的)

`python` 早期我是用來寫爬蟲的，它的一些解析器是非常好用的，現在非常多人用它做大數據分析

`ruby` 這個我也只拿來寫過爬蟲，據我觀察網上資料所知，這個語言漸漸淡出了…

`php` 我第一門學到的語言，網上最常聽見的就是世界上最美好的語言php，不用說語言簡單且不嚴格，亂寫寫不壞，加上有一些成熟的 CMS可以用，不過近年來版本更新的頻繁 (從 PHP 5.4...7.4)…其中 `laravel` 框架倒有點像是要往 `java` spring 全家桶的方向跑
曾經想要好好的把一些 module 建構起來寫了一個 `php+laravel` restful api 骨架: https://github.com/justintien/laravel-restful-api-skeleton (結果公司前面找的所有 phper 都離開了殘念)

`javascript` 自從 `nodejs` 的出現，它是唯一前後端可以共用同一種語言的語言(有點饒舌，但確實是這樣)

`golang` 簡單易學，寫區塊鏈、寫 web 都很容易

以下是用來練習 `java` `golang` `nodejs` repos:
https://github.com/justintien/blockchain-prototype
https://github.com/justintien/encrypt-decrypt
https://github.com/justintien/url-shortener

其實學這麼多語言，主要是概略知曉所有語言的特性以及優缺點，我想這對於之後我在寫主要語言的時候也會有所幫助吧，哈哈！

總之活到老學到老!!