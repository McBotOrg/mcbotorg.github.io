---
title: "Making password optional"
categories:
  - Update
tags:
  - Minecraft
  - Bot
  - Password
---

**DRAFT**

We always treat our customers seriously and keep trying hard to make sure all the information is secure especially sensitive pieces such as passwords.
That's why we are still not providing password login because of course passwords are absolutely protected if we even don't ask for them.

Today, we are pushing this further and make the password field for Bot optional!

## Why password is needed to run Bot

Our Bot service (McBot) is actually a piece of code simulating Minecraft client to communicate with those Minecraft servers.
Minecraft servers require any player must use a working Minecraft account and validate it with a username and password.
Therefore, in case to connect to any Minecraft server, either an official Minecraft client, a third-party launcher, or McBot needs to use a username and password to launch the game. After successfully authentication, player can then join the game.

## How we store passwords

Our service automatically encrypts all data before it is written to disk, including passwords. It's done by server-side encryption automatically. We manages the cryptographic keys, and all the data is encrypted under the [256-bit Advanced Encryption Standard](https://en.wikipedia.org/wiki/Advanced_Encryption_Standard). Each encryption key is itself encrypted with a regularly rotated set of master keys. The data is automatically and transparently decrypted when used by an Bot when necessary.

## What is changed

We read some research from anonymous user behavior analysis, many user gave up us after signed in before creating any Bot. It could happen because of any concern regarding providing their Minecraft passwords. Although all data is encrypted persisted, it is a valid opinion still. We understand an make a big improvement like this:

[screenshot of bot creation without password]

Password is optional now. Bot will ask for a password only when it starts running:

[screenshot of bot asking for password]

Instead of storing password before, the piece of information is only transfering through network and server memory. i.e. Password is not saving to disk anywhere across our service. (We also use [SSL](https://en.wikipedia.org/wiki/HTTPS) for any network communication within our services)

## Disadvantage

Everything has its drawbacks. Without saving your password, your Bot will ask for password everytime when you try to start it, and the following features will be affected as well:
- Auto-reconnecting: Since Bot does not remember the password, it could not reconnect to servers if got disconnected.

If you don't like those disadvantages, you can continue saving the password for convenience. Remember, **all your data** is encrypted and stored securely.
