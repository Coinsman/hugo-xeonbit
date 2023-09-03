---
title: 'How to mine Xeonbit $XNB?'
date: Thu, 08 Nov 2018 09:19:43 +0000
draft: false
tags: ['Articles', 'CPU', 'GPU', 'How to', 'Mining', 'mining', 'Technology', 'xeonbit', 'Xeonbit Updates', 'XNB']
toc: true
related: true
social_share: true
---

**Xeonbit (XNB)** is a Cryptonote algorithm based cryptocurrency, it relies on Ring Signatures in order to provide a certain degree of privacy when making a transaction. Xeonbit is a Proof of Work (PoW) cryptocurrency that can be miner with computational power from a CPU or GPU. There are currently no ASICs for Xeonbit, which means that anyone with a computer can mine it. The first thing you need to think about is if you are going to mine solo or on a pool. Mining on a pool usually comes with a fee but also has it’s advantages. Users that don’t have enough computational power may have to wait long periods of time before getting a reward, in a pool users pull their efforts together in order to reduce variance and have a steady flow of income. Users that have enough hardware or simply want to mine solo can also benefit from solo pools which function in the same way as normal solo mining, but don’t require users to run a full node or store the entire blockchain. We are going to use Xeonbit Hash for this guide, but you can use goldenhillpool.com, pool.xeonbit.com or any pool you like. Today we’re going to show you how to mine $XNB on a Mining Pool Goldenhillpool and pool.xeonbit.com AMD Graphic cards are optimal for Xeonbit Mining, but you can also mine it with a Nvidia GPU or CPU. To allow users to get the most profit for their specific hardware we will use a different software that was created for each of this options. **Part 1 – CPU Mining**

*   Step 1: Download the mining software. For this section of the guide we are going to use Wolf’s CryptoNote open souce CPU Miner, since it’s the one that has the provides the best results. You can find from bitcointalk link or github link 
*   Step 2: Extract the .zip file. You will be left with a folder like the one below.


*   Step 3: Now, inside the miner folder we have just extracted from the .zip file, you’ll need to hit ctrl + right mousekey. By doing this you’ll be given an extra option “open command window here”, click it and a command line window will appear.


*   Step 4: Now that our command line window (miner) is ready to go, all we need to do is type in the command: “minerd -a cryptonight -o stratum+tcp://goldenhillpool.com:1212 -uYOUR\_WALLET\_ADDRESS -p x”. You have to replace “YOUR\_WALLET\_ADDRESS” for your actual XNB wallet adress.
 You are now mining Xeonbit $XNB ! You can view all of the commands available by typing “minerd –help”. In our case we’re just using the -a command, which stands for algorithm, the -o stands for server, the -u is your wallet address and the -p is your password, which can be left with an x when the Mining pool does not require you to login. **Part 2 – AMD GPU Mining**

*   Step 1: Download the mining software. For this section of the guide we are going to use Wolf’s CryptoNote open souce AMD GPU Miner, since it’s the one that has the provides the best results. You can find the Download link Wolf9 or Claymore OpenCL (AMD)


*   Step 2: Extract the .zip file. You will be left with a folder like the one below.


*   Step 3: Now you’ll need to configure the xnb.conf or coin.conf file, open the file with the note pad and change “url”: to “stratum+tcp://goldenhillpool.com:1212” to your pool address or “stratum+tcp://pool.xeonbit.com:1212”. Replace the user with your wallet, in this case: “user”: “WcBfPDzkV5NUDpwrA7Df6UXfuzj2TRENXeNFjt3CSAjN33osXE6zK5XFsG6ihaaQ2qFnGRzcidcddWU4aUjMEqUM1ffPJ89zh”


*   Step 4: Once xnb.conf file is configured you need to go inside the miner folder we have extracted from the .zip file and hit ctrl + right mousekey (For windows 10 to get the extra options you need to hold shift+right mousekey). By doing this you’ll be given an extra option “open command window here”, click it and a command line window will appear.
 Now that our command line window (miner) is ready to go, all we need to do is point the miner to the xnb.conf file. type: “miner xnb.conf” And that’s it, you are now mining with your AMD GPU, which will surely give you the best results when mining XNB. **Part 3 – Nvidia GPU Mining**

*   Step 1: Download the mining software. For this section of the guide we are going to use CCMiner version forked by tsiv, since it’s the one that has the provides the best results when mining with Nvidia Graphic Cards.


*   Step 2: Extract the .zip file. You will be left with a folder like the one below.


*   Step 3: Now, inside the miner folder we have just extracted from the .zip file, you’ll need to hit ctrl + right mouse key (For windows 10 to get the extra options you need to hold shift+right mouse key). By doing this you’ll be given an extra option “open command window here”, click it and a command line window will appear.


*   Step 4: Now that our command line window (miner) is ready to go, all we need to do is type in the command: “ccminer -o stratum+tcp://goldenhillpool.com:1212 -u YOUR\_WALLET\_ADDRESS -p x”. You have to replace “YOUR\_WALLET\_ADDRESS” for your actual XNB wallet address. That was the last step. You are now mining Xeonbit XNB with your Nvidia Graphic Card. As you can see, mining XNB Xeonbit is possible with any hardware, even a CPU! What are you waiting for? So why not give it a try? (source: cryptocompare)