# ioh-talks-crawler
IOH 講座爬蟲

最近發現當兵前寫的 IOH 爬蟲GG，決定花些時間把它修好。

首先是第一頁，也就是 http://ioh.tw/talks/ 這一頁。

觀察噴錯的方向一開始以為是未安裝Nokogiri等等環境因素。

後來才發現是第一頁有隻講座缺少了 school 這項資料，而我寫的爬蟲並未做到相對應的判斷，難怪會噴錯 Orz。

原本以為問題僅此而已，沒想到 Bug 滿天飛， console 繼續噴。

搞了半天還是沒啥頭緒，於是決定再去觀察頁面。

爬到第 11 頁，乾，媽的，空白的 article 是怎樣啦 QQ ，難怪抓半天抓沒有。

於是在第2頁到最後一頁加入了簡單的判斷式，沒有 url 不存在的就 pass，如此遇到空白的講座就會跳過。

爬蟲還是挺好玩的啦，雖然除蟲的過程艱辛了點。
