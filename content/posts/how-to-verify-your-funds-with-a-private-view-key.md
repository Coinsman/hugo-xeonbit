---
title: 'How to verify your funds with a private view key'
date: Thu, 26 Sep 2019 05:47:49 +0000
draft: false
tags: ['Expert Tips', 'How to', 'viewkey']
toc: true
related: true
social_share: true
---

To prevent your Xeonbit (XNB) funds from being stolen if your computer is hacked, you will probably want to keep some of your funds in long term offline [cold storage].

In other words, you'd store your Xeonbit (XNB) in a wallet that you don't keep stored on your regular computer. You'd instead reboot to a freshly installed operating system that is unlikely to have any viruses, download the wallet software, disconnect your computer from the internet and create an offline wallet.

You'd then write the wallet seed down onto a piece of paper, delete the wallet from your computer and reboot.

Since your offline wallet will have never communicated with the internet, you'll want to check that your funds did really arrive to your offline wallet.

To do this, you will need to know your wallet's secret "view key" and your wallet's "address". At the time of writing, only the command line wallet can display your view key. To display your view key, run the command line wallet and type:\[wallet WcB5AUY\]: address **WcB5AUYzHvHYUxgHfyKUed2LoVyzgVDoi2zRXpJpYZ1CVDXma9p1fzsDhTscVLogx1MFbSrKtz4KBEBcUSvWajyq2t6Kvjrvk**\[wallet WcB5AUYz\]: viewkey secret: 8a881f323c5e43dc64cd8a648eda40be6d544acd9fbf8cbceca6d510d634a804 public: a0bc7f63eb578148a578167fabf3367f87a43ee601d9feda98c803c135c0b509The "secret" view key is what you will need. If the view key is ever disclosed, the worst that can happen is that someone will be able to view your funds. They will not be able to steal them.

Once you have the secret view key, you can create a new wallet that is only able to view funds on an internet-connected computer. This currently requires the command line version of Xeonbit (XNB). To create a command line wallet from your view key, do the following: (replace "**myviewonlywallet**" with the filename you'd like to use to save your wallet)

```
**./xeonbit-wallet-cli --generate-from-view-key myviewonlywallet** 
```

Xeonbit 'Dreizehnllium'' (v0.13.0.4-release) Logging at log level 0 to /root/xeonbit/./xeonbit-wallet-cli.log Restore from specific blockchain height (optional, default 0): 0 Standard address: **WcB5AUYzHvHYUxgHfyKUed2LoVyzgVDoi2zRXpJpYZ1CVDXma9p1fzsDhTscVLogx1MFbSrKtz4KBEBcUSvWajyq2t6Kvjrvk** View key: **8a881f323c5e43dc64cd8a648eda40be6d544acd9fbf8cbceca6d510d634a804** Enter a password for your new wallet: \*\*\*\*\*\*\*\*\*\* Confirm Password: \*\*\*\*\*\*\*\*\*\* Generated new wallet: **WcB5AUYzHvHYUxgHfyKUed2LoVyzgVDoi2zRXpJpYZ1CVDXma9p1fzsDhTscVLogx1MFbSrKtz4KBEBcUSvWajyq2t6Kvjrvk** Starting refresh... You can then use commands such as "balance" to check the contents of your view only wallet. You can also import the wallet file into your Xeonbit GUI to view the balance and transaction history there.

IMPORTANT: Using the steps outlined above, the view only wallet can ONLY be used to verify the amount of funds that have been sent to a wallet. If you spend your funds with a full wallet, your view only wallet will not reflect the decrease in funds. This is because Xeonbit's privacy mechanisms prevent anyone except an owner of a full wallet from knowing when funds have been spent. Therefore only rely on a view wallet to check when funds are received, and never rely on it to verify that funds have not been subsequently stolen.

There is a way to be able to monitor if you funds have been stolen using a view only wallet, and that requires you to export your 'key images' from your full wallet to your view only wallet. To do this, follow the clip.