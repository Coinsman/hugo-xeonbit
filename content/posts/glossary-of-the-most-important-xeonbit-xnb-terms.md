---
title: 'Glossary of the most important Xeonbit $XNB terms'
date: Thu, 08 Nov 2018 08:22:21 +0000
draft: false
tags: ['Articles', 'Expert Tips', 'Glossary', 'Technology', 'xeonbit', 'Xeonbit Updates', 'XNB']
toc: true
related: true
social_share: true
---

Public address
--------------

Also known as your address or wallet address . An example address looks like this: WcAH3omZSUYCmJYskCUx2tV5oB5tLVrp58AeMYLrFhcz2umUVQHiHu62nG5CS3mvcfgKHC3fPtq6DHkEbMjqvCAZJW5nw9E

Payment id
----------

When someone sends you funds, they can specify a payment ID of their or your choice. Because Xeonbit $XNB's privacy protections usually prevent you from knowing the source of funds that you receive, the payment ID can be used by the sender to identify themselves to you.

Integrated payment address
--------------------------

To make it easier for other people to send you funds with a payment ID that you require, you can generate an integrated address to send to them which contains both your public address and the payment ID you request them to use.

Wallet / wallet files / wallet software
---------------------------------------

Your wallet holds your private key, which allows you to view your funds and spend them. A wallet may be configured to only hold a view key, so that the wallet can observe your funds but not spend them. Your wallet also contains a list of transaction IDs and transaction keys, which allow you to see a list of payments you've previously made. If you create another wallet from your seed (which is a representation of your private key), then you will have the full ability to spend your funds but you will not be able to see a list of transactions that you've previously made. This is why, if you need to see a history of your transactions, that you should back up your wallet files and not just your seed. 'Wallet' may refer to just the wallet files on your computer, or additionally to the wallet software that you run which allows you to view your wallet files and transact. Your wallet communicates with a Xeonbit $XNB daemon to scan the blockchain for incoming transactions and to send new transactions.

Private key / Seed
------------------

Your private key is what allows you to spend your funds. Your 'seed' is just a 25 word representation of your private key which is easy for you to write down on paper. You must keep your private key a secret, or other people will be able to spend your funds. Your private key is the only thing you need to access and spend your funds. Your public address can be recovered from your private key, so you do not need to additionally keep a note of your public address.

View key, also known as a secret view key or private view key
-------------------------------------------------------------

Your view key is normally kept private. If you wish, you can give out your view key so that others can observe the contents of your wallet. For security reasons, you may use your own view key to observe your funds on a computer which may be at risk of attack. Therefore if that computer became compromised, the attacker could see that you have funds, but not be able to steal them. Your private key would be kept safe and only used when you need to send funds when on a more secure computer.

Daemon
------

'Daemon' is a technical term for a program that runs in the background. Xeonbit $XNB uses a daemon to synchronize with the Xeonbit $XNB network to scan for incoming transactions and to send new transactions. Your wallet needs to use the daemon to scan the entire blockchain for incoming transactions, because only your wallet has your private view key. Only your private view key can be used to detect which transactions on the Xeonbit $XNB network have been sent to you. This is a key part of Xeonbit $XNB's privacy technology.

Balance / Unlocked balance
--------------------------

When someone sends you funds, they will appear in your balance. Once the Xeonbit network has 'confirmed' the transaction 10 times, which will take on average 20 minutes, your funds will become spendable and will be listed as part of your 'unlocked' balance. The 10 confirmation minimum is necessary to prevent double spending by the sender.

Refresh / synchronization
-------------------------

Because of Xeonbit $XNB 's privacy mechanisms, your private view key needs to be used to scan the blockchain to detect transactions destined for you. This means that until your wallet software has scanned the entire blockchain, you will not see your funds appear in your wallet's balance.

Mining / Blocks / Blockchain
----------------------------

Mining is the process by which the network of Xeonbit $XNB nodes collectively verifies transactions, in exchange for a small transaction fee. When transactions are mined, this causes them to appear in a block, which is added to the blockchain. The blockchain is therefore the entire record of all Xeonbit $XNB transactions that have ever taken place. Xeonbit $XNB's privacy mechanisms ensure that the blockchain can only be used to reveal information about transactions to those involved in the transaction. The blockchain is necessary to prevent the double-spending of funds, because it contains the information necessary to verify that funds have not already been spent by their owner.

Mining pool
-----------

A group of computers that together run mining software to process Xeonbit $XNB transactions and collectively share in the reward. The advantage of a Mining pool is that a single computer would take too long to mine a single block if it were working alone, and so the owner of the computer would have to wait unreasonably long to receive their first share of the mining rewards.

Privacy level / mixing
----------------------

When you send funds, Xeonbit $XNB 's privacy mechanism will obscure your funds as a possible source by 'mixing in' other sources of funds in the transaction. It is impossible for any observer to know which is the real source of the funds, and only you can prove that you were the real source by deciding to reveal the secret transaction key generated by you for that transaction. A mixing level of 4, which is the minimum allowable in the Xeonbit $XNB GUI, will mean that your funds will appear to be one of 5 possible sources of funds for the transaction. In the GUI, the mixing level is referred to as the 'privacy level'. Remember that every other person that sends a transaction may randomly select your funds to be a plausible source in their own transaction. This means that although it may at first seem like you are one of 5 possible senders, the aggregate effect of all Xeonbit $XNB users constantly mixing each others' funds means your privacy level is radically higher than the number '5' would at first suggest. Over time, it will appear as if you've at some point plausibly directly or indirectly participated in transactions with most other Xeonbit $XNB users, even if you're hardly ever using Xeonbit $XNB.

Transaction priority
--------------------

Your transaction will be mined into a new block on the blockchain. However, if there are a lot of transactions occurring, your transaction may not make it into the very next block that is mined, and so you may have to wait a few more minutes for your transaction to be included in the blockchain. You can increase your transaction priority to compete for position in the next block that gets mined. Usually, there is no reason to increase your transaction priority because there will most often be room in the next block for your transaction. Xeonbit $XNB has been designed to automatically increase the size of blocks as transaction volume increases, which means you only need to adjust your transaction priority higher if the Xeonbit $XNB network is temporarily experiencing a surge in transaction volume and the Xeonbit network has not yet adjusted upwards the sizes of blocks that are created to store those transactions.

Sweep unmixable
---------------

A button that appears in the beta version of the Xeonbit GUI that you don't have to worry about. It's only for those that received payments long ago, before RingCT and before denominations were used as part of Xeonbit transactions.

Exchange
--------

A place you can go to exchange dollars, Bitcoin or other currencies for Xeonbit $XNB.

XNB
---

The currency code for Xeonbit.

GUI
---

GUI Stands for Graphical User Interface. It makes it easy for you to use Xeonbit $XNB.

CLI / Command line interface
----------------------------

A text only application that does not have a graphical interface.

Stealth address
---------------

When a transaction is sent, Xeonbit $XNB does not publicly record the recipient's public address as the destination, and instead creates a new anonymous one-time address as the destination that is not linked to the recipient's public address. This one-time address is called a stealth address, because it ensures that your public address does not appear on the blockchain. Only the recipient has the necessary secret view key to scan the blockchain to locate these one-time destination addresses that contain the received funds.