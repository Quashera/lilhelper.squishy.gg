---
layout: default
title: Helping out
nav_order: 4
has_children: true
---

# Helping out 
{: .no_toc }

## Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

This section is gonna hold how-to guides and examples for how this documentation is made, and how to help out!  

## Protip
Pro tip, 2 spaces at the end of a line makes a new line  

## Example  
**What it does 1**  
`!command [value1] [value2]`  
Description of how it works/what it does  

>!usage example, best used with all values filled so they're easy to understand  
{: .usage }


Here's the example  you just have read in markdown:  
```markdown
## Example  
**What it does 1**  
`!command [value1] [value2]`  
Description of how it works/what it does  

>!usage example, best used with all values filled so they're easy to understand  
{: .usage }

```

## More advanced example
Here's an example with explenations of the different fields where that feels neccesary  

**Hack Ban**  
`!hackban [userID] [days] [reason]`  
Bans user(s) that are not currently in the server, optionally you can add how many days of messages you want to delete, and a reason to appear in the logs.  

`[userID]` a user ID  
`[days]` is nuber of days of messages to delete, if they have been in your discord before. *Minimum 0, maximum 7 days.*  
`[reason]` is for the logs.  
*If `[days]` is not specified, it's treated as the first word of the reason.*  
>*Requires specifying the target user's ID, To find this, you may either:*  
>*1. Copy it from the mod log case (if one was created)*  
>*2. enable developer mode, right'click the user and select 'Copy ID'.*  

>!hackban 105845684625548632 3 spamming in that other discord i'm in
{: .usage }

```markdown
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
```