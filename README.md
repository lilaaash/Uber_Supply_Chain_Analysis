# Uber_Supply_Chain_Analysis
Analyzing service fulfillment gaps in Uber's network using Python.
# 🚕 Uber Supply Chain: Solving the 58% Fulfillment Gap

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](PASTE_YOUR_COLAB_URL_HERE)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Industry](https://img.shields.io/badge/Industry-Logistics%20%26%20Supply%20Chain-06C167)
![Status](https://img.shields.io/badge/Business_Impact-High-white)

## 📈 The Business Challenge
Uber's success depends on a perfectly balanced **Service Supply Chain**. In this analysis of **6,745 requests**, I discovered that over **half of our customers** are left unserved. This project isn't just about data—it's about recovering lost revenue by putting the right drivers in the right place at the right time.



---

## 🎯 At a Glance: The "So What?"
* **The Problem:** 58% of all ride requests fail to complete.
* **The Discovery:** We don't just have a "shortage of drivers"; we have a **geographic mismatch**.
* **The Result:** Two distinct "bottlenecks" that require different business strategies.

---

## 🛠️ The Analysis Journey

### 1. Network Health (Overall Performance)
We are currently operating at a **42% success rate**. I segmented the failures into:
* **Driver Cancellations** (The "Human" Behavioral Factor)
* **No Drivers Found** (The "Inventory" Capacity Factor)

### 2. The "When" & "Where" (Pattern Recognition)
By engineering raw timestamps into **Time Slots**, the data revealed a mirrored failure pattern:
* **The City Node:** Fails in the **Morning Rush** (Drivers cancel to avoid airport traffic).
* **The Airport Node:** Fails in the **Evening Rush** (Zero inventory when peak flights land).



---

## 🚀 Strategic Recommendations
To capture the missing 58% of revenue, I recommend:
1.  **Surge Pricing Re-calibration:** Specifically incentivize city drivers for "Airport-bound" requests during the 5 AM - 9 AM window.
2.  **Predictive Repositioning:** Move "Idle" city drivers to the Airport node 30 minutes before peak evening flight clusters (5 PM - 10 PM).

---

## 💻 Technical Skills Demonstrated
* **Data Wrangling:** Cleaned mixed date formats and handled null supply values in Python.
* **Feature Engineering:** Created custom temporal bins to identify behavioral trends.
* **Visualization:** Designed high-contrast, executive-level dashboards using `Seaborn` and `Matplotlib`.

---

## 📂 How to Explore this Project
1.  **Interactive Notebook:** View the [Full Google Colab Analysis](PASTE_YOUR_COLAB_URL_HERE).
2.  **The Data:** Cleaned dataset is available in the root folder.
3.  **The Dashboard:** Check the visual exports for the "Big Picture" view.

---
*Developed as a Supply Chain Analytics Portfolio Piece.*
