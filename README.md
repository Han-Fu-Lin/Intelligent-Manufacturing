# 介紹
什麼是Node-Red!?Node-Red是IBM推出的一款基於流程編程的視覺化程式設計語言開發工具，通過這一工具，開發者可以將硬體設備與應用程式接口和在線服務相連。並組成一個物聯網系統

參考安全智慧監控設計文檔，我們將使用Node-Red做為PLC資料收集&數據傳輸的工具

# 執行環境 Node.js
Node.js是基於javascript的跨平台、開源的執行環境，而Node-Red基於Node.js並專門用在物連網的視覺化套件

# Windows系統適用版本
適用Windows 10系統以上(含)

# 建置Node-Red執行環境
## 取得打包的Node-Red執行檔(.exe)
- 路徑:<K:\@安全智慧監控項目\1.Node-Red主程式>

## 下載壓縮包
- 從高雄廠K槽複製Node-RED-SFE-KH.zip
- 儲存於本地端或虛擬端，並將其解壓縮打開

# 啟動Node-Red開發環境
## 執行node-red-sfe.exe
- 路徑如:Users\Node-RED-SFE-KH\build\dist
- 點擊&執行node-red-sfe.exe
- 允許Node.js執行權限
- Node-Red執行程式位於工作列,請勿關閉

## 訪問Node-Red編輯環境
- Node-Red執行檔已完成啟動(工作列上)
- 打開瀏覽器訪問:<http:127.0.0.1:1880>

## 模組安裝
- 訪問Node-Red官網<https://nodered.org/>，在flows頁面找尋適合的模組
- 下載模組放入資料夾，路徑如:Users\Node-RED-SFE-KH\build\dist\NRUserDir\node_modules
- 本機端安裝Node.js可使用npm套件安裝模組
- 模組打包檔:<K:\@安全智慧監控項目\2.Node-Red模組>

## 節點版本
- node-red v4.0.2
- node-red-contrib-calc v1.0.6
- node-red-contrib-controltimer v0.4.1
- node-red-contrib-float v1.0.3
- node-red-contrib-google-sheets v1.1.2
- node-red-contrib-influxdb v0.7.0
- node-red-contrib-line-notify v3.1.3
- node-red-contrib-modbus v5.43.0
- node-red-contrib-ui-led v0.4.11
- node-red-dashboard v3.6.5
- node-red-node-ui-table v0.4.4

# 建置InfluxDB資料庫
## 下載InfluDB V2 & Influx CLI
- 路徑:<K:\@安全智慧監控項目\3.InfluxDB資料庫>
- influxdb2-2.7.10-windows.zip
- influxdb2-client-2.7.5-windows-amd64.zip

## 安裝資料庫
- 將下載的壓縮檔放置於C:\Program Files\InfluxData\influxdb資料夾內

## 啟動InfluxDB
- 製作一個bat檔，並將下面資訊打入
- cd -Path 'C:\Program Files\InfluxData\influxdb'
- ./influxd

## 將bat檔放置開機啟動設置