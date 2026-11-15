# Kith — Personal, Family & Shared Finances

<p align="center">
  <img src="docs/screenshots/kith_app_icon.png" width="140" height="140" alt="Kith Connected Wealth App Icon" style="border-radius: 28px; box-shadow: 0 10px 30px rgba(16, 185, 129, 0.35);" />
  <br/>
  <h2 align="center"><b>Kith — Universal Financial Management Platform</b></h2>
  <p align="center">
    <b>Smart Personal, Family & Shared Finance with Bank SMS Intelligence, Budget Caps, and 100% Offline Privacy</b>
  </p>
  <p align="center">
    <a href="#-platforms--release-apk"><img src="https://img.shields.io/badge/Platforms-Android%20%7C%20iOS%20%7C%20iPadOS%20%7C%20macOS%20%7C%20Web-blue?style=for-the-badge" alt="Platforms" /></a>
    <a href="#-security-privacy--vulnerability-audit"><img src="https://img.shields.io/badge/Security-Audited%20%26%20Hardened-green?style=for-the-badge" alt="Security" /></a>
    <a href="#-creator--contact"><img src="https://img.shields.io/badge/Creator-Nikhil%20Jacob%20Mathew-orange?style=for-the-badge" alt="Author" /></a>
  </p>
</p>

---

## 📖 About Kith

**Kith** is an offline-first, cross-platform financial management application designed to give individuals, families, friend groups, and office colleagues complete sovereignty over their wealth. Inspired by the classic phrase *"kith and kin"* (friends, relations, and community), Kith acknowledges that modern financial life does not exist in isolation: private personal spending, collective household budgets, and shared social adventures continuously intersect.

Whether balancing your daily budget, tracking mutual fund SIPs, splitting vacation expenses with friends, or monitoring bank SMS alerts with zero cloud exposure, Kith provides effortless visual intelligence across all your devices.

### 🌐 The Connected Nodes Design

The Kith app icon represents an interconnected **'K' glyph** constructed from luminous circular wealth nodes rendered in vibrant emerald green (`#10B981`) and electric cyan (`#38BDF8`) set against deep slate navy (`#0B1120`). 

Each geometric node represents an essential financial pillar—personal income, family household stability, and shared friend activities—joined together by dynamic digital flow lines to reflect transparent, synchronized money management.

---

## 🚀 Key Capabilities & Features

### 1. Multi-Profile Financial Ledgers & Family Sharing
* **Personal Wallet**: Private personal finances, daily expenses, salary inflows, investments, and personal savings.
* **Sharma Family Hub (Multi-Member Household Experience)**:
  * **Role**: You act as the **Father (`Father (You)`)**, joined by **Wife** (Vice Principal), **Son** (working Software Engineer), and **Daughter** (College Student).
  * **3 Working Salaries + Rental + Dividend**: Father (\$6,500), Wife (\$4,200), and Son (\$3,200) salaries, plus \$1,800 apartment rent and \$650 dividend payout (**\$16,350 total income**).
  * **Attributed Expenses with Explicit Tags**: Every household expense is attributed to its purchaser with explicit title and subcategory tags (e.g. `"Ate a Burger (added by Son)"`, `"Pizza & Wings (added by Son)"`, `"Weekend Family Restaurant Dinner (added by Father)"`, `"Supermarket Monthly Bulk Basket (added by Wife)"`, `"Artisan Breads (added by Daughter)"`).
  * **Multi-Member Savings**: Father Joint FD (\$1,500) & RD (\$400); Son Nifty 50 SIP (\$600) & Nasdaq ETF SIP (\$350); Wife Sovereign Gold Bond (\$500) & Physical Gold (\$300).
* **Goa Vacation Squad (Group Trip Experience)**:
  * Pool expenses with friends (Alex, Sam, Priya, You) for beach villa stay, watersports, Thar jeep rental, and Grand Island scuba diving, with automatic debt simplification.
* **Core Tech Team**: Office colleague sprint celebrations, team lunches, and pooled fund tracking.
* **1-Tap Dashboard Switcher**: Horizontal choice chip bar lets users jump between personal, family, and group ledgers instantly.
* **Local Multi-Profile Architecture**: Because Kith is 100% on-device and privacy-first, family members can manage shared ledgers on the same device or sign in with distinct on-device accounts. Multi-device cloud sync and live friend invites are currently **Work In Progress** and will officially launch with the upcoming Google Play Store release.

### 2. Generic Demo Mode & 100% On-Device Account Registration
* **Explore Demo Mode**: Any new user can instantly tap **"Explore Demo Mode"** on the initial launch screen to test a rich pre-loaded environment (`@demo_user`, `demo@kith.app`) with authentic cash flows, categories, reminders, and split ledgers.
* **Zero Cloud Dependency**: Kith operates entirely on your physical phone or tablet. All user accounts (`fima_accounts.json`) and financial ledgers (`fima_local_db.json`) are stored safely in on-device storage. No external cloud databases, servers, or internet connections are required.
* **Sign Out & Create Private Accounts**: Users can sign out of the demo environment at any time to register their private on-device account using their email, username, and password, persisting strictly on their physical device.

### 3. 5-Day GitHub Preview Evaluation Policy
* **100% Full Access for 5 Days**: To allow thorough community review on GitHub, every single feature—including unlimited custom categories, unlimited keyword triggers, natural language processing, visual analytics, and group split ledgers—is **completely unlocked without restrictions for 5 days** from installation.
* **In-App Purchases as Work In Progress**: Official in-app billing is currently marked as **Work In Progress** and will be powered by Google Play Store Billing upon official release.
* **Evaluation Conclusion Modal**: After the 5-day evaluation period concludes, a polite pop-up informs the user that the GitHub review period has ended, guiding them to continue with standard Free tier limits, reset the evaluation period in Settings, or contact the creator.

### 4. 100% On-Device Natural Language & Voice Agent
* Type or speak conversational sentences:
  * *"Went to a restaurant 65"* ➔ Categorized automatically into **Food & Dining Out** (Expense, \$65.00).
  * *"Bought tomatoes and vegetables 15"* ➔ Categorized automatically into **Groceries** (Expense, \$15.00).
  * *"Monthly SIP in Nifty 50 250"* ➔ Categorized into **SIP Mutual Funds** (Savings, \$250.00).
  * *"HDFC FD deposit 1000"* ➔ Categorized into **Fixed Deposit** (Savings, \$1000.00).
  * *"October salary credited 5200"* ➔ Categorized into **Salary** (Income, \$5200.00).
* **Zero Internet Required**: Powered by `VocabularyService`, written strictly in pure on-device Dart with regex scoring and whole-word boundary matching (`\b`). Zero external cloud LLM dependencies, sub-millisecond response time, and 100% private.

### 5. Expense Budget Limits (Spent in Red vs. Remaining in Category Color) & Interactive Pie Slabs
* Set monthly spend caps per Expense category (e.g. \$10,000 for Dining Out, \$40,000 for Rent).
* Apply caps as a **Monthly Template** (applies across all months) or as a **Per-Month Override** (specific to a selected month).
* **Clear Color Psychology**: Spent amounts are rendered in **Red**, while the remaining unspent limit is rendered in the category's distinct **Non-Red** color (Yellow for Dining, Blue for Utilities, Teal for Custom).
* Toggle instantly between **Stacked Bar Chart** and **Segmented Donut Pie Chart**.
* **Interactive Pie Slabs & Direct Arc Percentages**: In Pie mode, each category arc displays its percentage share directly on the arc, accompanied by dedicated slab cards showing Category Name, % of Budget, Red Spent, Non-Red Remaining, and Limit.
* **Category Drill-Down & Spends Filter**: Tapping any category (e.g. *Food & Dining Out*) in Bar or Pie mode immediately filters the ledger below to list only spends in that specific category, featuring a cyan filter banner with a 1-tap `[Show All ✕]` button.

### 6. Cash-Flow Analytics & 4-Box Stat Grid (Outflow Donut Pie)
* High-level cash-flow donut pie charts across **Daily** (Day vs. MTD toggle), **Weekly** (with tap-to-focus week), **Monthly**, and **Yearly** views in the Summaries tab.
* **Strict Outflows Pie Architecture**: The donut pie chart represents allocated outflows strictly (**Expense** in Red and **Savings** in Blue). The center of the donut shows total allocated funds (`Spent & Saved`).
* **4-Box Side Stat Grid**: Alongside the pie chart, 4 compact stat cards display key metrics:
  1. 🟩 **Income**: Total income received.
  2. 🟥 **Expense**: Total expenses and percentage of outflows.
  3. 🟦 **Savings**: Total savings/investments and percentage of outflows.
  4. 🟩 **Remaining Balance**: Net remaining income surplus after expenses and savings.
* **Top Ledger / Role Switcher in Summaries**: Switch instantly between Personal Wallet, Sharma Family Hub, Goa Vacation Squad, Varanasi Pilgrimage, College Tech Tour, or Core Tech Team right from the top of the Summaries page.
* **Family Wallet Subset Architecture & Automatic Roll-Up**:
  * **Personal Wallet as Subset**: Any expense or savings logged in Personal Wallet automatically updates and rolls up into the Sharma Family Hub.
  * **Group Trips Roll-Up**: Any trip expense paid by family members (Father in *Goa Vacation Squad*, Mother/Wife in *Varanasi Pilgrimage*, Son in *College Tech Tour*) automatically rolls up into the family hub because these expenses go out of family income.
  * **Traceable Provenance**: Every rolled-up transaction displays an explicit provenance badge: e.g. `🔗 added by Father (You) in Goa Vacation Squad`, `🔗 added by Wife in Varanasi Pilgrimage`, `🔗 added by Son in College Tech Tour`, `🔗 added by Father (You) in Personal Wallet`.
* **Household & Contributor Breakdown Card**:
  * **Income by Member & Sources**: Shows each contributor's earnings, percentage share, and source pills (Salary, Rent, Dividends).
  * **Expenses by Member & Per-Category Split**: Total spent per person + detailed split within each category (e.g. In Food & Dining: Father \$233.00, Son \$60.50; In Groceries: Wife \$280.00, Father \$115.00, Son \$54.00, Daughter \$32.00).
  * **Savings & Investments by Member**: Shows individual contributions to FDs, RDs, Index SIPs, and Gold.

### 7. Interactive Recurring Reminders
* Top Dashboard banner shows active upcoming and missed reminders (e.g. Credit Card Bill, Broadband Bill, SIP installments).
* Tap the banner to open the **Reminders Sheet**; tapping the completion checkbox settles the payment, marks the bill complete, and removes it from the pending banner.

### 8. Automated Crash Telemetry via Email
* Hooks `FlutterError.onError` and `PlatformDispatcher.instance.onError` to intercept uncaught exceptions.
* Automatically serializes diagnostic logs to on-device storage.
* Upon next application restart or resume, automatically prepares and dispatches diagnostic telemetry to `crashes@kith.app` without disrupting the user experience.
* Includes an interactive **"Simulate Crash & Auto-Send"** button in Settings.

### 9. Bank SMS Reading, Transfer Deduplication & Trigger Keyword Self-Learning
* **Automatic Bank SMS Parsing & Classification**:
  * Kith reads incoming bank SMS messages on user's phone to detect financial transactions without manual typing.
  * Detects transaction types: **Credit** (Salary & Earnings), **Debit** (Expenses), and **Self-Transfers** (Savings).
  * Pre-mapped smart directory:
    * `"Credited $1000 from Synaptics"` ➔ Categorized automatically under **Salary & Earnings** (Income).
    * `"Spent $100 at KFC"` ➔ Categorized automatically under **Food & Dining Out** (Expense).
    * `"Spent $50 at Decathlon"` ➔ Categorized automatically under **Entertainment & Sports** (Expense).
    * `"$50 for BookMyShow"` ➔ Categorized automatically under **Entertainment & Sports** (Expense).
    * `"$50 for RedBus"` ➔ Categorized automatically under **Commute & Travel** (Expense).
* **Dual-SMS Self-Transfer Correlation & Deduplication into Savings**:
  * Solves the dual-message problem when transferring money between own accounts (e.g. from HDFC to SBI).
  * Automatically cross-correlates debit from Bank 1 and credit to Bank 2 with matching amount and timestamp.
  * **Zero Duplicate Income**: Suppresses the credit SMS to eliminate false income inflation.
  * **Recorded as Savings**: Records only the debit, categorized directly as **Savings** (`Inter-Account Savings`, `TransactionType.savings`) rather than an expense.
* **Full User Editability & Self-Learning Trigger Keywords**:
  * Every transaction (especially parsed SMS or unknown spends) is 100% editable (Title, Amount, Type, Category, Date, Notes).
  * **Trigger Keyword Self-Learning Loop**: Checkbox `Teach Kith this trigger keyword` automatically saves the merchant keyword into `Category.keywords` in `FinanceService`.
  * Future transactions or SMS messages matching this keyword automatically route to the user's learned category!
* **First-Run / On-Install Previous Month SMS Scan Prompt**:
  * Automatically prompts the user on first install/launch: *"Analyze Previous Month SMS Spends?"*.
  * Scans and correlates October 2026 SMS messages, displaying a detailed breakdown review sheet with Income, Spends, Savings, and Unknown Spends.
  * Tap `Import Transactions` to batch import into your wallet with automatic deduplication.
* **Aggregator Unknown Spends Flagging (Razorpay, PayU, PhonePe)**:
  * Aggregator payments where the end merchant is unstated (e.g. `"Spent $10 in Razorpay"`) are flagged as `Unknown Spend`, titled explicitly e.g. `"$10 spent to Razorpay (Unknown Spend)"`, and highlighted with an orange border and badge guiding the user to easily review and teach the app the correct category.
* **On-Demand SMS Hub (`Bank SMS Scanner`)**:
  * Dedicated SMS action button on the Dashboard next to `Recurring Bill`.
  * Test any custom bank message in real time with 1-tap live preview and `+ Add to Wallet`!

### 10. Beta Tester Feedback Widget & Session Diagnostics Telemetry
* **Top Dashboard Helper Banner**: Prominent, elegant banner located right at the top of the Ledger during preview testing (`🧪 Tester Mode • Share Feedback`), making it effortless for testers to tap anywhere and submit observations.
* **`FeedbackService` Integration**: Captures feedback ratings (1 to 5 stars), category chips (Feature Idea, Bug / Issue, UI / Design Critique, General Feedback), and multi-line commentary.
* **Automatic Diagnostic Telemetry Snapshot**: Includes an expandable preview and toggle to attach device model, OS version, storage mode, and background crash history directly to the submission.
* **Direct Email Dispatch**: Feedback is formatted and routed directly to **`nikhiljacob77@gmail.com`** via interactive bottom sheet (`TesterFeedbackSheet`) and persisted to on-device storage (`kith_tester_feedbacks.json`).
* **Permanent Settings Entry Point**: A dedicated `TESTER FEEDBACK & SUGGESTIONS` card lives permanently in Account & Settings (`SubscriptionSettingsView`), ensuring that when the temporary top banner is removed for production App Store release, users and testers always retain a direct channel to provide feedback.

### 11. Group Expense Duplicate Detection, Mutual Notification & Interactive Resolution
* **Automatic Duplicate Detection Across Members**: In shared group ledgers (e.g. *Goa Vacation Squad*, *Sharma Family Hub*), when two members log an identical or similar expense within 72 hours, Kith automatically detects and flags both items.
* **Fuzzy Semantic Matcher**: Strips conversational prefixes ("had", "ordered", "bought", "for") and analyzes word stems and amounts (e.g. Alex's `"Ordered barbecue at beach shack" $1,000` vs. Sam's `"Had barbecue grill dinner" $1,000`).
* **Mutual Group Notifications**: Dispatches an explicit warning notification to both members: *"⚠️ Possible Duplicate Expense Flagged: Both Alex and Sam logged a $1,000.00 expense. Please review and confirm."*
* **Side-by-Side Resolution Sheet (`DuplicateResolutionDialog`)**: Compare both entries side-by-side with clear metadata (Who paid, date, notes). 1-tap options to:
  * `Remove Duplicate`: Permanently removes the redundant entry and marks the remaining entry as resolved.
  * `Keep Both (Not Duplicate)`: Confirms both were genuine independent expenses and dismisses the alert.

### 12. Group Edit History Tracking, `[H]` Badge & Notification Broadcast
* **Full Revision History**: Whenever any group member edits a transaction (amount, title, category, or notes), Kith captures a timestamped `TransactionEditRecord` diff (who edited it, old vs. new values).
* **`[H] History` Badge**: Spend cards with edit revisions display an explicit purple/indigo **`[H]`** badge. Tapping it opens the `TransactionHistoryDialog` showing a complete chronological audit trail with struck-through old values and highlighted new values.
* **Group Broadcast Notification**: Editing a group expense automatically dispatches a group notification to all members (e.g. *"✏️ Expense Edited: Alex edited 'Scuba Diving & Island Boat Trip at Grand Island': Amount updated from $280.00 to $320.00"*).

### 13. Bespoke Human-Crafted Aesthetic (De-AI Theme Overhaul)
* **Moving Beyond Generic AI Templates**: Replaced stereotypical "AI developer archetypes" with a soothing, editorial, human-crafted design palette (`AppTheme`):
  * **Canvas**: Deep warm obsidian (`#0D1117`) that minimizes eye fatigue.
  * **Surfaces**: Warm charcoal graphite (`#161B22` & `#1C222D`) with subtle tactile borders (`0xFF262D3D`).
  * **Accents**: Mineral sage & mint (`#14B8A6` / `#2DD4BF`), botanical emerald (`#10B981`), terracotta rose (`#F43F5E`), and soft lapis periwinkle (`#6366F1`).
* **Calm Information Architecture**: Clean typographic hierarchy, generous breathing room, and soft tactile rounded cards (16–20px radius).

### 14. Global World Currencies Directory & Multi-Currency Engine
* **Exhaustive 65+ ISO 4217 Currencies**: Supports all major world currencies out of the box, including USD (`$`), EUR (`€`), GBP (`£`), INR (`₹`), JPY (`¥`), CAD (`C$`), AUD (`A$`), CHF (`Fr`), CNY (`¥`), SGD (`S$`), AED (`د.إ`), SAR (`﷼`), KWD (`KD`), BRL (`R$`), ZAR (`R`), and dozens more.
* **Searchable Currency Bottom Sheet**: Seamless search by ISO code, symbol, country name, or flag emoji in Settings (`SubscriptionSettingsView`).
* **Dynamic Currency & Decimal Formatting**: All financial balances, charts, category budgets, ledger cards, and export spreadsheets format dynamically with the user's chosen currency symbol and native decimal precision (e.g. 0 decimals for JPY/KRW, 2 decimals for USD/EUR/INR, 3 decimals for KWD/BHD).
* **Persistent Preference**: Stored encrypted in `finsync_storage_settings.json` and restored on startup.

### 15. Universal Floating "Feedback" Widget & Consolidated Profile Switcher
* **Floating Across All Screens**: A persistent, elegant pill floating button labeled simply **"Feedback"** floats smoothly across all screens (Ledger, Summaries, Groups, Categories, Plans).
* **Consolidated Ledger Dropdown**: Eliminated duplicate horizontal choice chip bars from the Ledger dashboard. Switching between Personal Wallet, Sharma Family Hub, Goa Vacation Squad, Varanasi Pilgrimage, College Tech Tour, and Core Tech Team is managed cleanly from the top header dropdown with active indicators and balance previews.
* **"Add an Entry" Dynamic Logger**: Updated Smart Natural Language & Voice Logger trigger from "Add an Expense" to **"Add an Entry"**. Dynamically classifies input into **Income**, **Expense**, or **Savings** based on conversational input without forcing Expense by default.

### 16. On-Device Encryption at Rest (Encrypted Vault Storage)
* **Ciphertext Armor**: All persistent files (`finsync_local_db.json`, `fima_accounts.json`, `kith_tester_feedbacks.json`, `finsync_storage_settings.json`) are encrypted using an application-internal key via `EncryptionService`.
* **Zero Plaintext on Disk**: If an external file manager, backup utility, or unauthorized user opens raw JSON files on physical storage, they see only scrambled ciphertext junk (`__kith_secure_vault__`). Sensitive salary amounts, family transaction descriptions, and usernames are completely unreadable.
* **Non-Deterministic Multi-Round Salts**: Each write generates an 8-byte cryptographic random salt to ensure identical data yields unique ciphertexts, defeating rainbow table and replay attacks.

### 17. Excel Spreadsheet (.csv) Export & Email Dispatch
* **Top Summaries Export Button**: Prominent action button in the Summaries AppBar (`Icons.table_chart_rounded`) opens the Export Configuration Sheet.
* **Flexible Accounting Periods**: Export Daily (Selected Day), Weekly (Selected Week), Monthly (Selected Month), Yearly (Full Year), or All-Time.
* **4-Section Professional Dossier**:
  1. *Executive Financial Summary*: Total Inflows, Total Outflows, Investments/Savings, Net Liquid Reserve, and Savings Rate %.
  2. *Contributor & Member Split*: Income, Spends, and Savings grouped by contributor.
  3. *Category Budget Limits & Actuals*: Budget caps, actual spent, and status (HEALTHY / OVER BUDGET).
  4. *Detailed Itemized Ledger*: Full RFC-4180 CSV with IDs, timestamps, categories, payment methods, and notes.
* **Automatic Device Save & Clipboard Ready**: Saved directly to device storage (`kith_summary_<period>_<timestamp>.csv`) and copied to the system clipboard for 1-tap pasting into Microsoft Excel, Google Sheets, or Apple Numbers.

---

## 📱 Screenshots Gallery

<p align="center">
  <img src="docs/screenshots/kith_v93_inr_ledger.png" width="30%" alt="Kith Ledger with INR Currency & Floating Feedback" />
  &nbsp;&nbsp;
  <img src="docs/screenshots/kith_v93_entry_sheet.png" width="30%" alt="Add an Entry Smart Dynamic Logger" />
  &nbsp;&nbsp;
  <img src="docs/screenshots/kith_v93_currency_sheet.png" width="30%" alt="World Currencies Directory" />
</p>
<p align="center">
  <i>(Left) Main Ledger formatted in Indian Rupee (₹) with Consolidated Dropdown & Floating Feedback; (Center) Smart Voice & NLP "Add an Entry" Dynamic Logger; (Right) Searchable World Currencies Directory (65+ ISO Currencies).</i>
</p>

<p align="center">
  <img src="docs/screenshots/kith_v93_summaries.png" width="30%" alt="Summaries Outflow Pie & Top Export Button" />
  &nbsp;&nbsp;
  <img src="docs/screenshots/kith_v93_export_sheet_opened.png" width="30%" alt="Excel Export Configuration Sheet" />
  &nbsp;&nbsp;
  <img src="docs/screenshots/kith_v93_export_success.png" width="30%" alt="Excel Spreadsheet Generated & Saved" />
</p>
<p align="center">
  <i>(Left) Financial Summaries with Outflows Donut Pie & Top Excel Export Action; (Center) Excel Spreadsheet Export Configuration Sheet; (Right) Spreadsheet Generated (.csv) & Saved to Device Flash Storage.</i>
</p>

---

## 🛡️ Security, Privacy & Vulnerability Audit

Financial data demands defensive engineering. Kith has been hardened against common database, injection, privacy, and numerical vulnerabilities, backed by an automated security test suite (`test/security_vulnerability_test.dart`):

| Vulnerability Vector | Threat Scenario | Kith Defensive Countermeasure | Test Status |
| :--- | :--- | :--- | :---: |
| **Directory Traversal** | Passing relative paths like `../../etc/passwd` to file operations | File names are sanitized with regex stripping path separators (`/`, `\`) and `..` sequences, strictly confining files inside the application sandbox. | **PASSED** |
| **Database Corruption** | Incomplete writes or corrupted non-JSON payloads in local DB | `loadLocalDatabase()` validates content boundaries and safely catches `FormatException`, returning `null` without crashing the UI. | **PASSED** |
| **PHP / Script Injection** | Injecting `<?php system(...) ?>`, SQL injection, or `<script>` tags | Stored purely as inert text scalars in Dart memory and JSON, escaping quotes during serialization. The Flutter engine does not execute HTML/PHP scripts. | **PASSED** |
| **Offline Privacy Leak** | Transmitting financial transactions or metadata while offline | In `StorageMode.offlineOnly`, all network calls are disabled, and guest accounts (`@offline_user`) cannot access remote cloud credentials. | **PASSED** |
| **Diagnostic PII Exposure** | Passwords, tokens, or credit cards leaking in crash reports | `CrashReportingService.sanitizeDiagnosticText()` uses regex pattern redactors to mask passwords, bearer tokens, and 16-digit card numbers before writing to disk or email. | **PASSED** |
| **ReDoS & Buffer Overflows** | 50,000+ character strings fed to the natural language logger | Input is defensively truncated to a 500-character head/tail window and stripped of control bytes, executing in < 5ms without memory bloat. | **PASSED** |
| **Numeric Manipulation** | Negative amounts (`-$500`), `NaN`, or `Infinity` in transaction input | Amounts are clamped to finite positive values and normalized strictly to 2 decimal places (`toStringAsFixed(2)`), preventing balance tampering. | **PASSED** |
| **5-Day Evaluation & Privilege Escalation** | Free users exceeding 5-category or 5-keyword caps or group locks after trial | Verified 5-day preview unlocks all features for 5 days. After day 5, caps and group locks are strictly enforced at the domain layer. | **PASSED** |
| **On-Device Data Encryption at Rest** | External file managers, backup tools or snooping snooping raw DB files | Encrypted via `EncryptionService` with application-internal key and 8-byte dynamic salt. Raw files on disk contain only ciphertext junk. | **PASSED** |

---

## 📦 Platforms & Release APK

### Pre-Built Android Release APK
A production release-mode APK signed with release keys is ready for direct installation on Android devices:

* **File Location**: `build/app/outputs/flutter-apk/app-release.apk`
* **Absolute Path**: `/Users/nikhiljacobmathew/Documents/development_area/finsync/build/app/outputs/flutter-apk/app-release.apk`
* **File Size**: ~60.2 MB (Fully optimized AOT machine code)
* **Minimum Android Version**: Android 7.0 (API 24, Nougat) or higher
* **Target Android Version**: Android 15 (API 35)
* **Hardware Support**: Phones (e.g. Pixel 9 Pro XL), Tablets, Foldables, Large Displays, and Smart Screens.

### Installing the Release APK via ADB
```bash
adb install -r build/app/outputs/flutter-apk/app-release.apk
```

---

## 🛠️ Building & Running from Source

### Prerequisites
* Flutter SDK (3.13.7 or newer)
* Dart SDK (3.0.0 or newer)
* Android SDK (API 35) or Xcode 16+ (for iOS/macOS)

### 1. Clone & Setup
```bash
git clone https://github.com/nikhiljacob77/kith.git
cd kith
flutter pub get
```

### 2. Run Quality Assurance Tests
```bash
# Run all unit, widget, stress, security, feedback, duplicate and history tests (53/53 tests)
flutter test

# Run the SMS intelligence and deduplication test suite specifically
flutter test test/sms_parsing_test.dart

# Run the security and vulnerability test suite specifically
flutter test test/security_vulnerability_test.dart

# Check for zero code analysis warnings
flutter analyze
```

### 3. Launch on Target Device
```bash
# Run on connected Android device (e.g. Pixel 9 Pro XL)
flutter run -d <device_id>

# Run on iOS Simulator (iPhone 17)
flutter run -d 780C6C9F-E1BA-42D4-BAE9-A42D3EF1D209

# Run on iPadOS Simulator (iPad Pro 13-inch)
flutter run -d 6B96802A-CF77-49F1-A10C-1C600BFC8B40

# Run on macOS Native Desktop
flutter run -d macos

# Run on Chrome / Web
flutter run -d chrome
```

---

## 🤝 Creator & Contact

Kith was conceptualized, architected, and engineered by **Nikhil Jacob Mathew**.

* **Author**: Nikhil Jacob Mathew
* **Email**: [`nikhiljacob77@gmail.com`](mailto:nikhiljacob77@gmail.com)
* **Feedback & Suggestions**: If you have feature requests, suggestions for custom currency modules, security improvements, or questions regarding group finance management, please reach out via email.
* **Bug Reports**: Please open an issue on the GitHub repository with reproduction steps and diagnostic logs.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
