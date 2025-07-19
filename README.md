
## 📈 Crypto Price Alert Bot with n8n + Telegram

A fully automated cryptocurrency price alert bot built with n8n and integrated with Telegram. This workflow fetches live prices of popular cryptocurrencies every 15 minutes and sends real-time updates to a Telegram chat. It also alerts you when any coin price drops below your custom threshold.

---

## ⚙️ Features

⏱️ Scheduled every 15 minutes – Automatically runs and checks prices.

📊 Supports multiple coins – Currently fetches BTC, ETH, XRP, SOL, and DOGE.

📩 Sends Telegram messages – Uses your own bot to send updates to your Telegram chat.

🚨 Alerts on price drop – Triggers a special warning message or sticker if any price falls below your defined threshold.

---

## 🧰 Requirements

n8n (self-hosted or cloud)

A Telegram Bot

A Telegram chat ID (personal or group)

Free crypto price API (e.g., DIA Data)

Basic understanding of n8n nodes and workflows

---

## 🚀 Setup

1. Create a Telegram bot via BotFather and get the API token.

2. Find your Telegram chat ID (you can use @userinfobot or check message updates).

3. Import the workflow into n8n.

4. Replace all GET API URLs (default: https://api.diadata.org/v1/price/...) with your preferred coins.

5. Set your own price thresholds in the IF nodes (e.g., alert if BTC < $60,000).

6. Configure the Telegram node with your bot token and chat ID.

---

## 🔄 How It Works

1. A Schedule Trigger runs the flow every 15 minutes.

2. It fetches real-time prices for five coins (XRP, SOL, BTC, DOGE, ETH).

3. Each result goes through an IF condition:

If price is normal → gets added to a daily summary.

If price is below threshold → sends an alert message (or sticker).

4. Sends the final message(s) to the Telegram chat using your bot.

---

## 🤝 License

This project is open-source under the MIT License.

---

## 🤝 Contact
Feel free to connect with me on LinkedIn or check out more of my work on GitHub.

