# HiShops Email Templates

HiShops 電商平台的電子郵件模板集合，提供各種業務場景的專業 email 通知服務。

## 📁 專案結構

```
email template/
├── new/                    # 新製作模板（尚未排入正式使用）
│   ├── annual-fee-notification.html
│   ├── campaign-abnormal-offline-notification.html
│   ├── campaign-created-notification.html
│   ├── campaign-upcoming-notification.html
│   ├── emergency-maintenance-notification.html
│   ├── feature-release-notification.html
│   ├── festival-greeting-notification.html
│   ├── hicoin-purchase-notification.html
│   ├── hipoint-ai-token-redeem-notification.html
│   ├── inventory-low-notification.html
│   ├── kol-commission-payout-notification.html
│   ├── kol-invite-hidden-campaign-notification.html
│   ├── level-upgrade-notification.html
│   ├── performance-achievement-notification.html
│   ├── point-expiry-notification.html
│   ├── point-redeem-service-notification.html
│   ├── policy-update-notification.html
│   ├── product-offline-notification.html
│   ├── referral-link-generated-notification.html
│   ├── report-generated-notification.html
│   ├── refund-completed-notification.html
│   ├── scheduled-maintenance-notification.html
│   ├── security-alert-notification.html
│   └── internal-beta-test-invitation.html
└── old/                    # 已正式使用的模板
    ├── ec-password-changed.html
    ├── ec-password-reset.html
    ├── ec-signup-verify-email.html
    ├── ec-welcome-message.html
    ├── hishops-signup-verify-email.html
    ├── password-changed.html
    ├── password-reset.html
    └── welcome-message.html
```

## 🎯 模板分類

### 新製作模板 (new/)

#### 用戶通知類
- **annual-fee-notification.html** - 年費通知
- **level-upgrade-notification.html** - 等級升級通知
- **point-expiry-notification.html** - 點數到期通知
- **point-redeem-service-notification.html** - 點數兌換服務通知

#### 活動行銷類
- **campaign-created-notification.html** - 活動創建通知
- **campaign-upcoming-notification.html** - 活動即將開始通知
- **campaign-abnormal-offline-notification.html** - 活動異常下線通知
- **festival-greeting-notification.html** - 節日問候通知

#### 系統維護類
- **emergency-maintenance-notification.html** - 緊急維護通知
- **scheduled-maintenance-notification.html** - 定期維護通知
- **feature-release-notification.html** - 功能發布通知

#### 安全與政策類
- **security-alert-notification.html** - 安全警報通知
- **policy-update-notification.html** - 政策更新通知

#### 業務運營類
- **inventory-low-notification.html** - 庫存不足通知
- **product-offline-notification.html** - 商品下架通知
- **refund-completed-notification.html** - 退款完成通知
- **report-generated-notification.html** - 報表生成通知

#### KOL 與推廣類
- **kol-commission-payout-notification.html** - KOL 佣金發放通知
- **kol-invite-hidden-campaign-notification.html** - KOL 隱藏活動邀請通知
- **referral-link-generated-notification.html** - 推薦連結生成通知

#### 虛擬貨幣類
- **hicoin-purchase-notification.html** - HiCoin 購買通知
- **hipoint-ai-token-redeem-notification.html** - HiPoint AI 代幣兌換通知

#### 績效與成就類
- **performance-achievement-notification.html** - 績效成就通知

#### 內部測試類
- **internal-beta-test-invitation.html** - 內部封閉測試邀請

### 已使用模板 (old/)

#### 用戶認證類
- **ec-password-changed.html** - EC 密碼變更通知
- **ec-password-reset.html** - EC 密碼重設通知
- **ec-signup-verify-email.html** - EC 註冊驗證郵件
- **ec-welcome-message.html** - EC 歡迎訊息
- **hishops-signup-verify-email.html** - HiShops 註冊驗證郵件
- **password-changed.html** - 密碼變更通知
- **password-reset.html** - 密碼重設通知
- **welcome-message.html** - 歡迎訊息

## 🎨 設計特色

### 視覺設計
- **響應式設計**：支援各種設備和螢幕尺寸
- **品牌一致性**：統一使用 HiShops 品牌色彩和 Logo
- **專業排版**：清晰的資訊層次和易讀性

### 色彩系統
- **主色調**：`#009ef7` (藍色) - 用於主要標題和連結
- **成功色**：`#28a745` (綠色) - 用於正面訊息
- **警告色**：`#d7263d` (紅色) - 用於重要提醒
- **中性色**：`#7E8299` (灰色) - 用於次要文字

### 結構特色
- **標準化佈局**：統一的 header、content、footer 結構
- **模組化設計**：易於維護和更新的模板結構
- **多語言支援**：支援繁體中文內容

## 🚀 使用方式

### 1. 模板選擇
根據業務需求選擇對應的模板：
```html
<!-- 例如：發送退款完成通知 -->
email template/new/refund-completed-notification.html
```

### 2. 內容自訂
替換模板中的變數標記：
```html
<!-- 原始模板 -->
<li>訂單編號：[訂單編號]</li>
<li>退款金額：[退款金額]</li>

<!-- 實際使用 -->
<li>訂單編號：ORD-2024-001</li>
<li>退款金額：NT$ 1,500</li>
```

### 3. 發送測試
- 使用 HTML 郵件客戶端進行預覽
- 測試不同設備的顯示效果
- 確認連結和圖片正常顯示

## 📋 開發規範

### 命名規範
- 使用 kebab-case 命名方式
- 檔名應清楚描述模板用途
- 包含 `-notification.html` 或 `-invitation.html` 後綴

### HTML 結構
```html
<style>html,body { padding: 0; margin:0; }</style>
<div style="font-family:Arial,Helvetica,sans-serif; ...">
  <table align="center" ...>
    <!-- Header with Logo -->
    <!-- Content Area -->
    <!-- Footer with Contact Info -->
  </table>
</div>
```

### CSS 內聯樣式
- 使用內聯 CSS 確保郵件客戶端相容性
- 避免使用外部樣式表
- 優先使用 table 佈局確保跨平台相容性

## 🔄 版本管理

### 新模板開發流程
1. 在 `new/` 資料夾中創建新模板
2. 進行內部測試和審查
3. 確認無誤後移至 `old/` 資料夾正式使用
4. 更新版本記錄

### 模板更新原則
- 保持向後相容性
- 記錄重大變更
- 進行充分測試後發布

## 📞 聯絡資訊

- **Email**：service@hishops.com.tw
- **電話**：02-0000-0000
- **地址**：台北市重慶北路一段26巷9弄1號3樓

## 📄 授權

本專案為 HiShops 內部使用，版權所有。

---

**HiShops 開發團隊**  
*打造優質的電商平台體驗*
