# 🚨 Missing Blade Templates - Complete Inventory

**Last Updated**: November 2025  
**Status**: Comprehensive audit of all missing views  
**Total Missing Views**: **~170+ Blade Templates**

---

## 📋 **Quick Summary**

This document provides a complete inventory of all missing Blade templates required for the GoTrash Laravel application. The templates are organized by module/feature area with priority levels.

### **Critical Missing Areas:**
1. 🔴 **Merchant Platform** - 45 views (100% missing) - HIGH PRIORITY
2. 🔴 **Cleaner Platform** - 12 views (85% missing) - HIGH PRIORITY  
3. 🔴 **Guest Booking** - 8 views (100% missing) - HIGH PRIORITY
4. 🟡 **User Section** - 20 views (Partial missing) - MEDIUM PRIORITY
5. 🟡 **Admin Section** - 18 views (Partial missing) - MEDIUM PRIORITY
6. 🟡 **Reviews & Ratings** - 4 views (100% missing) - MEDIUM PRIORITY

### **Key Findings:**
- **MerchantController**: Currently API-only, needs web routes and views
- **GuestOrderController**: Currently API-only, needs public web routes and views
- **WalletController**: Currently API-only, needs web routes and views
- **ProductController**: Currently API-only, needs web routes and views
- **Cleaner Controllers**: Some views exist, but many critical ones are missing

---

## 📋 **Detailed Summary**

This document lists **ALL** missing Blade templates required for the GoTrash Laravel application. The templates are organized by module/feature area.

---

## 🔴 **1. MERCHANT PLATFORM VIEWS** (100% Missing)

### **1.1 Merchant Dashboard & Authentication**
- ❌ `resources/views/merchant/layouts/app.blade.php` - Merchant main layout
- ❌ `resources/views/merchant/auth/login.blade.php` - Merchant login page
- ❌ `resources/views/merchant/auth/register.blade.php` - Merchant registration/onboarding
- ❌ `resources/views/merchant/dashboard.blade.php` - Merchant dashboard (main)
- ❌ `resources/views/merchant/partials/navigation.blade.php` - Merchant navigation menu
- ❌ `resources/views/merchant/partials/sidebar.blade.php` - Merchant sidebar

### **1.2 Merchant Profile & Settings**
- ❌ `resources/views/merchant/profile/index.blade.php` - Merchant profile page
- ❌ `resources/views/merchant/profile/edit.blade.php` - Edit merchant profile
- ❌ `resources/views/merchant/settings/index.blade.php` - Merchant settings
- ❌ `resources/views/merchant/settings/bank-accounts.blade.php` - Bank account management
- ❌ `resources/views/merchant/settings/settlement.blade.php` - Settlement settings

### **1.3 Merchant KYC**
- ❌ `resources/views/merchant/kyc/index.blade.php` - KYC overview
- ❌ `resources/views/merchant/kyc/upload.blade.php` - KYC document upload
- ❌ `resources/views/merchant/kyc/status.blade.php` - KYC status page
- ❌ `resources/views/merchant/kyc/pending.blade.php` - KYC pending status

### **1.4 Product Management**
- ❌ `resources/views/merchant/products/index.blade.php` - Product listing
- ❌ `resources/views/merchant/products/create.blade.php` - Create product form
- ❌ `resources/views/merchant/products/edit.blade.php` - Edit product form
- ❌ `resources/views/merchant/products/show.blade.php` - Product details
- ❌ `resources/views/merchant/products/bulk-upload.blade.php` - Bulk product upload

### **1.5 RFID Management**
- ❌ `resources/views/merchant/rfid/index.blade.php` - RFID tags listing
- ❌ `resources/views/merchant/rfid/assign.blade.php` - Assign RFID to product
- ❌ `resources/views/merchant/rfid/scan.blade.php` - RFID scanner interface
- ❌ `resources/views/merchant/rfid/bulk-assign.blade.php` - Bulk RFID assignment

### **1.6 Inventory Management**
- ❌ `resources/views/merchant/inventory/index.blade.php` - Inventory overview
- ❌ `resources/views/merchant/inventory/stock-alerts.blade.php` - Low stock alerts
- ❌ `resources/views/merchant/inventory/adjustments.blade.php` - Stock adjustments
- ❌ `resources/views/merchant/inventory/scan-add.blade.php` - Scan to add stock
- ❌ `resources/views/merchant/inventory/scan-remove.blade.php` - Scan to remove stock
- ❌ `resources/views/merchant/inventory/history.blade.php` - Inventory history

### **1.7 Sales & Transactions**
- ❌ `resources/views/merchant/sales/index.blade.php` - Sales dashboard
- ❌ `resources/views/merchant/sales/transactions.blade.php` - Transaction history
- ❌ `resources/views/merchant/sales/analytics.blade.php` - Sales analytics
- ❌ `resources/views/merchant/sales/reports.blade.php` - Sales reports
- ❌ `resources/views/merchant/sales/daily.blade.php` - Daily sales report

### **1.8 Wallet & Withdrawals**
- ❌ `resources/views/merchant/wallet/index.blade.php` - Wallet balance & overview
- ❌ `resources/views/merchant/wallet/transactions.blade.php` - Wallet transactions
- ❌ `resources/views/merchant/wallet/withdraw.blade.php` - Withdrawal request form
- ❌ `resources/views/merchant/wallet/withdrawal-history.blade.php` - Withdrawal history
- ❌ `resources/views/merchant/wallet/topup.blade.php` - Wallet top-up (if needed)

### **1.9 Checkout & QR Codes**
- ❌ `resources/views/merchant/checkout/qr-generator.blade.php` - QR code generator
- ❌ `resources/views/merchant/checkout/point-of-sale.blade.php` - POS interface
- ❌ `resources/views/merchant/checkout/settings.blade.php` - Checkout settings

### **1.10 Merchant Routes Required**
- ❌ `routes/merchant.php` - Merchant route file (needs to be created)

---

## 🔴 **2. CLEANER PLATFORM VIEWS** (85% Missing)

### **2.1 Cleaner Dashboard** ✅ (EXISTS)
- ✅ `resources/views/cleaner/dashboard.blade.php` - Cleaner dashboard (EXISTS)
- ✅ `resources/views/cleaner/layouts/app.blade.php` - Cleaner layout (EXISTS)

### **2.2 Cleaner KYC** ❌ (MISSING)
- ❌ `resources/views/cleaner/kyc/index.blade.php` - KYC overview
- ❌ `resources/views/cleaner/kyc/level1.blade.php` - KYC Level 1 form
- ❌ `resources/views/cleaner/kyc/level2.blade.php` - KYC Level 2 form
- ❌ `resources/views/cleaner/kyc/status.blade.php` - KYC status page

### **2.3 Cleaner Commission** ❌ (MISSING)
- ❌ `resources/views/cleaner/commission/index.blade.php` - Commission overview
- ❌ `resources/views/cleaner/commission/history.blade.php` - Commission history
- ❌ `resources/views/cleaner/commission/pending.blade.php` - Pending commissions
- ❌ `resources/views/cleaner/commission/earned.blade.php` - Earned commissions
- ❌ `resources/views/cleaner/commission/request.blade.php` - Commission request form

### **2.4 Cleaner Jobs** ❌ (MISSING)
- ❌ `resources/views/cleaner/jobs/index.blade.php` - Jobs overview
- ❌ `resources/views/cleaner/jobs/notifications.blade.php` - Job notifications
- ❌ `resources/views/cleaner/jobs/history.blade.php` - Job history
- ❌ `resources/views/cleaner/jobs/details.blade.php` - Job details
- ❌ `resources/views/cleaner/jobs/accept.blade.php` - Accept job confirmation
- ❌ `resources/views/cleaner/jobs/complete.blade.php` - Complete job form

### **2.5 Cleaner Profile** ❌ (MISSING)
- ❌ `resources/views/cleaner/profile/index.blade.php` - Profile page

### **2.6 Cleaner Bank Accounts** ❌ (MISSING)
- ❌ `resources/views/cleaner/bank/index.blade.php` - Bank accounts management

### **2.7 Cleaner Earnings & Wallet** ❌ (MISSING)
- ❌ `resources/views/cleaner/wallet/index.blade.php` - GoPay wallet balance
- ❌ `resources/views/cleaner/wallet/transactions.blade.php` - Wallet transactions
- ❌ `resources/views/cleaner/wallet/withdraw.blade.php` - Withdraw earnings
- ❌ `resources/views/cleaner/earnings/summary.blade.php` - Earnings summary

---

## 🔴 **3. GUEST BOOKING VIEWS** (100% Missing)

### **3.1 Guest Booking Forms**
- ❌ `resources/views/guest/booking/cleaning.blade.php` - Guest cleaning booking form
- ❌ `resources/views/guest/booking/dry-cleaning.blade.php` - Guest dry cleaning booking form
- ❌ `resources/views/guest/booking/waste-pickup.blade.php` - Guest waste pickup booking form
- ❌ `resources/views/guest/booking/moving.blade.php` - Guest moving service booking form

### **3.2 Guest Order Tracking**
- ❌ `resources/views/guest/track/index.blade.php` - Public order tracking page
- ❌ `resources/views/guest/track/show.blade.php` - Order tracking details (public)
- ❌ `resources/views/guest/track/timeline.blade.php` - Order timeline view

### **3.3 Guest Order Confirmation**
- ❌ `resources/views/guest/confirmation.blade.php` - Order confirmation page
- ❌ `resources/views/guest/confirmation/sms-sent.blade.php` - SMS tracking link sent confirmation

### **3.4 Guest Routes Required**
- ❌ Guest booking routes in `routes/web.php` or `routes/guest.php`

---

## 🔴 **4. USER SECTION VIEWS** (Partial Missing)

### **4.1 User Requests** ❌ (MISSING)
- ❌ `resources/views/user/requests.blade.php` - User requests listing
- ❌ `resources/views/user/request-details.blade.php` - Request details page

### **4.2 User Wallet & GoPay** ❌ (MISSING)
- ❌ `resources/views/user/wallet/index.blade.php` - Wallet overview (different from balance.blade.php)
- ❌ `resources/views/user/wallet/topup.blade.php` - Wallet top-up form
- ❌ `resources/views/user/wallet/transfer.blade.php` - Wallet transfer form
- ❌ `resources/views/user/wallet/withdraw.blade.php` - Wallet withdrawal form
- ❌ `resources/views/user/wallet/transactions.blade.php` - Wallet transaction history
- ❌ `resources/views/user/wallet/qr-scan.blade.php` - QR code scanner for payments
- ❌ `resources/views/user/wallet/rfid-scan.blade.php` - RFID scanner for payments

### **4.3 User Checkout** ❌ (MISSING)
- ❌ `resources/views/user/checkout/qr.blade.php` - QR checkout page
- ❌ `resources/views/user/checkout/rfid.blade.php` - RFID checkout page
- ❌ `resources/views/user/checkout/cart.blade.php` - Shopping cart
- ❌ `resources/views/user/checkout/confirm.blade.php` - Checkout confirmation

### **4.4 User Product Scanning** ❌ (MISSING)
- ❌ `resources/views/user/products/scan.blade.php` - Product scanner (public)
- ❌ `resources/views/user/products/show.blade.php` - Product details page
- ❌ `resources/views/user/products/search.blade.php` - Product search

### **4.5 User Order History** ❌ (MISSING)
- ❌ `resources/views/user/orders/index.blade.php` - Unified order history
- ❌ `resources/views/user/orders/reorder.blade.php` - Reorder confirmation
- ❌ `resources/views/user/orders/details.blade.php` - Order details

### **4.6 User KYC History** ❌ (MISSING)
- ❌ `resources/views/user/kyc-history.blade.php` - KYC submission history (REFERENCED in UserController)

### **4.7 User Advanced Features** ❌ (MISSING)
- ❌ `resources/views/user/agent-messages.blade.php` - Agent messages (REFERENCED in UserController)
- ❌ `resources/views/user/service-acknowledgments.blade.php` - Service acknowledgments (REFERENCED in UserController)
- ❌ `resources/views/user/referral-system.blade.php` - Referral system (REFERENCED in UserController)
- ❌ `resources/views/user/ratings-reviews.blade.php` - Ratings and reviews (REFERENCED in UserController)
- ❌ `resources/views/user/service-preferences.blade.php` - Service preferences (REFERENCED in UserController)

---

## 🔴 **5. REVIEWS & RATINGS VIEWS** (100% Missing)

### **5.1 Reviews**
- ❌ `resources/views/reviews/index.blade.php` - Reviews listing
- ❌ `resources/views/reviews/create.blade.php` - Create review form
- ❌ `resources/views/reviews/show.blade.php` - Review details
- ❌ `resources/views/reviews/edit.blade.php` - Edit review form

### **5.2 Ratings**
- ❌ `resources/views/ratings/create.blade.php` - Create rating form
- ❌ `resources/views/ratings/show.blade.php` - Rating details

---

## 🔴 **6. ADMIN SECTION VIEWS** (Partial Missing)

### **6.1 Admin Merchant Management** ❌ (MISSING)
- ❌ `resources/views/admin/merchants/index.blade.php` - Merchant listing
- ❌ `resources/views/admin/merchants/show.blade.php` - Merchant details
- ❌ `resources/views/admin/merchants/kyc-review.blade.php` - Merchant KYC review
- ❌ `resources/views/admin/merchants/approve.blade.php` - Approve merchant
- ❌ `resources/views/admin/merchants/products.blade.php` - Merchant products management
- ❌ `resources/views/admin/merchants/transactions.blade.php` - Merchant transactions
- ❌ `resources/views/admin/merchants/withdrawals.blade.php` - Merchant withdrawals

### **6.2 Admin Payment & Commission Management** ❌ (MISSING)
- ❌ `resources/views/admin/payments.blade.php` - Payments listing (REFERENCED in AdminController)
- ❌ `resources/views/admin/commissions.blade.php` - Commissions listing (REFERENCED in AdminController)
- ❌ `resources/views/admin/financial/pending-bonuses.blade.php` - Pending bonuses (REFERENCED in AdminController)
- ❌ `resources/views/admin/financial/commission-report.blade.php` - Commission report (REFERENCED in AdminController)
- ❌ `resources/views/admin/financial/report.blade.php` - Financial report (REFERENCED in AdminController)

### **6.3 Admin Agent Management** ❌ (MISSING)
- ❌ `resources/views/admin/agents/details.blade.php` - Agent details page (REFERENCED in AdminController)

### **6.4 Admin Disposal Management** ❌ (MISSING)
- ❌ `resources/views/admin/disposal/unconfirmed.blade.php` - Unconfirmed disposals (REFERENCED in AdminController)
- ❌ `resources/views/admin/disposal/report.blade.php` - Disposal report (REFERENCED in AdminController)

### **6.5 Admin Reports** ❌ (MISSING)
- ❌ `resources/views/admin/reports/export.blade.php` - Export report (REFERENCED in routes)

### **6.6 Admin GoPay Management** ❌ (MISSING)
- ❌ `resources/views/admin/gopay/wallets.blade.php` - Wallet management
- ❌ `resources/views/admin/gopay/transactions.blade.php` - Transaction monitoring
- ❌ `resources/views/admin/gopay/withdrawals.blade.php` - Withdrawal requests
- ❌ `resources/views/admin/gopay/fx-rates.blade.php` - FX rate management

### **6.7 Admin Guest Orders** ❌ (MISSING)
- ❌ `resources/views/admin/guest-orders/index.blade.php` - Guest orders listing
- ❌ `resources/views/admin/guest-orders/show.blade.php` - Guest order details
- ❌ `resources/views/admin/guest-orders/assign.blade.php` - Assign provider to guest order

---

## 🔴 **7. AUTHENTICATION VIEWS** (Partial Missing)

### **7.1 Merchant Authentication** ❌ (MISSING)
- ❌ `resources/views/merchant/auth/login.blade.php` - Merchant login
- ❌ `resources/views/merchant/auth/register.blade.php` - Merchant registration
- ❌ `resources/views/merchant/auth/forgot-password.blade.php` - Merchant password reset

### **7.2 Cleaner Authentication** ❌ (MISSING)
- ❌ `resources/views/cleaner/auth/login.blade.php` - Cleaner login (if separate)
- ❌ `resources/views/cleaner/auth/register.blade.php` - Cleaner registration (if separate)

---

## 🔴 **8. EMAIL TEMPLATES** (Partial Missing)

### **8.1 Merchant Emails** ❌ (MISSING)
- ❌ `resources/views/emails/merchant/welcome.blade.php` - Merchant welcome email
- ❌ `resources/views/emails/merchant/kyc-approved.blade.php` - KYC approval email
- ❌ `resources/views/emails/merchant/kyc-rejected.blade.php` - KYC rejection email
- ❌ `resources/views/emails/merchant/sale-notification.blade.php` - New sale notification
- ❌ `resources/views/emails/merchant/low-stock.blade.php` - Low stock alert
- ❌ `resources/views/emails/merchant/withdrawal-processed.blade.php` - Withdrawal processed

### **8.2 Guest Emails** ❌ (MISSING)
- ❌ `resources/views/emails/guest/order-confirmation.blade.php` - Guest order confirmation
- ❌ `resources/views/emails/guest/order-assigned.blade.php` - Guest order assigned
- ❌ `resources/views/emails/guest/order-completed.blade.php` - Guest order completed

### **8.3 Cleaner Emails** ❌ (MISSING)
- ❌ `resources/views/emails/cleaner/job-assigned.blade.php` - Job assigned to cleaner
- ❌ `resources/views/emails/cleaner/earnings-credited.blade.php` - Earnings credited

---

## 🔴 **9. COMPONENTS & PARTIALS** (Partial Missing)

### **9.1 Merchant Components** ❌ (MISSING)
- ❌ `resources/views/components/merchant/product-card.blade.php` - Product card component
- ❌ `resources/views/components/merchant/rfid-scanner.blade.php` - RFID scanner component
- ❌ `resources/views/components/merchant/qr-generator.blade.php` - QR code generator component
- ❌ `resources/views/components/merchant/stock-alert.blade.php` - Stock alert component

### **9.2 User Components** ❌ (MISSING)
- ❌ `resources/views/components/user/wallet-balance.blade.php` - Wallet balance component
- ❌ `resources/views/components/user/product-scanner.blade.php` - Product scanner component
- ❌ `resources/views/components/user/checkout-summary.blade.php` - Checkout summary component

### **9.3 Guest Components** ❌ (MISSING)
- ❌ `resources/views/components/guest/booking-form.blade.php` - Guest booking form component
- ❌ `resources/views/components/guest/tracking-timeline.blade.php` - Tracking timeline component

---

## 🔴 **10. LAYOUTS** (Partial Missing)

### **10.1 Merchant Layouts** ❌ (MISSING)
- ❌ `resources/views/merchant/layouts/app.blade.php` - Main merchant layout
- ❌ `resources/views/merchant/layouts/guest.blade.php` - Guest merchant layout (for public pages)

### **10.2 Cleaner Layouts** ✅ (EXISTS)
- ✅ `resources/views/cleaner/layouts/app.blade.php` - Cleaner layout (EXISTS)

---

## 📊 **STATISTICS**

### **Total Missing Views: ~170+**

| Category | Missing Views | Priority |
|----------|--------------|----------|
| **Merchant Platform** | ~45 views | 🔴 HIGH |
| **Cleaner Platform** | ~12 views | 🔴 HIGH |
| **Guest Booking** | ~8 views | 🔴 HIGH |
| **User Section** | ~20 views | 🟡 MEDIUM |
| **Reviews & Ratings** | ~4 views | 🟡 MEDIUM |
| **Admin Section** | ~18 views | 🟡 MEDIUM |
| **Authentication** | ~5 views | 🟡 MEDIUM |
| **Email Templates** | ~10 views | 🟢 LOW |
| **Components** | ~10 views | 🟢 LOW |
| **Layouts** | ~2 views | 🔴 HIGH |

---

## 🎯 **PRIORITY ORDER FOR IMPLEMENTATION**

### **Phase 1: Critical (MVP Launch)**
1. **Merchant Platform** - Complete merchant dashboard, products, RFID, inventory
2. **Guest Booking** - Booking forms and tracking
3. **Cleaner Platform** - KYC, jobs, commission views
4. **User Wallet & Checkout** - Wallet management and QR/RFID checkout

### **Phase 2: Important (Post-Launch)**
5. **User Order History** - Unified order history
6. **Reviews & Ratings** - Review system views
7. **Admin Merchant Management** - Merchant admin views
8. **Email Templates** - Transactional emails

### **Phase 3: Enhancement**
9. **Components** - Reusable components
10. **Additional Features** - Advanced features

---

## 📝 **NOTES**

1. **Merchant Controller**: Currently returns JSON responses only. Needs web routes and views.
2. **Guest Order Controller**: Currently API-only. Needs public web routes and views.
3. **Wallet Controller**: Currently API-only. Needs web routes and views.
4. **Product Controller**: Currently API-only. Needs web routes and views.
5. **Cleaner Controllers**: Some views exist, but many are missing (KYC, Commission, Jobs, Profile, Bank).

---

## 🔗 **RELATED FILES**

- `routes/web.php` - Main web routes
- `routes/merchant.php` - **NEEDS TO BE CREATED**
- `routes/guest.php` - **NEEDS TO BE CREATED**
- `routes/cleaner.php` - Exists, but may need updates
- `app/Http/Controllers/MerchantController.php` - API only, needs web methods
- `app/Http/Controllers/GuestOrderController.php` - API only, needs web methods
- `app/Http/Controllers/WalletController.php` - API only, needs web methods
- `app/Http/Controllers/ProductController.php` - API only, needs web methods

---

## ✅ **ACTION ITEMS**

1. ✅ Create `routes/merchant.php` with merchant web routes
2. ✅ Create `routes/guest.php` with guest booking routes
3. ✅ Add web methods to `MerchantController` for views
4. ✅ Add web methods to `GuestOrderController` for views
5. ✅ Add web methods to `WalletController` for views
6. ✅ Create all missing merchant views
7. ✅ Create all missing cleaner views
8. ✅ Create all missing guest booking views
9. ✅ Create all missing user wallet/checkout views
10. ✅ Create all missing review/rating views

---

**Last Updated**: November 2024  
**Next Review**: After Phase 1 implementation

