---
title: "Support Login with Microsoft Account"
categories:
  - Update
tags:
  - McBot
  - Minecraft
  - Release
  - Authentication
  - Microsoft
---

We have received many user reports regarding Bot login failures: `Invalid credentials. Invalid username or password.`
After investigation, they were because we only supported Mojang account login but they were using Microsoft accounts.
According to Minecraft official website: 

> Beginning December 1, 2020, you will need a Microsoft account to buy and play Minecraft Java Edition.

Today, we start to allow Microsoft account logins!

## New Login Flow

Unlike Mojang account, Microsoft account login can involve many other factors such as 2FA, Different Location Warning. To still archieve our goal,
additional steps are needed from you to help your Bot get through the authentication process.

If you are using Microsoft account, you are likely to see the following screen after starting your Bot:

![screenshot for microsoft msa](/assets/images/2021_1_microsoft_msa.png)

Please follow the instructions and help your Bot complete the authentication flow.

**Note**: You should finish the verification flow **ASAP**. Otherwise, you'll likely experience some timeout issue, or your verification code would be expired.
If this is the case, just stop your Bot and start again.

## Need Help?

Since this is a brand new feature, if you have any trouble or question, feel free to contact us through `Need Help` button in the Bot page.
