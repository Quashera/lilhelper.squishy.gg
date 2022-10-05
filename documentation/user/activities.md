---
layout: default
title: Activities
parent: User Commands
nav_order: 5
---

# Activities
{: .no_toc }

## Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Dice rolls
**!dice**  
Perform die roll.  
`!dice [how many and what type of die]`  
>!dice 2d6+1d20
{: .usage }
## Very important facts
**!catfact**  
Gets a random cat fact.

## Banking and Money

### Banking  

**Check your balance**  
`!bank balance [user]`  
Show the user's account balance. If no user is mentioned it checks your own bank account.  

**Transfer money**  
`!bank transfer <tagged user> <amount>`  
Transfer currency to other users.  
This will come out of your balance, so make sure you have enough!  
>!transfer @squishy 69
{: .usage }

### "Earning" Cutiecoins
**Go to work**  
`!work`  
You go to work, and earn some cash.

**Commit a crime**  
`!crime`  
You commit a crime! If you get caught you can lose your cutie coins, but if you succeed the payout can be quite good!  

**Play roulette**  
`!roulette <amount> <bet>`  
Bet on the roulette wheel! Amount is the money you bet, and the supported bets are;  
Single - Any single number.  
Colors - Red/Black  
Halfs - 1st/2nd half  
Even Odd - Even or Odd  
Dozens - 1st/2nd/3rd Dozen (Groups of 12)  
Colums - 1st/2nd/3rd Column.  
>!roulette 168 single
{: .usage }
`!roulette start`   
starts the game when everyone is done betting (+60s)  


**List your remaining cooldowns**  
`!cooldowns`  
Gives a list of your remaining cooldowns for crime and work for example  
