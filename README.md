# redis<br/>
# 安裝方法<br/>
### 到https://redis.io/download 找到stable的下載連結<br/>
### 複製<br/>
### 進入linux<br/>
### cd /usr/local/src<br/>
### wget 貼上剛剛複製的連結<br/>
### 解壓原碼並進入目錄<br/>
### tar zxvf redis-........<br/>
### cd redis-......<br/>
### make<br/>
### 等待編譯......<br/>
# 如果編譯中出現時間錯誤<br/>
### 解決方法: date -s 'yyy-mm-dd hh:mm:ss' 重寫時間<br/>
### 再使用: clock-w 寫入 cmos<br/>
# 編譯完後
### 使用 make test 來檢查一下<br/>
# 安裝並指定安裝路徑
### make PREFIX=/usr/local/redis install<br/>
### cd /usr/local/redis/ 進入目錄看一下<br/>
### ls 看到只有一個bin<br/>
### ls bin 可看到幾個文件<br/>
#各文件說明
### redis-benchmark<br/>
### redis-check-aof<br/>
### redis-cli <br/>
### redis-server <br/>
###<br/>
###<br/>
###<br/>
###<br/>
###<br/>
###<br/>
###<br/>
###<br/>
###<br/>

