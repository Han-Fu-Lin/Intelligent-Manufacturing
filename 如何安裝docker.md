# 參考資料
技術爬爬蝦 https://github.com/tech-shrimp/docker_installer

# 啟動BIOS虛擬化支援
- 搜尋欄搜尋"控制台"
- "程式集"點選"解除安裝程式"
- 點選"開啟或關閉Windows功能"
- 打勾"Hyper-V"、"Windows Hpersvisor平台"、"Windows子系統Linux版"、"容器"、"虛擬機平台"
- 安裝後，重啟電腦
- wsl --set-default-version 2
- wsl --update --web-download
- wsl --install
- 上敘步驟安裝unbuntu至wsl 2

# 安裝Docker Desktop
https://github.com/tech-shrimp/docker_installer/releases

# PULL鏡相檔