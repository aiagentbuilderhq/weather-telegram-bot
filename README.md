# Project 2: Weather API → Telegram Bot (Any API → Any Destination — Make.com + n8n + MCP)

> **One-liner:** Daily weather + any API data delivered to Telegram automatically — my first API integration, foundation for Shopify, Stripe, HubSpot, and any REST API. Built for Make.com AND n8n.

[![OpenWeatherMap API](https://img.shields.io/badge/API-OpenWeatherMap-orange)](https://openweathermap.org/api)
[![Telegram Bot API](https://img.shields.io/badge/Telegram%20Bot%20API-Bot-blue)](https://core.telegram.org/bots)
[![Make.com](https://img.shields.io/badge/Make.com-Automation-blue)](https://make.com)
[![n8n](https://img.shields.io/badge/n8n-Workflow-red)](https://n8n.io)
[![MCP](https://img.shields.io/badge/MCP-Model%20Context%20Protocol-purple)](https://modelcontextprotocol.io)
[![Webhooks](https://img.shields.io/badge/Webhooks-HTTP%20%2F%20JSON-orange)](https://en.wikipedia.org/wiki/Webhook)

**Live Hub:** [automation-portfolio](https://github.com/aiagentbuilderhq/automation-portfolio) | **Other Projects:** [Sheets → Gmail](https://github.com/aiagentbuilderhq/sheets-gmail-automation) · [Form → Slack](https://github.com/aiagentbuilderhq/form-slack-leads) · [AI Inbox](https://github.com/aiagentbuilderhq/ai-inbox-assistant) · [Lead Scoring](https://github.com/aiagentbuilderhq/ai-lead-scoring)

## 🎯 Problem
Learning APIs is intimidating. Most beginners never move past Sheets → Email. This project proves API handling is simple and repeatable — critical for client work where 80% of automations are API integrations (Shopify, Stripe, HubSpot, etc.).

## ✅ Solution — API → Telegram Pattern (Works for Any API)

**Core Pattern (Same for Make.com and n8n):**
1. **HTTP Request Node** — GET `https://api.openweathermap.org/data/2.5/weather?q=Lagos&appid=YOUR_KEY&units=metric` → Returns JSON
2. **Parse JSON / Set Node** — Extract temp, humidity, description
3. **Telegram Send Message** — Formatted alert via Telegram Bot API

**Why This Matters:** Replace OpenWeatherMap URL with Shopify API (`/admin/api/orders.json`), Stripe API (`/v1/charges`), HubSpot API (`/crm/v3/objects/contacts`) — same nodes, different URL. That's why founders hire API specialists.

**MCP Angle:** This workflow follows MCP principles — Model (API) → Context (JSON parsing) → Protocol (Telegram delivery). MCP is what advanced AI agents use to talk to tools.

## 🏗️ Architecture

```
Make.com:
[HTTP: Make a Request - OpenWeatherMap API / Any REST API]
        ↓
[Telegram: Send a Message — Telegram Bot API]
Message: 🌤 Weather in Lagos — Temp: {{temp}}°C — Humidity: {{humidity}}% — Condition: {{description}}

n8n:
[Schedule Trigger: Every Day 7 AM] → [HTTP Request: GET API] → [Set Node: Format Message] → [Telegram Node: Send Message]
```

## 📈 Results

- **Learning Outcome:** APIs = URL + Key + Method → JSON. Once understood, any API is automatable.
- **Build Time:** 20 minutes
- **Use Cases Unlocked:** Shopify New Order → Slack, Stripe Payment → Sheets, HubSpot Contact → Gmail, Any API → Any destination
- **Reliability:** Runs daily at 7 AM via Cron/Scheduling

## 🛠️ Tools Used — Founder-Searched Skills

- **APIs:** OpenWeatherMap API (Free) · Telegram Bot API (Free) · HTTP / REST APIs · JSON Parsing · Webhooks
- **Automation:** Make.com (Free) · n8n (Free self-host) · Scheduling / Cron
- **Advanced:** MCP (Model Context Protocol) pattern · Error Handling · Retry Logic
- **Running Cost:** $0/month
- **Translation to Client Work:** "Weather is demo — your Shopify, Stripe, HubSpot, Notion, Airtable — same pattern, different API endpoint"

## 🎥 Demo Video

**YouTube Unlisted Link:** `[Paste Link Here]`

**Demo Script:** Show Make.com scenario → Run Once → Telegram message arrives → Show n8n version → Show how swapping URL to Shopify API works

## 🚀 How To Replicate — Any API

1. Get API key (OpenWeatherMap, Shopify, Stripe — any)
2. Make.com: HTTP → Make a Request → URL: API endpoint → Method: GET → Headers: Authorization if needed
3. n8n: HTTP Request node → Same
4. Telegram: BotFather → /newbot → Copy Token → Telegram node → Chat ID → Message template
5. Schedule: Cron / Every day 7 AM
6. Test: Run Once → Check Telegram

**Client Pitch:** "If it has an API, I can connect it. Weather is just the demo. Your CRM, e-commerce, payment processor — same nodes, different URL. I work with both Make.com and n8n, so I build in your existing stack."

## 🔒 Security

- NEVER upload real API key or bot token
- Blur keys in screenshots
- Replace with `YOUR_API_KEY` in blueprint.json

---
**Built by Isaac — aiagentbuilderhq | [Full Portfolio Hub](https://github.com/aiagentbuilderhq/automation-portfolio) | Tech: Make.com + n8n + MCP + Any REST API + Telegram Bot API + Webhooks**
