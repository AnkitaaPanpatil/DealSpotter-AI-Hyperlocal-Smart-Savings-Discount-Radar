# 🏷️ DealSpotter AI — Hyperlocal Smart Savings & Discount Radar

[![License: MIT](https://img.shields.io/badge/License-MIT-emerald.svg)](https://opensource.org/licenses/MIT)
[![Technology](https://img.shields.io/badge/Stack-Single--File%20Vanilla%20JS%20%7C%20TailwindCSS%20%7C%20Leaflet-059669)](https://leafletjs.com/)
[![Geospatial Telemetry](https://img.shields.io/badge/Geolocation-Hyperlocal%20Proximity%20Radar-10b981)](#)
[![AI Engine](https://img.shields.io/badge/AI%20Copilot-Gemini%203%20Flash-f59e0b)](https://ai.google.dev/)
[![Verification Integrity](https://img.shields.io/badge/Anti--Markup-30--Day%20Price%20History%20Guard-f43f5e)](#)

> **A cutting-edge, zero-latency hyperlocal discount discovery platform and anti-markup verification terminal engineered for modern urban shoppers, bargain hunters, and community savers.**

---

## 📌 Executive Summary

Urban consumers face fragmented promotional channels, ephemeral flash sales, misleading "false discount" markups, and unorganized voucher barcodes at physical retail checkouts. Millions of dollars in legitimate local savings—such as evening bakery clearance markdowns, restaurant happy-hour specials, supermarket bogo promotions, and student/senior stackable perks—expire unredeemed every day.

**DealSpotter AI** bridges the gap between brick-and-mortar storefront inventory and digital consumer discovery. Built under a strict **Single-File Mandate** (`deal_spotter_app.html`), the platform integrates interactive geospatial proximity radar mapping, anti-markup 30-day historical price analysis, an instant contactless barcode/QR coupon wallet, crowdsourced deal validation, and a senior retail bargain strategist powered by Google Gemini.

---

## 🚨 Urban Retail Challenges & DealSpotter AI Solutions

| The Shopping Barrier | Consumer Reality | DealSpotter AI Systematic Solution |
| :--- | :--- | :--- |
| **Fragmented Local Promotions** | Great neighborhood discounts are scattered across flyers, store windows, and disparate social media channels. | **Hyperlocal Proximity Radar (Leaflet.js)**: Real-time map displaying geofenced verified discounts across dining, groceries, tech, and boutiques within an adjustable radius ($1.0\text{ km} - 5.0\text{ km}$). |
| **Artificial Pre-Sale Markups** | Stores inflate retail prices by $40\%$ before applying a $30\%$ discount sticker, creating deceptive bargains. | **True-Discount Verifier & 30-Day History (Canvas)**: Tracks rolling 30-day price trajectories to calculate price manipulation risk and confirm genuine net percentage savings. |
| **Friction at In-Store Checkout** | Shoppers scramble to find promo codes or digital voucher passes while standing in checkout lines. | **Contactless Barcode & QR Wallet**: Claimed deals generate instant scannable 1D/2D digital barcode passes for cashiers and 1-click clipboard promo code copy for delivery apps. |
| **Perishable Food Waste** | Bakeries, delis, and bistros discard surplus inventory daily after closing hours. | **Zero-Waste Flash Drop Engine**: Alerts users to steep evening markdowns ($50\% - 70\%$ off) within a critical 90-minute expiry window. |
| **Unoptimized Coupon Stacking** | Shoppers rarely know how to combine merchant coupons with loyalty hours and demographic discounts. | **DealSpotter Copilot (Gemini 3 Flash)**: On-demand AI retail strategist providing tailored advice on price matching, student/senior perks, and multi-voucher stacking. |

---

## 🌟 Core System Pillars

### 1. 🛰️ Hyperlocal Proximity Radar & Directory (Leaflet.js)
* **CartoDB Dark Matter GIS Grid**: Real-time visualization of neighborhood merchants categorized by deal severity:
  * 🟢 **Standard Deals ($\ge 20\%$)**: Regular promotional discounts across cafes and stationery stores.
  * 🟡 **Mega Drops ($40\% - 59\%$)**: High-value midday lunch specials and electronic clearances.
  * 🔴 **Flash Steals ($\ge 60\%$)**: High-urgency, short-expiry evening drops with animated pulsing radar pins.
* **Proximity Directory**: Search by keywords (`sourdough`, `sushi`, `headphones`, `organic`) with dynamic distance radius filters ($1.0\text{ km}$, $2.5\text{ km}$, $5.0\text{ km}$) and instant map panning.

### 2. 📉 True-Discount Verifier & 30-Day Price History
* **High-Resolution HTML5 Canvas Chart**:
  * Visualizes the 30-day historical price polyline against regular retail average baselines.
  * Highlights price drop callouts with color-coded confidence indicators ($99.4\%$ verified genuine bargain).
* **Price Manipulation Risk Metric**: Flags artificial price spikes preceding promotional campaigns to guarantee verified savings.
* **Price Drop Watchlist**: Allows users to configure custom target trigger alerts for high-value retail products.

### 3. 💳 Contactless Voucher Pass & Barcode Wallet
* **Dynamic 2D / QR Scanner Generator**: Generates clean, high-contrast matrix barcodes via HTML5 Canvas for seamless optical scanning by retail point-of-sale (POS) systems.
* **Voucher Telemetry**: Tracks unique voucher IDs (`#DS-NY-2026-9912`), store names, promo codes, and real-time countdown expiration timers.
* **1-Click Clipboard Integration**: Copies voucher codes for instant checkout pasting into third-party food delivery and ecommerce applications.

### 4. 🧠 DealSpotter Copilot — AI Bargain Hunter (Gemini 3 Flash)
* **Domain-Trained Generative Strategist**: Evaluates retail price elasticity, student/senior discount stacking, supermarket clearance patterns, and seasonal cycles.
* **Pre-Configured Advisory Shortcuts**:
  * 🍣 *Nearby happy hour dining and bento specials within walking distance.*
  * 🛒 *Highest percentage discounts on organic produce and grocery staples.*
  * 💡 *Advanced coupon stacking rules and student identification combinations.*
* **Offline Heuristic Resiliency**: Gracefully provides built-in retail heuristics if network access or API credentials are unavailable.

### 5. 📸 Community "Spot & Share" & Flash Drop Simulator
* **Crowdsourced Intelligence**: Enables community members to publish local in-store finds with store tags, category selections, and expiry parameters (+50 Karma points).
* **Live Flash Drop Simulation**: Instant interactive simulation demonstrating an emergency $70\%$ clearance markdown at a nearby artisan bakery.
* **Native Web Audio Synthesizer**: Custom acoustic synthesizer using the Web Audio API for claim chimes, flash alert stingers, and upvote confirmations.

---

## 📐 Mathematical Formulation: True-Discount Verification

DealSpotter AI quantifies the authenticity of a promotional markdown using the **True-Discount Confidence Index ($TCI$)**:

$$TCI = \left( 1 - \frac{\bar{P}_{14} - \bar{P}_{30}}{\bar{P}_{30}} \right) \times \left( \frac{P_{\text{retail}} - P_{\text{deal}}}{P_{\text{retail}}} \right)$$

Where:
* $P_{\text{retail}}$: Listed standard manufacturer suggested retail price (MSRP)
* $P_{\text{deal}}$: Current promotional sale price
* $\bar{P}_{14}$: Mean recorded retail price over the preceding 14 days
* $\bar{P}_{30}$: Mean recorded retail price over the preceding 30 days

### Price Manipulation Risk ($PMR$)
If a merchant inflates their price in the 14 days immediately preceding a promotional event ($\bar{P}_{14} > \bar{P}_{30}$), the system triggers an anti-markup warning:

$$PMR = \max\left(0, \; \frac{\bar{P}_{14} - \bar{P}_{30}}{\bar{P}_{30}}\right) \times 100\%$$

* **$PMR = 0\%$**: Verified authentic price reduction.
* **$PMR > 15\%$**: Flagged as artificial pre-discount inflation.

---

## 💻 Tech Stack & Architecture

DealSpotter AI strictly adheres to the **Single-File Mandate** (`deal_spotter_app.html`), requiring zero build pipelines, package managers, or server runtimes.

```
┌────────────────────────────────────────────────────────┐
│                   DealSpotter AI OS                    │
├──────────────────────────┬─────────────────────────────┤
│ User Interface           │ HTML5, TailwindCSS (CDN),   │
│                          │ Plus Jakarta Sans, Mono     │
├──────────────────────────┼─────────────────────────────┤
│ Geospatial Radar         │ Leaflet.js (v1.9.4) &       │
│                          │ CartoDB Dark Matter Tiles   │
├──────────────────────────┼─────────────────────────────┤
│ Dynamic Visualizations   │ HTML5 2D Canvas (Price Graph│
│                          │ and Contactless Barcodes)   │
├──────────────────────────┼─────────────────────────────┤
│ Audio Synthesis          │ Native Web Audio API        │
├──────────────────────────┼─────────────────────────────┤
│ Intelligence Engine      │ Google Gemini 3 Flash API   │
│                          │ with Offline Fallbacks      │
└──────────────────────────┴─────────────────────────────┘
```

---

## 🚀 Quick Start Guide

### Option 1: Direct Browser Launch
1. Download or clone `deal_spotter_app.html`.
2. Double-click the file to open it directly in Google Chrome, Mozilla Firefox, Microsoft Edge, Brave, or Safari.

### Option 2: Local HTTP Server
```bash
# Using Python 3
python -m http.server 8080

# Using Node.js npx
npx serve .
```

Open your browser and navigate to:
```
http://localhost:8080/deal_spotter_app.html
```

---

## 🔑 Activating Google Gemini AI

DealSpotter AI operates out-of-the-box with built-in heuristic bargain advice. To enable real-time generative reasoning via Google Gemini 3 Flash:

1. Open `deal_spotter_app.html` in an editor.
2. Locate the `submitAiBargainQuery` function (around line 630):
   ```javascript
   const apiKey = "YOUR_GEMINI_API_KEY_HERE";
   ```
3. Paste your free Gemini API key generated via [Google AI Studio](https://aistudio.google.com/).
4. Save the file and refresh your browser.

---

## 🛒 Smart Shopping Rules (Algorithmic Best Practices)

1. **The 6:30 PM Window**: Gourmet bakeries, sushi bars, and prepared-food delis discount fresh items by $50\% - 70\%$ after 6:30 PM to eliminate daily surplus inventory.
2. **Student & Senior Stacking**: Presenting valid academic or senior credentials at local indie cafes on designated weekdays typically yields an additional $10\%$ stack on top of promotional codes.
3. **Anti-Markup Inspection**: Always check the 30-day historical chart on high-ticket electronics before purchasing to confirm that "clearance" prices represent authentic reductions.

---

## 📜 License

This project is licensed under the **MIT License** — free for individual consumers, urban developers, local merchant associations, and research groups.
