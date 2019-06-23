# redis<br/>
# 安裝方法<br/>
### 到https://redis.io/download 找到stable的下載連結<br/>
### 複製<br/>
### 進入linux<br/>
### cd /usr/local/src<br/>
### wget 貼上剛剛複製的連結<br/>
### 解壓原碼並進入目錄<br/>
### tar zxvf redis-{版本號}<br/>
### cd redis-{版本號}<br/>
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
# 各文件說明
### redis-benchmark: 性能測試工具<br/>
### redis-check-aof: 檢查aof日誌的工具<br/>
### redis-check-rdb: 檢查rdb日誌的工具<br/>
### redis-cli: 連接用的客戶端 <br/>
### redis-server: 服務進程 <br/>
# 複製配置文件
### cp /usr/local/src/redis-{版本號}/redis.conf ./ 從原文件中複製一份到當前目錄<br/>
# 啟動與連接
## 啟動<br/>
### 例如: [root@localhost redis]# ./bin/redis-server ./redis.conf <br/>
### 請勿用control c 退出 因為會關掉<br/>
### 再開一個連接進去<br/>
### 或是用守護進程啟動:<br/>
### vim redis.conf<br/>
### 找到daemonize no<br/>
### 改為: daemonize yes<br/>
### 再次啟動試試 ./bin/redis-server ./redis.conf<br/>
### 此時沒東西出現 <br/>
### 輸入 ps aux|grep redis <br/>
### 可以看到在後台運行了<br/>
## 連接<br/>
### 例如: [root@localhost redis]# ./bin/redis-cli  <br/>
# 簡易操作
### 在客戶端輸入 set name abcd<br/>
### get name 可得到abcd<br/>
###<br/>
###<br/>

