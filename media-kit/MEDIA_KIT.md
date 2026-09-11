# Media Kit: Meter Record (میٹر ریکارڈ)

> **The Smart Household Electricity Command Center for Multi-Meter Homes in Pakistan.**  
> Monitor independent connections, protect your $\le 200$ kWh lifeline slab, track consolidated bills, and prevent late surcharges.

---

## ⚡ Executive Summary & Fact Sheet

| Field | Details |
| :--- | :--- |
| **App Name** | **Meter Record** (میٹر ریکارڈ) |
| **Tagline** | Master Your Household Electricity • Keep Protected, Never Overpay |
| **Developer** | Hassan (Okara, Pakistan) |
| **Category** | Utilities / Personal Finance / Smart Living |
| **Platform** | Native Android (Jetpack Compose, Material 3, Room SQLite, Coroutines/Flow) |
| **Minimum OS** | Android 8.0 (API level 26) |
| **Target OS** | Android 15 (API level 35) |
| **Current Version**| Version 2.1 (Build 17 • Room Schema v4) |
| **Pricing** | 100% Free & Open • No Ads • No Trackers • Zero In-App Purchases |
| **Privacy & Storage** | **100% Offline & Private** (All data stays locally on device; optional Google Sign-in / local JSON backup) |
| **Languages** | English & Urdu (اردو — Full RTL layout) |
| **Supported DISCOs** | LESCO, K-Electric, IESCO, FESCO, GEPCO, MEPCO, PESCO, HESCO, SEPCO, QESCO |

---

## 🎨 Official Promo Banner

![Meter Record Promo Banner](/promo_feature_graphic_1789118970686.jpg)

---

## 🔍 The Story: Solving Pakistan’s Multi-Meter Reality

### The Economic Context
In Pakistan, electricity tariffs set by NEPRA operate on steep, non-linear progressive slabs. For domestic consumers, staying at or below **200 kWh/month** grants **"Protected" status** with heavily subsidized lifeline rates (typically Rs 14–20/unit). 

However, crossing just **1 unit** past 200 units (e.g., 201 kWh):
1. Immediately bumps the consumer into the **Unprotected** tariff slab.
2. Increases the base tariff and fuel price adjustments (FPA) drastically (often jumping from Rs 20/unit to Rs 45–60+/unit).
3. **Disqualifies the household from Protected status for the subsequent 6 consecutive months**, costing tens of thousands of extra rupees over the year.

### The Multi-Meter Home Setup
To manage this reality legally, many Pakistani homes install **multiple independent single-phase meters** (e.g., 4 physical meters mounted on a shared board: *Main House*, *Garage*, *Studio*, and *Basement*), each with its own 14-digit LESCO reference number and separate billing cycle.

### The Daily Friction
* **No Unified Overview**: Bills arrive at different times; meter readings are scattered on disparate slips or paper bills.
* **Blind Slab Jumps**: Without mid-month pacing alerts, a single air conditioner or appliance on one meter can silently breach the 200 kWh threshold.
* **Bill Juggling & Late Surcharges**: Tracking 4 different due dates and remembering which bank app paid which bill leads to avoidable late-payment surcharges.
* **Clunky Utility Apps**: Official distribution company apps are often slow, ad-ridden, online-dependent, or fail to support multi-meter consolidated households.

**Meter Record** was built to solve this exact problem cleanly, privately, and beautifully.

---

## 🚀 Core Features Matrix

### 1. 🏠 Multi-Meter Command Center
* Monitor up to 4+ physical, independent meters side-by-side.
* Real-time billing cycle tracking showing days elapsed, units consumed, and projected finish.
* Dynamic usage-tier visualization: Safe Green ($\le 150$), Caution Amber ($150–175$), Warning Orange ($175–199$), and Danger Red ($\ge 200$).

### 2. 🛡️ $\le 200$ kWh Protected Slab Watchdog
* Daily pace projection calculated from reading intervals: `On pace to finish this cycle at ~190 kWh`.
* Instant banner warnings when any connection crosses warning thresholds (150 or 175 kWh), giving users time to balance loads before the billing cycle closes.

### 3. 🧾 Consolidated Household Monthly Bills & Due-Date Tracker
* **Household Overview**: Aggregates total household electricity expenditure (e.g. `Rs 10,640 across 4 meters`) and combined units (`522 kWh`).
* **Effective Rate Calculation**: Shows real effective household cost per kWh (`Rs 20.38/unit`) derived directly from actual bills.
* **Urgent Due-Date Banner**: Prominently alerts on Home before bills are due (`⚠️ Main House bill is due 18 Jul — avoid late surcharge!`).
* **1-Tap Fast Batch Entry (`+ Record Month Bills`)**: Enter units and rupee amounts for all 4 meters in a single dialog in under 30 seconds, with live auto-calculating totals.
* **1-Tap Reference Number Copy**: One tap copies the clean 14-digit reference number directly to the clipboard, ready to paste into Meezan Mobile, Nayapay, SadaPay, or Easypaisa.
* **Payment Status Tracking**: 1-tap "Mark Paid / Unpaid" toggle with payment method notes (`Paid via Nayapay`).

### 4. 🇵🇰 Complete Bilingual Parity (English & Urdu RTL)
* Seamlessly switch between English and natural Urdu (`اردو`).
* Native Right-to-Left (RTL) layout with localized typography and intuitive phrasing (`گھریلو بجلی کے بل`, `ادا شدہ نشان لگائیں`).

### 5. 🔒 100% Offline, Private & Ad-Free
* Zero third-party trackers, analytics, or advertisements.
* All data stored in a local encrypted SQLite database via Android Jetpack Room.
* Comprehensive JSON backup & restore + one-tap CSV and PDF report export.
* Optional biometric app lock (fingerprint / PIN) for privacy.

### 6. 📱 Interactive Home Screen Widgets & Shortcuts
* Android Glance home screen widget displaying live per-meter usage and tier status without needing to open the app.
* Quick-add shortcuts to log readings instantly.

---

## 🎨 Brand Guidelines & Visual Design System

### 1. Logo & Iconography
* **Icon Description**: A minimalist house silhouette rendered in electric lime stroke (`#C7F24B`) framing a dynamic, multi-stage rainbow gradient lightning bolt (`#FF3B30` → `#FF9500` → `#FFCC00` → `#34C759` → `#007AFF` → `#AF52DE`) against a warm dark charcoal tile (`#131210`).
* **Symbolism**: The house represents the household; the lime frame represents safety and protected boundaries; the rainbow lightning bolt symbolizes dynamic, balanced electrical energy across diverse loads.

### 2. Color Palette

#### Dark Theme (Default)
| Color Name | Hex Code | RGB | Role / Usage |
| :--- | :--- | :--- | :--- |
| **Dark Background** | `#131210` | `19, 18, 16` | Main app background (warm dark charcoal) |
| **Card Surface** | `#1B1915` | `27, 25, 21` | Elevated container cards & dialog surfaces |
| **Card Border** | `#2A2721` | `42, 39, 33` | Subtle structural division |
| **Electric Lime (Accent)**| `#C7F24B` | `199, 242, 75` | Primary CTA, active selections, hero highlights |
| **Accent Ink** | `#1A1206` | `26, 18, 6` | High-contrast text on accent surfaces |
| **Text Primary** | `#EFE9E1` | `239, 233, 225`| High-legibility warm ivory headlines and values |
| **Text Muted** | `#9A9184` | `154, 145, 132`| Secondary labels, subtitles, helper text |

#### Light Theme
| Color Name | Hex Code | RGB | Role / Usage |
| :--- | :--- | :--- | :--- |
| **Light Background** | `#F7F5F1` | `247, 245, 241`| Clean, paper-warm daylight background |
| **Card Surface** | `#FFFFFF` | `255, 255, 255`| Crisp elevated card containers |
| **Border** | `#ECE8E0` | `236, 232, 224`| Soft outline for tactile card separation |
| **Teal (Accent)** | `#1F6F6B` | `31, 111, 107` | Grounded, high-contrast daylight accent |
| **Text Primary** | `#2B2B2B` | `43, 43, 43` | Charcoal text |

#### Usage Tier Status Indicators
* **Safe / Normal ($\le 150$ kWh)**: `#6FAE6F` (Calm Green)
* **Caution ($150–175$ kWh)**: `#E8A75A` (Amber)
* **Warning ($175–199$ kWh)**: `#E0794F` (Orange)
* **Danger ($\ge 200$ kWh)**: `#DA4B45` (Crimson Red)

### 3. Typography
* **Headline & Hero Values**: **Fraunces** (Variable Serif Display) — brings editorial authority, warmth, and financial clarity to large numbers (`Rs 10,640`, `522 kWh`).
* **Numerals, Meters & Keypad**: **Space Grotesk** (Variable Monospace-feel Sans) — crisp, technical legibility for reading dates, reference numbers, and units.
* **UI & Body**: **IBM Plex Sans** — neutral, engineered readability for labels, forms, and dialogs.

---

## 📸 Media Assets & Screenshot Showcase

````carousel
![Home Screen Dashboard](/screen_home_final.png)
<!-- slide -->
![Consolidated Household Bills Screen](/screen_household_bills_fresh.png)
<!-- slide -->
![Batch 4-Meter Bill Entry Modal](/batch_entry_all_filled.png)
<!-- slide -->
![Urdu RTL Household Bills Screen](/screen_household_bills_urdu_live.png)
<!-- slide -->
![Light Theme Household Bills Screen](/screen_household_bills_light_mode.png)
<!-- slide -->
![Settings & Customization Screen](/screen_settings.png)
````

---

## 🎙️ Developer Q&A (Interview Ready)

**Q: Why did you build Meter Record?**  
> *"In Pakistan, electricity billing isn't just about paying a bill at the end of the month; it’s an active budgeting challenge. When you cross 200 units on a domestic meter, your tariff effectively doubles and you lose protected status for half a year. Many families, including mine, run multiple meters across different floors or sections of the home to manage this legally. But existing apps only look at one meter at a time, spam you with ads, or force you into clunky online portals. I wanted an app that felt like a premium financial dashboard: fast, offline, privacy-first, and built specifically for the multi-meter reality."*

**Q: What makes the "Consolidated Household Bills" feature unique?**  
> *"When 4 paper bills arrive in your mailbox or via SMS, you have to scramble to check 4 different due dates, copy 14-digit reference numbers into your banking app, and mentally add up the total expense. Meter Record lets you record all 4 bills in 30 seconds, gives you 1-tap reference number copy buttons, alerts you before due dates so you never pay late surcharges, and shows your true combined household cost and effective rate per unit."*

**Q: Does the app require internet or send user data to the cloud?**  
> *"Not at all. Meter Record is built offline-first. Your meter readings, consumption history, and bills never leave your phone unless you explicitly choose to export a CSV, PDF report, or backup file. There are no analytics trackers, no account requirements, and zero ads."*

---

## 📬 Contact & Links

* **Developer**: Hassan (Okara, Pakistan)
* **Official User Guide**: [docs/USER_GUIDE.md](file:///c:/Users/Hassan/Projects%20Gemini/Meter%20Record/docs/USER_GUIDE.md) | [Web Guide](file:///c:/Users/Hassan/Projects%20Gemini/Meter%20Record/docs/index.html)
* **App Repository / Downloads**: Available upon release
* **Press Inquiries**: Hassan (Okara, Pakistan)
* **Media Kit Version**: 1.0 (September 2026)
