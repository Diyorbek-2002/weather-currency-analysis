# Weather & Currency Telegram Bot

## 📌 Project Overview
This project is an automated Telegram bot that delivers daily weather updates and USD exchange rates to subscribed users.  
It fetches real-time data from public APIs and sends formatted messages every day at a scheduled time.

## ⚙️ Features
- Daily USD exchange rate (UZS and GBP)
- Current weather information for:
  - Tashkent
  - London
- Automated daily messages at 07:00
- User subscription management via Telegram commands
- Admin notifications for new and removed users

## 📊 Data Sources
- Weather data: OpenWeatherMap API
- Currency exchange rates: ExchangeRate API

## 🛠 Tools & Technologies
- Python
- asyncio, aiohttp
- python-telegram-bot
- REST APIs
- JSON file-based storage
- Task scheduling

## 🔍 How It Works
1. Users subscribe via the `/start` command
2. The bot stores user IDs in a JSON file
3. Every day at 07:00:
   - USD exchange rates are fetched
   - Weather data is collected for Tashkent and London
4. A formatted message is sent to all active users
5. Users can unsubscribe using `/stop`

## 📈 Key Skills Demonstrated
- Asynchronous programming in Python
- API integration and data handling
- Automation and scheduling
- Real-world bot deployment logic
- Clean separation of logic (data, messaging, scheduling)

## ▶️ How to Run the Project

### 1. Install dependencies
```bash
pip install python-telegram-bot aiohttp schedule
