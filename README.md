# Auto Reaction Bot No Hosting 

- **Telegram Bot that automatically reacts to posts in telegram channels, groups, and private messages**.
- **Lightweight and Serverless**: Built on Cloudflare Workers, the bot is serverless, efficient, and no hosting platform required.

## Deployment

**Step 1** : Create a Cloudflare Account 

**Step 2** : Go to Workers & Pages Tab, and Click on Create Worker and Choose a Sub Domain

**Step 3** : Copy code from Repo's react.js file and Paste it

**Step 4** : Add the `BOT_TOKEN` Secret:
    - Go back to your worker's dashboard.
    - Click on the **Settings** tab, then select **Variables**.
    - Under **Environment Variables**, click **Add variable**.
    - Enter `BOT_TOKEN` as the **Variable name** and paste your Telegram bot token as the **Value**.

**Step 5** : Click on Deploy and your Site is Ready !

### Step 5: Webhook Setup

```bash
https://api.telegram.org/bot<BOT_TOKEN>/setWebhook?url=<YOUR_WORKER_URL>
```
Replace the placeholders:
- `<BOT_TOKEN>` - Your bot token from BotFather
- `<YOUR_WORKER_URL>` - Your deployed Cloudflare Worker URL.
