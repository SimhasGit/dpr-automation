# DPR Automation

A Telegram bot that converts casual employee messages into structured Daily Progress Reports and emails them automatically.

## How it works
1. Employee sends a casual message to the Telegram bot
2. Gemini AI formats it into a structured report
3. Report is emailed to the manager via Gmail

## Stack
- n8n (workflow automation)
- Telegram Bot API
- Google Gemini AI
- Gmail

## Report Format
- Work Done
- Achievements
- Hurdles / Blockers
- Help Needed

## Setup
1. Clone this repo
2. Import `workflows/DPR Automation.json` into n8n
3. Configure credentials (Telegram, Gemini, Gmail)
4. Set up ngrok or host n8n on a VPS
5. Register Telegram webhook
