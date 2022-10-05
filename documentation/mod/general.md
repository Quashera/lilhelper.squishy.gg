---
layout: default
title: Moderation
parent: Moderator Commands
nav_order: 1
---

# Moderation
{: .no_toc }

## Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Moderation Log

**!modlogset modlog**  
`!modlogset modlog [channel]`  
Set a channel as the modlog.  
Send without a mentioned channel to disable the modlog.  


## Messages
**!purge**  
`!purge [number of messages]`  
Deletes a provided amount of messages from the channel  
>!purge 78
{: .usage }

**!slowmode**  
`!slowmode [interval=0:00:00]`  
Changes channel's slowmode setting.  


## Kicking And Banning

**Normal Ban**  
`!ban [user] [days] [reason]`  
Bans a user  
You have to tag a user, and optionally you can add how many days of messages you want to delete, and a reason to appear in the logs.  
[user] a tagged person  
[days] is nuber of days of messages to delete *Minimum 0 days, maximum 7.*   
[reason] is for the logs.  
*If [days] is not specified, it's treated as the first word of the reason. *  

>!ban @cutie 5 posting spam time and time again
{: .usage }
  

**Hack Ban**  
`!hackban [userID] [days] [reason]`  
Bans user(s) that are not currently in the server, optionally you can add how many days of messages you want to delete, and a reason to appear in the logs.  
[userID] a user ID  
[days] is nuber of days of messages to delete, if they have been in your discord before *Minimum 0 days, maximum 7.*  
[reason] is for the logs.  
*If [days] is not specified, it's treated as the first word of the reason.*  
>*Requires specifying the target user's ID, To find this, you may either:*  
>*1. Copy it from the mod log case (if one was created)*  
>*2. enable developer mode, right'click the user and select 'Copy ID'.*  

>!hackban 105845684625548632 3 spamming in that other discord i'm in
{: .usage }

**Kick**  
`!kick [user] [reason]`  
Kick a user.   

**Soft Ban**  
`!softban <user> [reason]`  
Kick a user and delete 1 day's worth of their messages.  


**Temporary Ban**  
`!tempban <user> [days=1] [reason]`  
Temporarily ban a user from this server.  


**Unban**  
`!unban <user_id> [reason]`  
Unban a user from this server.  
>*Requires specifying the target user's ID, To find this, you may either:*  
>*1. Copy it from the mod log case (if one was created)*  
>*2. enable developer mode, go to Bans in this server's settings, right-click the user and select 'Copy ID'.* 

>!unban 105845684625548632 they promised they'd buy me chocolate
{: .usage }

## Voice moderation
**!voiceban**  
Ban a user from speaking and listening in the server's voicechats   
`Syntax: !voiceban <user> [reason]`

**!voicekick**  
Kick a member from a voice channel.  
`Syntax: !voicekick <member> [reason]`

**!voiceunban** Unban a user from speaking and listening in the server.  
`Syntax: !voiceunban <user> [reason]`

## User information and names
**!userinfo**  
Show information about a user.  

**!names**  
Show previous names and nicknames of a user.  

**!rename**  
Change a user's nickname.  
`Syntax: !rename <user> [nickname]`

## Warnings
Warnings:
actionlist List all configured automated actions for Warnings.  
mywarnings List warnings for yourself.  
reasonlist List all configured reasons for Warnings.  
unwarn Remove a warning from a user.  
warn Warn the user for the specified reason.  
warnaction Manage automated actions for Warnings.  
warnings List the warnings for the specified user.  
warningset Manage settings for Warnings.  
warnreason Manage warning reasons.  


## Moderation Configuration

**!modset**  
Manage server administration settings.  

**!modset banmentionspam**  
Set the autoban conditions for mention spam.
**!modset defaultdays**  
Set the default number of days worth of messages to...
**!modset deleterepeats**  
Enable auto-deletion of repeated messages.
**!modset dm**  
Toggle whether a message should be sent to a user when they ...
**!modset hierarchy**  
Toggle role hierarchy check for mods and admins.
**!modset reinvite**  
Toggle whether an invite will be sent to a user when u...

## Birthday management
For birthday user commands, see user commands  
/documentation/user/other.html#birthdays

**List all registered birthdays**  
`!birthday list`  
Lists the birthdays of users in the server.  

**Change the role assigned to users on their birthday**  
`!birthday role <role>`  
Sets the role to assign to a birthday user.  
Make sure this role can be assigned and removed by the bot by placing it in the correct hierarchy location.  
> !birthday role @BDAY CHILD 
{: .usage }

**Removing the birthday role**  
`!birthday unassign <member>`  
Removes the birthday role from a tagged user
>!birthday unassign @squishy#1234
{: .usage }

**Message Channel**  
`!birthday channel [channel]`  
Set(toggle) the channel to mention members on their birthday.  
Defaults to current channel if you don't mention a channel  
> !birthday channel #general
{: .usage }

To test the channel mention, you can run `!birthday test`  

**Adding other users**  
`!birthday aadd <member> [day] [month]`  
Add any user's birthday to the list. If date is not specified, it will default to the current day. 
> !birthday aadd @squishy#1234 24 3  
{: .usage }

**Removing other users**  
`!birthday adelete <member>`
Delete any user's birthday role and birthday from the list.
> !birthday adelete @squishy#1234
{: .usage }
