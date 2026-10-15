# SCOREIFY
# 🏏 GULLY Cricket Scoreboard — Pro Match & Super Over Edition

> **⚡ Zero-Install Digital Cricket Scorer for Local Tournaments, Club Matches & Ground Organizers**
>
> Built with **HTML5**, **CSS3**, and **Vanilla JavaScript** — runs in any mobile or desktop browser, works 100% offline, and exports instant WhatsApp scorecards.

🚀 **Live App Link:** [**https://**](https://www.google.com/search?q=https%3A%2F%2Fvnp-naga-1201.netlify.app)[**vnp-scoreify.netlify.app**](https://vnp-scoreify.netlify.app/)

## ✨ Why Organizers & Cricketers Love It

* **📱 Built for the Ground**: High-contrast dark stadium theme (`#0b1120` & `#38bdf8`) engineered for clear readability under bright outdoor sunlight.

* **⚡ Popup-Free One-Tap Scoring**: Inline action drawers for **No-Balls**, **Wides**, **Byes/Leg-Byes**, and **Wickets**—no annoying browser popups.

* **🔥 Official Super Over Tie-Breaker**: Full ICC/T20 Super Over support with 1-over limits, 2-wicket maximums, reverse batting order, and repeat Super Overs.

* **📊 Complete Over-by-Over Ledger**: Tracks every delivery badge (`0`, `1`, `4`, `6`, `NB+4`, `FH(6)`, `WD`, `W`) with a live **Over Sum** and end-of-over score.

* **💾 Auto-Save Protection**: Powered by browser `localStorage` so accidental tab refreshes or phone screen locks never lose a single ball.

* **📲 Instant WhatsApp Scorecard**: One-tap clipboard export of the complete match summary, batting/bowling tables, and over-by-over records.

## 🎮 Core Features at a Glance

| Module | What It Tracks & Automates | 
| ----- | ----- | 
| **🏟️ Match & Chase Engine** | Custom team names, configurable max overs, 1st & 2nd innings transitions, live **CRR**, target calculation, remaining balls, and **RRR**. | 
| **🔥 Super Over Mode** | Auto-detects tied matches (`runs === target - 1`) or starts manually; enforces **1 Over (6 legal balls)**, **Max 2 Wickets**, and reverse batting order. | 
| **⚡ No-Ball & Free Hit** | Credits `1` penalty run + bat runs (`NB+1` to `NB+6`), charges total runs to bowler (`0` legal balls), and triggers **⚡ FREE HIT** (Run Out only). | 
| **🎯 Wides & Byes / LB** | Logs Wides (`WD` to `WD+4`) without advancing balls; logs Byes & Leg-Byes (`B1–B4`, `LB1–LB2`) as legal balls with `0` bat runs and `0` bowler runs. | 
| **🏏 Full Batting Card** | Archives every dismissed batter (`howOut`, runs, balls, `4s`, `6s`, Strike Rate) plus active `not out*` batters with automatic strike rotation. | 
| **🎳 Multi-Spell Bowling Card** | Remembers each bowler's cumulative `Overs`, `Runs`, `Wickets`, and `Economy` across multiple spells in the innings. | 

## 📏 Official Cricket Rules Implemented

| Delivery / Situation | Team Score | Legal Ball Count | Striker Stats | Bowler Figures | Automatic Rule Trigger | 
| ----- | ----- | ----- | ----- | ----- | ----- | 
| **Legal Runs (`0–6`)** | `+Runs` | `+1 Ball` | `+Runs`, `+1 Ball`, `4s/6s` | `+1 Ball`, `+Runs` | Rotates strike on `1`, `3`, `5` & end of over | 
| **No-Ball (`NB + Bat`)** | `+1 + Bat Runs` | `0 Balls` | `+Bat Runs`, `+1 Ball`, `4s/6s` | `0 Balls`, `+1 + Bat Runs` | Activates **⚡ Free Hit** on next ball | 
| **Free Hit (`FH`)** | `+Runs` | `+1 Ball` | `+Runs`, `+1 Ball`, `4s/6s` | `+1 Ball`, `+Runs` | Blocks Bowled/Caught/LBW/Stumped (**Run Out only**) | 
| **Wide (`WD + Extra`)** | `+1 + Extra` | `0 Balls` | `0 Runs`, `0 Balls` | `0 Balls`, `+1 + Extra` | Carries over **Free Hit** if active | 
| **Byes / Leg-Byes (`B/LB`)** | `+Bye Runs` | `+1 Ball` | `0 Runs`, `+1 Ball` | `+1 Ball`, `0 Runs` | Rotates strike on odd byes (`1`, `3`) | 
| **Super Over (`🔥 SO`)** | `Target = 1st + 1` | `Max 6 Balls (1 Ov)` | `3 Batters (Max 2 Out)` | `Max 1 Over` | 2nd wicket ends innings immediately | 

## 🚀 Quick Start (Run Locally or Online)

1. **Use Online Immediately**:

   * Open [**https://**](https://www.google.com/search?q=https%3A%2F%2Fvnp-naga-1201.netlify.app)[**vnp-scoreify.netlify.app**](https://vnp-scoreify.netlify.app/) on any phone, tablet, or laptop browser.

2. **Run Offline on Your Device**:

   * Download or clone this repository.

   * Double-click `index.html` (or `cricket_scoreboard.html`) to open it in Chrome, Safari, Edge, or Firefox—no server or internet required.

3. **Score Your Match**:

   * Tap **Settings** to set Team 1, Team 2, and Maximum Overs.

   * Tap any batter or bowler name to rename players on the fly.

   * Tap **WhatsApp Share** anytime to copy the formatted match report and paste it into your team chat group.

## 📂 Repository Structure

* `index.html` — Primary deployment entry file containing the complete HTML, CSS, and JavaScript application.

* `cricket_scoreboard.html` — Standalone copy of the application for local offline use.

* `README.md` — Project documentation, rule matrix, and live deployment link.
