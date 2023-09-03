---
title: 'Importing the Blockchain to Xeonbit GUI wallet (Windows)'
date: Thu, 02 May 2019 05:25:02 +0000
draft: false
tags: ['CLI', 'Expert Tips', 'GUI', 'How to', 'Import blockchain', 'Technical and Troubleshooting', 'Technology', 'windows']
toc: true
related: true
social_share: true
---

### Step 1

Download our Current bootstrap or at Xeonbit Download Folder; you can skip this step if you are importing the Blockchain from another source.

### Step 2

Find the path of your Xeonbit wallet (the folder where you extracted your wallet). For example mine is:

`D:\xeonbit-gui-0.10.3.1`

Your path may be different depending on where you decided to download your wallet and what version of the Xeonbit wallet you have. Please use our latest wallet version from our Download Folder

### Step 3

Find the path of your downloaded Blockchain for example mine was:

`C:\Users\HappySun\Downloads\blockchain.raw`

Yours might be different depending on where you downloaded the Blockchain to.

### Step 4

Open a Command Prompt window. You can do this by pressing the Windows key + R, and then typing in the popup box `CMD`

### Step 5

Now you need to navigate using the CMD window to the path of your Xeonbit wallet. You can do this by typing:

`cd C:\YOUR\XEONBIT\WALLET\FILE\PATH\HERE`

It should look something like:

`cd D:\xeonbit-gui-0.10.3.1`

If your Xeonbit wallet is on another drive you can use `DriveLetter:` for example if your Xeonbit wallet was on your D drive then before using the cd command you would do `D:`

### Step 6

Now type in your command prompt window:

`xeonbit-blockchain-import --input-file C:\YOUR\BLOCKCHAIN\FILE\PATH\HERE`

For example I would type :

`xeonbit-blockchain-import --input-file C:\Users\HappySun\Downloads\blockchain.raw`

If you downloaded the Blockchain from a trusted, reputable source you may set `verify 0` this will reduce the amount of time to sync the Blockchain.

### Step 7

After the the Blockchain has finished syncing up you can open your Xeobit wallet normally. Your downloaded blockchain.raw can be deleted.