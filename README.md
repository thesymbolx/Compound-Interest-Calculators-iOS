# Compound Interest Calculator (iOS)

> Mathematically rigorous compound interest calculator built with SwiftUI. 

Unlike generic calculators that use simplified annual formulas, this app aligns precisely with how actual banks calculate compound interest using **Daily Accrual** mathematics. Complete with animated graphs and parallax scrolling for a premium user experience.

[![Swift](https://img.shields.io/badge/Swift-5.9+-orange.svg)](https://swift.org)
[![iOS](https://img.shields.io/badge/iOS-16.0+-blue.svg)]()
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

---

## 📸 See it in Action

<!-- 
  PRO TIP: Remember the drag-and-drop trick from earlier! 
  Drop your GIF here and replace this comment with the generated link. 
  Try to show the parallax scrolling and animated graphs in the GIF! 
-->
![App Demo](assets/demo.gif) 

---

## ✨ Features

### Premium User Interface
* **SwiftUI Native:** Built entirely with Apple's modern UI framework.
* **Animated Graphs:** Data visualization that smoothly animates as parameters change.
* **Parallax Scrolling:** Depth-based scrolling effects for a highly polished, tactile feel.

### Banking-Standard Mathematics
Most calculators use basic `A = P(1 + r/n)^nt` formulas. This app utilizes **Banking-Standard Daily Accrual** to provide real-world accuracy.

The core calculation engine enforces the following rules:
1. **Calendar Precision:** Uses the actual number of days in the current month (e.g., exactly 31 for January, 28/29 for February).
2. **Forward-Starting:** Accrual starts on the next full month from the current date to prevent over-calculation on days that have already passed.
3. **Favorable Timing:** Regular deposits are calculated as being added at the *start* of the month, ensuring they earn full interest for that period.
4. **Daily Rate Accuracy:** Uses a true daily rate (`Annual Rate / 365`) rather than a simplified monthly division.
5. **Deferred Rounding:** Interest is accrued with floating-point precision in the background and only rounded to 2 decimal places at the exact moment of payout (Monthly or Annually).

## 🚀 Quick Start

### Prerequisites
* Xcode 15.0 or later
* iOS 16.0+ target deployment
* Swift 5.9+

### Installation

1. Clone the repository:
   ```bash
   git clone [https://github.com/thesymbolx/Compound-Interest-Calculators-iOS.git](https://github.com/thesymbolx/Compound-Interest-Calculators-iOS.git)
