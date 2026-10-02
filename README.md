# Project 2: Weather API → Telegram Bot

> **One-liner:** Daily Lagos weather delivered to Telegram automatically — my first API integration, foundation for all API automations.

[![OpenWeatherMap](https://img.shields.io/badge/API-OpenWeatherMap-orange)](https://openweathermap.org/api)
[![Telegram](https://img.shields.io/badge/Telegram-Bot_API-blue)](https://core.telegram.org/bots)
[![Make.com](https://img.shields.io/badge/Make.com-Automation-blue)](https://make.com)

## 🎯 Problem
Learning APIs is intimidating. Most beginners never move past Sheets → Email. This project proves API handling is simple and repeatable — critical for client work where every integration is an API.

## ✅ Solution
3-step Make.com scenario:
1. **HTTP Request** — GET `https://api.openweathermap.org/data/2.5/weather?q=Lagos&appid=YOUR_KEY&units=metric`
2. **Parse JSON** — Extract temp, feels_like, humidity, description
3. **Telegram Send Message** — Formatted weather alert to private channel/bot

## 🏗️ Architecture

```
[HTTP: Make a Request - OpenWeatherMap API]
        ↓
[Telegram: Send a Message]
Message: 🌤 Weather in Lagos — Temp: {{temp}}°C — Feels like: {{feels_like}}°C — Humidity: {{humidity}}% — Condition: {{description}}
        ↓
[Schedule: Every Day 7:00 AM]
```

## 📸 Screenshots (Add Yours)

- `scenario.png` — HTTP + Telegram modules
- `telegram-message.png` — Telegram chat showing weather message
- `api-key-page.png` — OpenWeatherMap API key page (BLUR YOUR KEY)

## 📈 Results

- **Learning Outcome:** APIs = menus. You ask, it serves JSON. Once understood, any API is automatable.
- **Build Time:** 20 minutes
- **Use Cases Unlocked:** Any API → Any destination (e-commerce orders, CRM updates, Slack alerts)
- **Reliability:** Runs daily at 7 AM, zero manual effort

## 🛠️ Tools Used

- OpenWeatherMap API (Free tier — 1,000 calls/day)
- Telegram Bot API (Free forever)
- Make.com (Free tier)
- **Running Cost:** $0/month

## 🎥 Demo Video

**YouTube Unlisted Link:** `[Paste Link Here]`

**Demo Script (30 sec):**
- 0-5s: "Weather Bot — API → Telegram"
- 5-25s: Show Make.com scenario → Click Run Once → Show Telegram message arriving instantly
- 25-30s: "Built with Make.com + OpenWeatherMap — saves manual checking daily"

## 🚀 How To Replicate

1. openweathermap.org → Sign Up Free → API Keys → Copy Key (save privately, never commit)
2. Telegram → Search @BotFather → /newbot → Name: MyWeatherBot → Username: must end with bot → Copy Token (save privately)
3. Search @userinfobot → Start → Copy your Chat ID
4. Make.com → New Scenario → HTTP → Make a Request → URL: `https://api.openweathermap.org/data/2.5/weather?q=Lagos&appid=YOUR_API_KEY&units=metric` → Method: GET
5. Add Telegram → Send Message → Create Connection → Paste Bot Token → Chat ID: your ID → Message Text: template above
6. Schedule: Click clock icon → Every day 7:00 AM → Save → Turn ON
7. Test: Run Once → Check Telegram

## 🔒 Security — READ THIS

- **NEVER** upload your real API key or bot token to GitHub
- In screenshots, blur keys with Canva or phone markup
- In blueprint.json, replace keys with `YOUR_API_KEY` and `YOUR_BOT_TOKEN`
- Public repos leak secrets within hours — bots scan GitHub constantly

## 📄 Case Study

See `case-study.md`

---
**Built by Isaac — aiagentbuilderhq | [Full Portfolio](https://github.com/aiagentbuilderhq/automation-portfolio)**
