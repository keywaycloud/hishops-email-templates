# HiShops Email Templates

HiShops 電商平台的電子郵件模板集合，提供各種業務場景的專業 email 通知服務。

## 📁 專案結構

```
hishops-email-templates/
├── mall_customer/                    # 買家郵件模板（賣家寄送給買家）
│   ├── ec-email-changed.html
│   ├── ec-password-changed.html
│   ├── ec-password-reset.html
│   ├── ec-refund-completed-notification.html
│   ├── ec-signup-verify-email.html
│   └── ec-welcome-message.html
├── mall_seller/                      # 賣家郵件模板（平台寄送給賣家）
│   ├── account/                      # 帳號相關
│   │   ├── email-changed.html
│   │   ├── hishops-signup-verify-email.html
│   │   ├── password-changed.html
│   │   ├── password-reset.html
│   │   └── security-alert-notification.html
│   ├── billing/                      # 帳務相關
│   │   ├── annual-fee-notification.html
│   │   ├── hicoin-purchase-notification.html
│   │   └── hipoint-ai-token-redeem-notification.html
│   ├── events/                       # 活動相關
│   │   ├── campaign-abnormal-offline-notification.html
│   │   ├── campaign-created-notification.html
│   │   └── campaign-upcoming-notification.html
│   ├── KOL relate/                   # KOL 相關
│   │   ├── kol-commission-payout-notification.html
│   │   └── kol-invite-hidden-campaign-notification.html
│   ├── inventory-low-notification.html
│   ├── level-upgrade-notification.html
│   ├── performance-achievement-notification.html
│   ├── point-expiry-notification.html
│   ├── point-redeem-service-notification.html
│   ├── product-offline-notification.html
│   ├── referral-link-generated-notification.html
│   ├── report-generated-notification.html
│   ├── scheduled-maintenance-notification.html
│   ├── welcome-message.html
│   └── STYLE_GUIDE.md                # 樣式指南
└── system/                           # 系統相關郵件
    ├── emergency-maintenance-notification.html
    ├── feature-release-notification.html
    ├── festival-greeting-notification.html
    └── policy-update-notification.html
```

## 🎯 模板分類

### 買家郵件模板 (mall_customer/)

**說明**：這些郵件是賣家寄送給買家的，使用**變體三**格式（動態品牌 Logo/名稱）。郵件以賣家身份直接與買家溝通，不顯示平台商（好嗨商）的品牌資訊。

#### 帳號認證類
- **ec-email-changed.html** - Email 修改確認通知
- **ec-password-changed.html** - 密碼變更通知
- **ec-password-reset.html** - 密碼重置通知
- **ec-signup-verify-email.html** - 帳號驗證通知

#### 歡迎與通知類
- **ec-welcome-message.html** - 歡迎訊息（使用**變體二**格式）
- **ec-refund-completed-notification.html** - 退款完成通知

### 賣家郵件模板 (mall_seller/)

**說明**：這些郵件是平台寄送給賣家的，使用**變體一**格式（橫向品牌 Logo）。郵件以平台商（好嗨商）身份與賣家溝通。

#### 帳號相關 (account/)
- **email-changed.html** - Email 修改申請通知
- **hishops-signup-verify-email.html** - 帳號驗證通知
- **password-changed.html** - 密碼變更通知
- **password-reset.html** - 密碼重置通知
- **security-alert-notification.html** - 帳號安全異常警告

#### 帳務相關 (billing/)
- **annual-fee-notification.html** - 年費通知
- **hicoin-purchase-notification.html** - HiCoin 購買通知
- **hipoint-ai-token-redeem-notification.html** - HiPoint AI 代幣兌換通知

#### 活動相關 (events/)
- **campaign-created-notification.html** - 活動創建通知
- **campaign-upcoming-notification.html** - 活動即將開始通知
- **campaign-abnormal-offline-notification.html** - 活動異常下線通知

#### KOL 相關 (KOL relate/)
- **kol-commission-payout-notification.html** - KOL 佣金發放通知
- **kol-invite-hidden-campaign-notification.html** - KOL 隱藏活動邀請通知

#### 其他通知類
- **inventory-low-notification.html** - 庫存不足通知
- **level-upgrade-notification.html** - 等級升級通知
- **performance-achievement-notification.html** - 績效成就通知
- **point-expiry-notification.html** - 點數到期通知
- **point-redeem-service-notification.html** - 點數兌換服務通知
- **product-offline-notification.html** - 商品下架通知
- **referral-link-generated-notification.html** - 推薦連結生成通知
- **report-generated-notification.html** - 報表生成通知
- **scheduled-maintenance-notification.html** - 定期維護通知
- **welcome-message.html** - 歡迎訊息

### 系統郵件模板 (system/)

**說明**：系統層級的郵件通知，可能使用變體一或變體二格式。

- **emergency-maintenance-notification.html** - 緊急維護通知
- **feature-release-notification.html** - 功能發布通知
- **festival-greeting-notification.html** - 節日問候通知
- **policy-update-notification.html** - 政策更新通知

## 🎨 設計特色

### 樣式變體

本專案使用三種主要的樣式變體，詳細規範請參考 `mall_seller/STYLE_GUIDE.md`：

#### 變體一：橫向品牌 Logo（卡片外上方）
- **適用場景**：賣家郵件模板（mall_seller/）
- **特點**：Logo 位於卡片外部上方，橫向排列 Logo + 品牌名稱「好嗨商」
- **使用範例**：`mall_seller/account/email-changed.html`

#### 變體二：Banner 圖片（卡片內）
- **適用場景**：歡迎郵件、行銷類郵件
- **特點**：Banner/Logo 位於卡片內部，使用橫向 banner 圖片
- **使用範例**：`mall_customer/ec-welcome-message.html`

#### 變體三：動態品牌 Logo/名稱（卡片外上方，支援條件顯示）
- **適用場景**：買家郵件模板（mall_customer/）
- **特點**：
  - Logo 和品牌名稱位於卡片外部上方
  - 使用 Thymeleaf 條件判斷，支援兩種顯示模式：
    - 有 Logo：顯示 Logo + 品牌名稱（橫向排列）
    - 無 Logo：僅顯示品牌名稱
  - 適用於賣家寄送給買家的郵件，使用動態賣家資訊
- **使用範例**：`mall_customer/ec-email-changed.html`

### 視覺設計
- **響應式設計**：支援各種設備和螢幕尺寸
- **品牌一致性**：
  - 賣家郵件：統一使用 HiShops 品牌色彩和 Logo
  - 買家郵件：使用動態賣家品牌資訊
- **專業排版**：清晰的資訊層次和易讀性

### 色彩系統
- **主色調**：`#009ef7` (藍色) - 用於主要標題和連結
- **品牌主色**：`#152022` - 好嗨商品牌主色（用於按鈕背景）
- **強調色**：`#e7ff25` - 黃綠色強調色（用於按鈕文字）
- **成功色**：`#50cd89` (綠色) - 用於正面訊息
- **警告色**：`#d7263d` (紅色) - 用於重要提醒
- **中性色**：`#7E8299` (灰色) - 用於次要文字

### 結構特色
- **標準化佈局**：統一的 header、content、footer 結構
- **模組化設計**：易於維護和更新的模板結構
- **多語言支援**：支援繁體中文內容
- **動態變數**：使用 Thymeleaf 模板引擎支援動態內容

## 🚀 使用方式

### 1. 模板選擇
根據業務需求和收件對象選擇對應的模板：

**賣家郵件**（平台 → 賣家）：
```html
<!-- 例如：發送帳號驗證郵件給賣家 -->
mall_seller/account/hishops-signup-verify-email.html
```

**買家郵件**（賣家 → 買家）：
```html
<!-- 例如：發送退款完成通知給買家 -->
mall_customer/ec-refund-completed-notification.html
```

### 2. Thymeleaf 變數使用

#### 賣家郵件變數
使用標準的 Thymeleaf 語法：
```html
<span th:text="${verificationUrl}">[verificationUrl]</span>
<a th:href="${verificationUrl}">確認連結</a>
```

#### 買家郵件變數（變體三）
使用動態賣家資訊：
```html
<!-- 賣家名稱（必填） -->
<span th:text="${storeInfo.teamName}">[storeName]</span>

<!-- 賣家 Logo（可選） -->
<img th:src="${storeInfo.storeLogo}" th:if="${storeInfo.storeLogo != null and storeInfo.storeLogo != ''}" />

<!-- 賣家客服資訊（可選） -->
<a th:href="'mailto:' + ${storeInfo.serviceEmail}" th:text="${storeInfo.serviceEmail}" th:if="${storeInfo.serviceEmail != null and storeInfo.serviceEmail != ''}">[serviceEmail]</a>
<a th:href="'tel:' + ${storeInfo.servicePhone}" th:text="${storeInfo.servicePhone}" th:if="${storeInfo.servicePhone != null and storeInfo.servicePhone != ''}">[servicePhone]</a>
```

### 3. 發送測試
- 使用 HTML 郵件客戶端進行預覽
- 測試不同設備的顯示效果
- 確認連結和圖片正常顯示
- 測試 Thymeleaf 變數的正確渲染

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
- **必須使用內聯 CSS** 確保郵件客戶端相容性
- 避免使用外部樣式表（大多數郵件客戶端不支援）
- 優先使用 table 佈局確保跨平台相容性
- **注意**：IDE 可能會顯示 "CSS inline styles should not be used" 的警告，這是正常的。Email 模板必須使用內聯樣式，因為：
  - Gmail、Outlook 等郵件客戶端會過濾或忽略外部 CSS 和 `<style>` 標籤
  - 內聯樣式是 Email HTML 開發的業界標準做法
  - 如需忽略此警告，已建立 `.stylelintignore` 配置文件

## 📐 樣式指南

詳細的樣式規範、變體說明和最佳實踐請參考：
- **`mall_seller/STYLE_GUIDE.md`** - 完整的樣式指南文檔

### 快速參考

**變體選擇指南**：
- 賣家郵件 → 使用**變體一**（橫向品牌 Logo）
- 買家歡迎郵件 → 使用**變體二**（Banner 圖片）
- 買家其他郵件 → 使用**變體三**（動態品牌 Logo/名稱）

**重要原則**：
- 所有 CSS 必須使用 inline styles（郵件客戶端限制）
- 使用 table-based 佈局確保跨客戶端兼容性
- 避免使用現代 CSS 功能（flexbox、grid 等）
- 聯絡資訊和 Footer 為固定區塊，應保持一致

## 🔄 版本管理

### 模板開發流程
1. 根據業務需求選擇適當的變體格式
2. 參考 `mall_seller/STYLE_GUIDE.md` 中的規範
3. 使用對應目錄下的現有模板作為參考
4. 進行內部測試和審查
5. 確認無誤後提交使用

### 模板更新原則
- 保持向後相容性
- 遵循樣式指南規範
- 記錄重大變更
- 進行充分測試後發布

## 📞 聯絡資訊

### 平台客服（賣家郵件使用）
- **官方LINE**：@322sqanl
- **聯絡電話**：02-2558-0837
- **客服信箱**：services.hishops@gmail.com

### 賣家客服（買家郵件使用）
買家郵件模板使用動態變數 `${storeInfo.serviceEmail}` 和 `${storeInfo.servicePhone}`，由系統根據賣家設定自動填入。

## 📄 授權

本專案為 HiShops 內部使用，版權所有。

---

**HiShops 開發團隊**  
*打造優質的電商平台體驗*
