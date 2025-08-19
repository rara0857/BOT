# 設定檔說明

## 初次使用設定

1. **複製範本檔案**：
   ```bash
   cp settings.json.template settings.json
   ```

2. **編輯 settings.json**，填入您的個人資訊：
   - `facebook_account`: 您的 Facebook 帳號
   - `kktix_account`: 您的 KKTIX 帳號  
   - `password`: 您的密碼
   - `ticketplus_account`: 您的 TicketPlus 手機號碼

## 重要提醒

⚠️ **請勿將 settings.json 檔案上傳到公開的程式碼儲存庫！**

- settings.json 已加入 .gitignore，不會被 Git 追蹤
- 只有 settings.json.template 會被上傳，不包含任何敏感資訊
- 每次 clone 專案後都需要重新設定 settings.json

## 設定選項說明

- `ticket_number`: 搶票數量
- `homepage`: 預設首頁
- `area_keyword_1`: 票區關鍵字搜尋
- `auto_check_agree`: 自動勾選同意條款
- `debug`: 除錯模式（顯示更多資訊）
