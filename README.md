# DPR Automation 🤖

A Telegram bot that converts casual employee messages into structured Daily Progress Reports using Gemini AI, emails them to managers via Gmail, and stores them in Supabase.

## How it works
1. Employee sends a casual message to the Telegram bot
2. Bot replies: "Got your message! Generating your report..."
3. Gemini AI formats it into a structured daily report
4. Report is emailed to the manager via Gmail
5. Employee gets a confirmation with a link to the sent email
6. Report is saved to Supabase database

## Stack
- n8n — workflow automation
- Telegram Bot API — employee interface
- Google Gemini AI — report formatting
- Gmail — email delivery
- Supabase (PostgreSQL) — report storage

## Report Format
- Work Done
- Achievements
- Hurdles / Blockers
- Help Needed

## Project Status
- [x] Telegram bot live
- [x] AI report formatting
- [x] Gmail delivery
- [x] Telegram status updates
- [x] Email link in confirmation
- [x] Error handling
- [x] Supabase storage
- [x] Structured field extraction
- [ ] Frontend dashboard
- [ ] Employee registration
- [ ] VPS hosting

## Setup
1. Clone this repo
2. Import `backend/DPR Automation.json` into n8n
3. Configure credentials (Telegram, Gemini, Gmail, Supabase)
4. Set up ngrok or host n8n on a VPS
5. Register Telegram webhook
