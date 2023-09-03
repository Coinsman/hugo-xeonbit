---
title: 'How to track your received amount on Explorer and Restore your wallet from 24-25 words seed?'
date: Thu, 08 Nov 2018 08:59:41 +0000
draft: false
tags: ['How to', 'Restore your wallet', 'Security', 'Technology', 'track your amount', 'xeonbit', 'Xeonbit Updates', 'XNB']
toc: true
related: true
social_share: true
---

There is use-case about sending to another wallet but balance not showing on the receive address. Please make sure your target address is correctly and your transaction got confirmation on blockchain. Fist of all please run your daemon xeonbitd.exe before sending or receiving. Type command ‘status’ to see if it had synced to the latest block. Open your xeonbit-wallet-cli.exe to login your sendwallet to check your current balance after sending. Balance will show automatically after loading your wallet. Please use command ‘show\_transfers out’ to check all the transactions had been sent out. As in the example above image, the latest transaction is the transaction we had sent out to receive address. Now let’s check the transaction on explorer.xeonbit.com if the wallet had reach the receive address. Question: But in my receive wallet the balance do not show? like the image below Answer: Actually the amount had been reached your wallet and confirmed on blockchain, you may use your viewkey to Decode Out put on explorer.xeonbit.com with the receiving transaction. How to get your viewkey? Type command ‘viewkey’ copy the secret viewkey and paste it on explorer.xeonbit.com Decode Out put tab below transactions viewing. Proof of receiving will be shown like the image below.

Question: But the balance in my wallet is still 0 XNB as shown. What should I do?

Answer: Please try to use command ‘rescan\_bc’ to reload your wallet again. If the balance still can not show we will recover the receivewallet from 24-25 words seed.

Please use command ‘seed’ to view your 24-25 words wallet seed, write down it on your note and keep it safe because with this seed any one can retrieve all your balance.

After get 24-25 word seed you can process like article restore seed on simplewallet on WIN x64 CLI also the same command to restore.

Just type ‘xeonbit-wallet-cli.exe –restore-deterministic-wallet’

Then you need to enter your new wallet name: restorewallet

Password is depend on you

Just Enter and let the Wallet Load from beginning of blockchain.


Congratulation!!!! After completed, your restorewallet will show up with the amount had been received.

Please don’t use your previous receivewallet. You should back up your 24-25 words wallet seed keep it safe.

After researching I found out, there are 24 word seed (previous version CLI) and 25 words wallet seed (for recent version CLI), both seed can recover same wallet address.

Troubleshoot with any balance not showing issue please follow these simple steps:

– Please make sure daemon is at the latest height. You can check on Pool or Explorer.

– Please make sure the transaction had been confirmed on blockchain. You can check on Explorer

– Please try to ‘rescan\_bc’ your wallet.

– Please try to restore your wallet from 24-25 words seed.

Thanks for your reading and learning more about Xeonbit $XNB. Happy researching !!!