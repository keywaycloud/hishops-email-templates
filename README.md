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
