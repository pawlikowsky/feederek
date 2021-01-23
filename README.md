# Feederek 
### Simple Telegram bot for providing feeds to telegram channel. 

## :warning: This script is outdated and not maintained for years. You can use it, but I recommend to look for other similar tools. :warning:

## Installation

Just download feederek.py and db.p (storage for feeds). Create Telegram channel and bot (If you are not familiar with telegram bots and chat read the docs https://core.telegram.org/bots). Set up your settings and run. 

## Settings 

Insert your feeds links into feed list

```python
feed_list =["https://yourfeed.com/feed/",
]
```

Paste your Telegram bot token

```python
bot = telegram.Bot(token='YOUR_TOKEN')
``` 

Set up your Telegram channel id
```python
bot.sendMessage(chat_id="@CHANNEL_NAME", text=message)
```

If you want to change number of checking last feeds (default 5), change

```python
for x in range(5):
```

## Summary

Last feeds links are store in db.p, but you can change it for almost any other kind of text file. You can set frequency of feeds checking using cron or similiar tool.  