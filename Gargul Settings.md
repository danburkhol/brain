---
share: true
---


Here is how I configure and some tips on how I use Gargul to master loot efficiently with as little cognitive load on the operator as possible.

- [Macro - Click Popup](Gargul%20Settings.md#Macro%20-%20Click%20Popup)
	- [Explanation](Gargul%20Settings.md#Macro%20-%20Click%20Popup)
- [Gargul Configuration](Gargul%20Settings.md#Gargul%20Configuration)
	- [SoftRes](Gargul%20Settings.md#Gargul%20Configuration)
	- [Dropped Loot](Gargul%20Settings.md#Gargul%20Configuration)
	- [Loot Trade Timers](Gargul%20Settings.md#Gargul%20Configuration)
	- [Autoloot](Gargul%20Settings.md#Gargul%20Configuration)
		- [Autoloot Item Rules](Gargul%20Settings.md#Autoloot)
	- [Master Looting](Gargul%20Settings.md#Gargul%20Configuration)
		- [Roll Tracking](Gargul%20Settings.md#Master%20Looting)
		- [Awarding Loot](Gargul%20Settings.md#Master%20Looting)
	- [Trade Announcements](Gargul%20Settings.md#Gargul%20Configuration)


# Macro - Click Popup 
- This is not Gargul-specific but this macro saves me so much extra clicking in-game for so many things.
    - I bind this to my `X` key. Being able to just hit this macro when the trade window opens is so convenient. 
    - Single best quality of life macro I ever added in-game.

```
/click StaticPopup1Button1
/click QuestFrameCompleteQuestButton
/click QuestFrameCompleteButton
/click QuestFrameAcceptButton
/click TradeFrameTradeButton
/click BattlefieldFrameJoinButton
```

## Explanation
- **`/click StaticPopup1Button1`** - Clicks the first button on popup dialogs (usually "Yes", "Accept", or "OK")
- **`/click QuestFrameCompleteQuestButton`** - Clicks the "Complete Quest" button when turning in a quest
- **`/click QuestFrameCompleteButton`** - Clicks the final "Complete" button after selecting quest rewards
- **`/click QuestFrameAcceptButton`** - Clicks "Accept" to take a new quest
- **`/click TradeFrameTradeButton`** - Clicks the "Trade" button in player trading windows
- **`/click BattlefieldFrameJoinButton`** - Clicks "Join Battle" for battleground queues


# Gargul Configuration
## SoftRes
![Pasted image 20250719091503.png](./0%20-%20Attachments/Pasted%20image%2020250719091503.png)

## Dropped Loot
- Use raid warning!
![Pasted image 20250719091540.png](./0%20-%20Attachments/Pasted%20image%2020250719091540.png)

## Loot Trade Timers
- Using the Loot Trade Timer bars is the best way to track the loot to be rolled.
- Having the bars enabled, I can simply go down the list and `alt + click` to initiate a roll. 
- Once it's awarded, it's cleared from the list and I can move on. 
- No digging in bags to find things!!!
    - One exception is BoE Epics. Since they do not have a trade expiration, they don't show up here. 

- Note: I unchecked "Only show bars when I'm the master looter" so I could show the trade timers in the screenshot. I keep that checked otherwise.

![Pasted image 20250719092151.png](./0%20-%20Attachments/Pasted%20image%2020250719092151.png)


## Autoloot
- Autoloot always, just go go go go.
- If it cannot be autolooted, the loot window will stay open. 
- For items that cannot but autolooted for any reason, `alt + click` to roll it off immediately. 
    - It'll be sent to the winner's bag from the loot window upon award.
![Pasted image 20250719092340.png](./0%20-%20Attachments/Pasted%20image%2020250719092340.png)

### Autoloot Item Rules
- Typically I'll autoloot everything to myself. 
    - But to save bag space, if you have a willing raider, you can assign items of a specific rarity threshold be sent to someone else.
    - e.g. Send all firey cores to someone else trusted to save your bag space.
- Autoloot _will not_ pick up untradeable items. So you do not have to worry about accidentally looting things like the Tranq Shot book or a Dragon Head.

![Pasted image 20250719092359.png](./0%20-%20Attachments/Pasted%20image%2020250719092359.png)


## Master Looting
![Pasted image 20250719092741.png](./0%20-%20Attachments/Pasted%20image%2020250719092741.png)

### Roll Tracking
- I prefer to do a 10 second roll timer AND accept rolls 10 seconds after the rolloff ends. 
- Players actually have 20 seconds to roll on an item but are only exposed to the 10 second timer, giving them a sense of urgency. 
- And it just feels better than 20 seconds some how.
![Pasted image 20250719092813.png](./0%20-%20Attachments/Pasted%20image%2020250719092813.png)

### Awarding Loot
- Auto trading with the disenchanter during the rolloff is just a mess. Do it when you're all done.

![Pasted image 20250719093501.png](./0%20-%20Attachments/Pasted%20image%2020250719093501.png)


## Trade Announcements
![Pasted image 20250719093640.png](./0%20-%20Attachments/Pasted%20image%2020250719093640.png)

