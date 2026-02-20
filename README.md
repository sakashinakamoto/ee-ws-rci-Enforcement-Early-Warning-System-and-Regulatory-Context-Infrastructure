# Enforcement Early Warning System + Regulatory Context Infrastructure (EEWS + RCI)

This repository contains the MVP for **EEWS + RCI** — an Enforcement Early Warning System and Regulatory Context Infrastructure designed to provide real‑time regulatory signal ingestion, automated RDI scoring, and founder‑focused alerts.

This system is:
- **Cloud‑based**
- **Telegram‑controlled**
- **Deployable on Render**
- **Operable from an iPhone**
- **Private MVP for AI/fintech risk signals**

---

## 🧠 Core Features (MVP)

1. **Regulatory Feed Ingestion**  
   Parses RSS feeds from regulatory agencies (FTC, SEC, CFPB).

2. **Regulatory Drift Index (RDI)**  
   Calculates a weekly risk score (0–100) based on signal velocity.

3. **Enforcement Early Warning System (EEWS)**  
   Sends alerts via Telegram with score + severity.

4. **Private Dashboard**  
   Lists captured signals and RDI scores.

---

## 📦 File Structure
---

## 🛠 Requirements

- Python 3.10+
- FastAPI
- SQLAlchemy
- PostgreSQL (or managed cloud DB)
- Render account
- Telegram Bot

---

## 🚀 Setup Instructions

### 1. Telegram Setup

1. Open Telegram → Search `@BotFather`
2. `/newbot` → Create bot → Copy token
3. Send a message to the bot
4. Fetch your chat ID:
5. Save:
- `TELEGRAM_BOT_TOKEN`
- `TELEGRAM_CHAT_ID`

---

### 2. Local Testing (Optional)

Install dependencies:

```bash
pip install -r requirements.txt
uvicorn app:app --reload
