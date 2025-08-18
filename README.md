# tixcraft_bot
MaxBot是一個免費、開放原始碼的搶票機器人。祝您搶票成功。

MaxBot is a FREE and open source bot program. Good luck getting your expected ticket.

## Features (功能特色)

### 🎫 支援多個票務網站
- **KKTIX** - 自動登入 (Email + 密碼)
- **TixCraft** - 拓元售票系統
- **TicketPlus** - 自動登入 (電話號碼 + 密碼) ✨新功能
- **Facebook** - 自動登入 (Email + 密碼)
- **CityLine** - 城市售票網
- **URBTIX** - 城市電腦售票網
- **FamiTicket** - 全家便利商店購票系統
- **ibon** - 統一超商購票系統

### 🔐 自動登入功能
- **密碼管理**: 在設定中輸入一次密碼，自動套用到支援的網站
- **多帳號支援**: 每個網站可設定不同的帳號
- **安全儲存**: 密碼在本地設定檔中加密儲存

### 🤖 智能自動化
- 自動選擇日期和場次
- 自動選擇座位區域
- 自動填入票券數量
- 驗證碼辨識 (OCR)
- 自動重新載入售票頁面
- 音效提醒

### 📱 使用者界面
- 圖形化設定介面 (GUI)
- 多語言支援 (中文、英文、日文)
- 詳細的設定選項
- 即時狀態顯示

## 最新更新 (Latest Updates)

### ✨ TicketPlus 自動登入功能 (2025-01-18)
- 新增 TicketPlus 電話號碼 + 密碼自動登入
- 智能表單元素偵測
- 支援多種登入頁面格式
- 詳細錯誤訊息和除錯功能

使用方法：
1. 在「Advanced」設定頁面中輸入 TicketPlus 電話號碼
2. 輸入密碼（與其他網站共用）
3. 程式會自動在 TicketPlus 登入頁面填入帳號密碼

詳細說明請參考：[TicketPlus 登入功能使用說明](TICKETPLUS_LOGIN_GUIDE.md)

# Download (搶票程式下載)
https://github.com/max32002/tixcraft_bot/releases

# Demo (示範影片)

Max搶票機器人 (2023-01-12) tixcraft 猜測驗證碼後不送出

https://youtu.be/mVzyDUV8Mao

Max搶票機器人 (2023-01-11) tixcraft 自動輸入驗證碼

https://youtu.be/t1k0CvmBNhQ (macOS)

https://youtu.be/6JdEdcW8LtY (Windows)

Max搶票機器人 (2023-01-07)：輸入驗證問題答案為"同意"

https://youtu.be/UgemzrsCC-M

Max搶票機器人 (2023-01-05)：不等 cityline 的 10秒，直接重導網址

https://youtu.be/wGU4GJJ-ufw

Max搶票機器人 (2023-01-02)：KKITX自動猜測驗證問題

https://youtu.be/7CtSVBGwx9I (macOS)

https://youtu.be/BcyfkXF2AJU (Windows)

Max搶票機器人 (2023-01-02)：支援 ibon 售票系統

https://youtu.be/VaYc5GKk1Rk

Max搶票機器人 (2023-01-01)：支援新版本的 cityline

https://youtu.be/R5LY7pJgAzI (macOS)

https://youtu.be/2UNaAEjysvk (Windows)

Max搶票機器人 (2023-01-01)：支援新版本的 urbtix

https://youtu.be/_6jxqVC39x8 (macOS)

https://youtu.be/PWKBZ8aG9Rg (Windows)

Max搶票機器人 (2022-12-22)：支援新版本的 cityline

https://youtu.be/KOhQ2XdfjjQ

Max搶票機器人 (2022-11-24)：KKTix 支援避開「剩餘 1」的區域的功能。增加關鍵字#2 的欄位。

https://youtu.be/nupJlwRNOIA

Max搶票機器人 (2022-11-18)：增加 adblock plus 的功能。輸入驗證碼時，會播放音效，在清票時很有幫功，不需要一直緊盯著螢幕。

https://youtu.be/Atujl8MPHQI

Max搶票機器人 (2022-11-06)：優化kktix/拓元的關鍵字比對，修改為不區分逗號、空格與大小寫。

https://youtu.be/v9mI02kVaNw

Max搶票機器人 (2022-10-22)：優化kktix/拓元的價格的關鍵字比對。

https://youtu.be/NZzQcDQkrNI

Max搶票機器人 (2022-10-21)：針對kktix 活動增加第二個關鍵字欄位。

https://youtu.be/x-OdqvUupiA

Max搶票機器人 (2022-01-26)：FamiTicket

https://youtu.be/ZV-G91FHVik

Max搶票機器人 (2022-03-24):

https://youtu.be/AmOYg8Oj0qM

# How to use (如何使用)
* tixcraft: https://max-everyday.com/2018/03/tixcraft-bot/
* kktix: https://max-everyday.com/2018/12/kktix-bot/
* cityline: https://max-everyday.com/2019/03/cityline-bot/
* urbtix: https://max-everyday.com/2019/02/urbtix-bot/
* FamiTicket: https://max-everyday.com/2019/01/maxbot-famiticket/
* ibon: https://max-everyday.com/2023/01/ibon-bot/

# How to execute source code (透過原始碼的執行方法)
1: download chromedrive to "webdriver" folder:
http://chromedriver.chromium.org/downloads

change the chromedrive in chrome_tixcraft.py, source code:
<code>chromedriver_path =Root_Dir+ "webdriver/chromedriver"</code>
the default path is the script path + "webdriver/chromedriver", My suggestion is to create a new directory, then move the chromedrive under new folder.

2: <code>python3 -m pip install selenium</code>

3: <code>python3 settings.py</code>

PS:
* this script only running in python3. (原始碼只可以在 python3 下執行。）
* 請先確定你的python 執行環境下已安裝 selenium 及相關的套件，請參考 pip-reg.txt 檔案內容。
* 如果是 2022-09-13 之前的版本，請到ChromeDriver網站 ([https://chromedriver.chromium.org/](https://chromedriver.chromium.org/)) 下載與您目前相同版本的 ChromeDriver 的執行檔，放在搶票程式的webdriver目錄下(Mac電腦請放到 MaxBot.app 套件裡的 /Contents/Resources/webdriver/)，在執行搶票程式前，第一次執行搶票主程式前，前請先手動點 ChromeDriver 的執行檔。
* 透過 python3 執行 settings.py 就可以有 GUI 的設定界面。
* 如果你是使用 macOS 並且執行環境沒有 python3，請 python 官方網站([https://www.python.org/downloads/](https://www.python.org/downloads/))來安裝 python3, 如果在 macOS 裡會使用終端機(Terminal)，建議使用 https://brew.sh/ 安裝 python3.
* 如果你是使用 Firefox, ChromeDriver 的元件是叫 geckodriver，下載點在：https://github.com/mozilla/geckodriver/releases ，與 ChromeDriver 的處理方式是一樣，如果是 mac 電腦，要在元件按右鍵開啟，做一次授權的動作，mac 有2個版本，-macos.tar.gz 與 -macos-aarch64.tar.gz ，如果是 intel CPU 的版本，請服用前面沒有 aarch64 的版本。

# Introduce the implement (實作方法)
https://stackoverflow.max-everyday.com/2018/03/selenium-chrome-webdriver/

# Execute suggestion (搶票建議)
please run this source code with high performance hardware computer and high speed + stable network.

門票的「限量」是很殘酷的，建議不要用破舊的電腦或連線不穩的手機網路來搶票，因為只要比別人慢個 0.1 秒，票可能就沒了。為了要搶到限量的票真心建議去一下網咖或找一個網路連線穩定且快的地方並使用硬體不差的電腦來搶票。

# TODO about cpatcha (關於驗證碼)

目前驗證碼需要手動輸入，也許你會想自動輸入驗證碼，可以參考看看：實作基於CNN的台鐵訂票驗證碼辨識以及透過模仿及資料增強的訓練集產生器 (Simple captcha solver based on CNN and a training set generator by imitating the style of captcha and data augmentation)
https://github.com/JasonLiTW/simple-railway-captcha-solver

# Donate (贊助Max)

如果你覺得這篇文章或MaxBot寫的很好，想打賞Max，贊助方式如下： https://max-everyday.com/about/#donate
