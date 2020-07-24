# Bitmex-to-Telegram
> Manage your Bitmex account using the Telegram bot


## Configuration

### Telegram bot

* Contact [@BotFather](https://t.me/botfather) in your Telegram messenger
* Create a new bot by sending ```/newbot``` command and choose new name for your bot. Then, you will receive an access token.
* Head over to the ```bot_manager.py``` file and set your access token to ```TELEGRAM_BOT_TOKEN``` variable

### Bitmex API KEYS

* Setup ```BITMEX_API_KEY``` and ```BITMEX_API_SECRET``` environment variables to your bitmex account api key and secret.

## Make Telegram Bot Private

You need to make sure that no one will use this bot except yourself. So, we make the bot so that it will respond only to messages from your telegram account.

Run ```main.py``` file, send ```/help``` command in your bot and check the logs. You get:

```
2020-07-24 20:17:03,612 - bot_manager - INFO - Admin Chat ID: 432156789
2020-07-24 20:17:03,612 - bot_manager - INFO - First Name: Spiral
2020-07-24 20:17:03,612 - bot_manager - INFO - Last Name: Dev
```

Now, stop the script and head over to the ```telegram_helper.py``` file and set ```ADMIN_CHAT_ID```, ```ADMIN_FIRST_NAME``` and ```ADMIN_LAST_NAME``` variables to what you got from the console.

Done!

## Commands

Bot has the following commands:
```
/help - List of all commands 
/long - Create buy market order. ::Symbol, Quantity 
/short - Create sell market order. ::Symbol, Quantity 
/margin_status - Get margin status 
/positions - Get open positions 
/orders - Get orders ::Last-n 
/cancel - Cancel order with ID ::OrderID 
/cancel_all - Cancel all orders 
/leverage - Set leverage ::Symbol,leverage 
/history - Get wallet history. ::Last-n 
/instrument - Get instrument(s). ::Symbol 
/indices - Get price indices. ::Root Symbol
```

## Contributions
Contributions and feature requests are always welcome! 

## Support

Your Support and Donations are welcomed and appreciated!

* **BTC:** 1PUGs6mxcW2W3SJi95aG8GvRQRJsoFHWWQ

* **ETH:** 0x66615e09f7f46429e7620ffbf78479879bbab41d

* **LTC:** LRxYMgEXMumwxYdimZo9EJ5CfBcipD5c3n
