# Whispr — Telegram Bot Setup

## Step 1: Create Your Bot (takes 2 minutes)

1. Open Telegram → Search for **@BotFather**
2. Send `/newbot`
3. Name it: `Whispr Ping`
4. Username: `WhisprPingBot` (or any available name like `whisprping_yourname_bot`)
5. BotFather gives you a **token** like: `7123456789:AAGxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`

## Step 2: Add Token to Whispr

Open `index.html` and find this line near the top of the script:

```javascript
const TG_BOT_TOKEN = 'YOUR_TELEGRAM_BOT_TOKEN_HERE';
```

Replace `YOUR_TELEGRAM_BOT_TOKEN_HERE` with your actual token.

## Step 3: Get Your Chat ID (and share process with friend)

Each user needs to:
1. Open Telegram → Search for **your bot name** (e.g. `@WhisprPingBot`)
2. Send `/start`
3. The bot won't reply yet (it's not set up for commands) — but you can get the Chat ID by:
   - Going to: `https://api.telegram.org/bot<YOUR_TOKEN>/getUpdates`
   - Find `"chat":{"id": 123456789}` — that number is the Chat ID

## Step 4: Enter Chat ID in Whispr

When you first log in to Whispr, the app will ask for your Telegram Chat ID.
Enter the number you found above.

## That's it!

When your friend sends you a message, you'll get a Telegram notification instantly.
