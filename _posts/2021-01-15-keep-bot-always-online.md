---
title: "Keep your Minecraft Bot always online"
categories:
  - Tutorial
tags:
  - AFK
  - Minecraft
  - Reconnect
  - Bot
---

This tutorial will show you how to keep your McBot always online. If you don't know what McBot is, feel free to read our last tutorial here: [AFK your Minecraft farms without a computer](/tutorial/afk-minecraft-farms-without-computer/). In short, McBot is a Minecraft Bot service in the cloud. You don't need to download or install anything, and you'll be able to AFK your farms without keeping your computer on.

## Why

If you play on some public Minecraft servers, you may have experienced the following situations:
- Server got restarted sometimes (usually daily)
- Got kicked out randomly due to AFKing
- Disconnected from server because of your intermittent internet connection
- Computer went to sleep
- and more...

McBot has a build-in feature to try to reconnect to the server automatically when disconnected.

## How to set it up

By default, the feature is not turned on. You need to manually enable it by:

Navigate to your Bot `Settings` page, and choose an option like this:

![screenshot for the settings page](/assets/images/2021_1_bot_settings_options.png)

You can pick either `in 5 min` or `in 10 min`. It means in how many minutes your Bot will try to reconnect to the server after disconnected.

If you are playing on your own server, `in 5 min` is a good option, but if you are playing on some public server, `in 10 min` is preferred.

Click `Save` button to save your preference settings.

## Notes

The change would not apply to a running Bot. Your Bot will pick up the preferences next time when you click `Start Bot` button.

When you are playing on your computer, remember to **stop your Bot** if you have set up auto-reconnecting. Otherwise, your Bot will try to reconnect and kick you out :)
