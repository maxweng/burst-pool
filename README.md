burst-pool
==========

Lex Pool for Burstcoin
Official Pool URL: http://burst.lexitoshi.uk/#
Recipient: BURST-F3XD-Y4M5-SN8C-G9FFJ

please donate for development to or alternatly leave the (OPTIONAL) devfee on the pool on.

for burst or pool related discussion go to http://discord.io/burstofficial 

those who have enabled the devfee feature ill support as best as i can. this way you get some support for supporting the project.
the devfee also helps claw back the huge amount of burst i lost due to ghostblocks and forks. and the cost of the vps server for 4 months along with any development.

a few users disable the devfee and just send me a one off donation instead as a thank you for taking on this project and to help towards these costs.

We have already had a few keyboard warriors take to the forums about the devfee option but the argument stands that the software is still free and the fee is OPTIONAL and can be enabled/disabled at users descrestion. these users have caused themselves to lose credibility in the community so please refrain from any negative comments on the forums and if you have a problem please just message me instead. (note: im very busy with other burst related projects so it might take me a while to respond)

Donate :D buy me a beer or something ;)
[Burst] BURST-GAJL-VWKN-2XPB-H39R9

[Bitcoin] 1EWqGpP96Jx2gnD4UQBEoMrdpJPmLpdKJH

developed with node v4.7.1. works with versoin https://nodejs.org/download/release/v5.12.0/ and below

node v6 has changed a lot of functions and causes it to crash shortly after if not when a block is hit. or even stops it from running alltogether. a user has taken it upon himself to break backwards compatability for my users. 

please do not use pascal66's fork of the repo as it uses V6 & v7 of node. which when i do updates for the current versoin might not be compatably with his.

he also removed all credits to myself for any of the work i did for stopping ghostblocks. adding miner types. and various others.
this user went out of his way to descredit me on the forums by calling  me a copy and paste coder. and clearly didnt look at the commit history.

i will not help or support the versoin he has released.


forum thread

https://forums.burst-team.us/topic/2643/lex-pool-a-rewritten-pool-based-on-uray-source

config


"devFee" that if enabled would send [devFeePercent] of the pools earnings as a developer fee to myself after a few requests of people wanting to support the project. 1% works out to be less than 25 coins. getting lower each month.

"devFeePercent" pool owners can choose the percent they wish to donateto development

"blockMature" amount of blocks the pool goes back and checks for block winner

"txFeePercent" Currently not implemented. tx fee is currently added to block reward and then a pool fee is applied to that total - 0.01 = 1%

"poolFee" the percent a pool owner charges for hosting etc. 0.01 = 1%

"poolPort" the port the pool is run on. default 8124

"poolPvtKey" pool private key

"poolPublicRS" pool public BURST- Address

"poolPublic" Pool numerical burst address

"poolFeePaymentAddr" where the fees for Pool Fee should get sent

"cumulativeFundReduction" % to reserve for each prior round.

"logWebsocketToConsole" output whats sent to peoples browsers into the console window

"maxRoundCount" max rounds to display in all round shares. any that exceed this are deleted

"maxRecentPaymentHistory" max lines to show in payment history

 
 
 in the pool config.js a useful feature if you ever have to swap hosts is
 

redirection : {

      enabled : false,
      
      target : 'http://8.8.8.8:8124'
      
  },
  
so change the 8.8.8.8 on the old server config to the new servers ip and enabled to true then it should forward all the requests.

tip - make sure you also change a few characters in the old servers passphase so the pool doesnt accidentally pay out twice
