# About Winter!

Winter Bot is a legal bot made for the game "GOT: Winter is coming" that can help players with a variety of functions on discord.

Winter Bot is made to help players with Protocol officers queuing, offline calculations , game server management, Bubble reminder, Rally calculators, Buff calculators, Pack calculators and etc! Its also going to have a bunch of very cool online games for discord servers!

Most of the functions are free! To be able to make up for the hardware resources and host cost of this bot, and for future development, some are only available for Patreons. Winter needs your help! Join me on this journey and help winter to become the best!

## Support and Contact

Winter has expenses. I need money to be able to work on it properly! become my patreon and support Winter from today!

**[Become My Patron](https://www.patreon.com/winterbot)**

You can also find Winter discord channel [here](https://discord.gg/gVA9adu).

## Installation

To install Winter open the following link if you have the permission to do so (Server Management or Admin): [Install Link](https://discord.com/api/oauth2/authorize?client_id=626364547539664909&permissions=268435456&scope=applications.commands%20bot)

Just choose your server and confirm the captcha and it's done :)

Reminder that you don't need to give Winter the administrator permissions :) Bot needs "Manage roles" permission if you want the Po functions to work properly though!

**[Become My Patron](https://www.patreon.com/winterbot)**

## Help Function

```markdown
/help (command (Optional))
```

Helps you with your question about other winter functions :)

## Protocol Officing Functions

### Setup a PO channel

Before using the PO functions, a server admin who is a veteran patreon (5$ or higher) must use the following command in the channel they want to setup as po requests channel.

```markdown
/setuppo
```

This function is the only po function that is limited only to patreons, meaning after setting up a channel as PO channel, everyone will be able to use the rest of the functions for free unlimitedly.

After activating the channel as a PO channel, bot will send a confirmation message there and announces that it's party time!

**[Become My Patron](https://www.patreon.com/winterbot)**

### Active/Deactive (for POs)

The players who have a PO role on server can use this following function to announce they are active to give away the buffs.

```markdown
/activate-po
```

And when they are going offline they can use the following function to announce they are gone:

```markdown
/deactivate-po
```

Winter will automatically mention the "Active PO" whenever its anyones turn to recieve the buff.

Note: To be able to use this function, define a server role called "PO" (caps characters are not important) and give the role to all the people who should have access to this function (that should be able to announce themself as active po)

Note: If you define a server role called "Active PO" (caps characters are not important); the bot will automatically give that server role to the active po and will remove it from them when they go offline. Change the color of that role and click on "Display this role seprately" so when the bot gives the current active po that server role, they show up on top with a different color! pay attention that Winter needs to have Manage Roles permission over that new server role (it needs to be higher in roles list on your roles page in server setting). Ultimately you can give Winter admin permission.

Note: Server Admins and people with a server role called "Chief PO" are also allowed to -deactive people (In case they vanished or must be removed!)

### Need (for Players requesting for buff)

The players can request for a buff using this simple command:

```markdown
/need (buff) (for_account (Optional)) (ccs_buff (optional))
```

That way the bot will assume that their server nickname (display name) is their account name. Or they can request it for someone else (or input their account name manually in (for_account) optional parameter. In this case the bot will mention the person who made the request whenever needed but will ask the Protocol officier to give the buff to the alternative name they provide.

Players can add extra requests from PO or ask for ccs buffs using the (ccs_buff) option. The secondary requests will not be queued and will only be shown to PO so they can assign it when your turn comes. This is useful for assigning CCS buffs specially.

For example:
"/need buff:r for_account:"Winter Angel" ccs_buff:"Research officer"
Will queue Winter Angel for both Grand Maester and Research Officer. Winter Angel name will only exist in a single queue but the PO will be asked for both buffs.

Currently recognized buff aliases are (Not case sensetive):

Grand Maester = Maester, Research, Tech, Technology, "Grand Maester", GrandMaester, GM, R, Res

Chief Builder = Building, Build, "Chief Builder", ChiefBuilder, Builder, Construction, CB, B, Cons, Const

Master of Whisperers= Train, "Troop Train", TroopTrain, "Master of Whisperers", Whisperers, MOW, MasterOfWhisperers, Whisper, Whispers, T, Troop, Whis, TR

Master of Ships= Ship, "Master of Ship", "Master of Ships", MasterOfShip, MasterOfShips, Speed, March, "March Speed", MarchSpeed, Gather, S, Gathering, MOS

Lord Commander= "Lord Commander", LordCommander, Lord, Commander, LC, L

You don't have to use any alias for secondary buff requests (CCS buffs) and the pure text will show up.

### Done (for Players when they are done with the buff)

Players can remove their requests whenever they want using this function.

```markdown
/done (buff (optional))
```

If a certain buff is mentioned, the request for that gets removed, otherwise all submitted requests get removed.

### Use (for PO after they assigned a buff)

A protocol officer can use this function to mention the player on top of the queue that they assigned the buff to them in game.

```markdown
/use (buff)
```

Note: Mentioning the buff is not optional for this command.

### Next (for PO to skip someone in a queue)

A protocol officer can use this function to skip the person who is in top of the queue right now:

```markdown
/next (buff)
```

Note: Mentioning the buff is not optional for this command.

### Queue (for everyone!)

Using this function you can see a priview of the current queue!

```markdown
/queue
```

### Clear Queue (for PO)

Using this function a PO can clear a specific buff queue or all buffs queues at the same time

```markdown
/clear-queue (buff (Optional))
```

### Lock/Unlock Queue (for PO)

When a buff queue is locked, it wont show up in queue and no one can submit a request for that buff with /need function. Also /done /next and /use wont work for that buff.

All POs (with a server role called PO) are allowed to lock/unlock buffs with following commands:

```markdown
/lock (buff (Optional))
/unlock (buff (Optional))
```

If no buff is mentioned all queues will get locked/unlocked together.

Lord Commander is the only queue that's locked by default.


### PO summary

This command can be used to check the PO activities on the channel for a set period of time.

```markdown
/po-summary (since) (till (Optional)) (sort_by_request_count (Optional))
```

Output is a summary of all POs online time and total requests since "Today minus (since)"  till "Today minus (till)" forexample "/po-summary since:4 till:1" will give you a list since 4 days ago till 1 day ago. If you don't include (till) it will return the list till today.

By default the output is sorted based on total active time. add "sort_by_request_count:True" to function so it sorts the list based on total request count.


### Multi-Queueing Settings (for PO)

 If its enabled, players can submit their buff request in multiple queues at the same time (they still cant submit in each queue more than once).

All POs (with a server role called PO) are allowed to enable/disable this option using the following command:

```markdown
/multi-queue
```

### Offline Queueing Settings (for PO)

If no PO is marked as active PO and offline queueing is disabled for the requested buff, the bot will return an error instead of submitting the request in that certain queue (when people use /need function).

If offline queueing is active, the bot will mention a warning reminding people that there are no active PO, but will submit their request. Whenever a PO becomes an Active PO (using /activate), the top of all queues will be reminded to them so they can assign buffs.

All POs (with a server role called PO) are allowed to enable/disable this option using the following command:

```markdown
/offline-queue (buff (optional))
```

### Automated Queueing Settings (for PO)

Automated queueing means, when activated, the queues will jump forward (to next person in list) after some time is passed. This function is specially usable when a Tyrion event is up or queue is busy.

You can use set time function to setup the time between each jump:

```markdown
/set-time (time) (buff (Optional))
```

Time is based on minutes. If Buff name is not mentioned it will set the time similarly for all buff queues in same manner. Default time is 2 minutes. (time) must be an integer 0<x<61.

POs can activate or deactivate the automated queuing with /auto function anytime:

```markdown
/auto (buff (Optional)) (type (Optional)) 
```

Types are:
0: Automated queuing is disabled. POs must manually use -next or players must announce /done before Winter announces next person.
1: Automated queuing is enabled and is attached to "/use" function. Time for each person starts only after PO asks them to use the buff with use function.
2: Automated queuing is enabled but is not attached to "/use" function. Time starts whenever PO is asked by Winter, to give someone the buff.

Notes:
- The default type is 0 (disabled). If the type is not specified the auto function changes between 0 (disable) and 1 (enable and attached to use function).
- You have to define the type if you want to define the auto function for a certain buff queue. for example "/auto buff:gm" is wrong you must use "/auto type:1 buff:gm"
- If no specific buff queue is mentioned, all queues will share the automated queue setting.

Simply calling "/auto" will activate automated queuing mode 1 (enabled and attached to use function) for all queues. If an automated queuing is already active, using "/auto" will disable all.

### AFK (for PO)

Will announce to any future requestors that PO is away from keyboard. Using any commands by them will break this state.


```markdown
/afk
```

They can also use the following command to announce they are back:

```markdown
/back
```


**[Become My Patron](https://www.patreon.com/winterbot)**

## Bubble Reminder

Note: Non patrons can only have one active reminder.
Light patrons can have up to 3 active reminders.
Veteran Patrons and higher can have unlimited amount of reminders.

```markdown
-bubble (type) (hour) (minute (Optional)) (day (Optional)) (loop_each (Optional)) (threshold (Optional)) (comment (Optional)
```

You can input time as:
) hour
) hour:minute
) day:hour:minute
with optional hour and minute paramters

Pay attention that this function doesnt support seconds.

type 1: "in"
Will remind you to bubble after "time - threshold" from now (bubble in 10 hours for example translates to "/bubble type:in hour:10"

Threshold determines how many minutes earlier than your specified Time, the bot should notify you. Default Threshold is 5 minutes. Threshold must be written in minutes.

type 2: "at"
Will remind you for bubble at the time you specified. Threshold is in minutes and shows how much earlier than the time you specified you want to be mentioned. Default Threshold is 5 minutes.

The number of days will be added to current date, but the bot will announce the notify in specified hour/minutes.

For example lets say its 1/25 12:00:

/bubble type:at hour:5 day:2 minute:12

Will mention you at 1/27 5:07:-- (Seconds not important) the reason its not at min 12 is because the default threshold is 5 minutes.

This following types are only available to patrons: (1$ and higher)

type 3: daily

Exactly like "at" function for first notification. Then the bot will automatically notify you each 24 hours.

type 4: each

Exactly like "at" function for first notification. Then the bot will automatically notify you each (hour) hours. Its mandatory for this option to add (loop_each) paramter in hours to determine the cycle of the loop.

There are other bubble reminder related commands:

```markdown
/bubble-list
```

Shows a list of all current reminders set for you.

```markdown
/bubble-remove (id (Optional))
```

Removed all bubble reminders set for you. If an ID is specificed only will remove that reminder. You can see reminder IDs using the list command above.



### Setup Bubble Reminder channel

Patrons of Elite (10$ or higher) can setup one and only one bubble reminder channel to allow all players to fully use bubble reminder functions that are mentioned above to reduce the restrictions..

```markdown
/setup-bubble
```

Daily and Each functions will be available in a bubble reminder channel. Players will be able to have up to 5 reminders in that channel instead of normal restrictions.


**[Become My Patron](https://www.patreon.com/winterbot)**

## Protectors and Alts database

### Protector

You can let winter know your protector in any server.

```markdown
/add-protector (name) (protecting_of (Optional)
```

Add a protector for yourself. name can be a mention, multiple mentions or simple text. You can only have protector data on one server. If you use this function again your previous data gets wiped. 

Admins of a server can use (protecting_of) paramter to write protector of another player in same server as long as they don't have  protector detail in another server saved.

```markdown
/search-protector (mention)
```

Mention the player your searching for their protector information. This information will show if the person saved info on same discord server and will ping whoever was set to be mentioned.

```markdown
/remove-protector
```

Removes your saved protector information

### Setup Alts

Each patron of 10$ (Elite) or higher can setup one channel for saving alts information.

```markdown
/setup-alts
```

All players will be able to use this channel to save their alts and everyone will be able to use that channel to search in the saved information (to figure out whose alt is this or that).

Each patron can only have one channel. You can use -setupalt on a new channel and it will expire the credential for your old channels. The data on previous servers wont be deleted however.

### Alts

After an alts channel is setup players can save their alts information (limited to 20 alts per player atm)

```markdown
/add-alt (name) (type (Optional)
```

for example "/add-alt name:"Winter Angel" type:"Fighter" will add Winter Angel as my alt with a tag "Fighter". Tags are optional and can be used for categorizing alts or leaving a message/note for each.

Players can search for others alts:

```markdown
/search-alt (name)
```

or can list all their alts (or others alts if the optional field is filled):

```markdown
/list-alt (mention (Optional))
```

Also with following command, they can remove a certain alt from their own list or all the alts:

```markdown
/remove-alt (name (Optioanl)) (all (Optioanl)
```

**[Become My Patron](https://www.patreon.com/winterbot)**


## Information/Calulation Functions

### Troop

Information about troops.

```markdown
/troop (type) (tier (Optional)) (count (Optional)) (speed (Optional)) (reductio (Optional))
```

- (count) is for troop count.
- (speed) is for troop train speed buff. You can see yours in your lord details page.
- (reduction) is for Cost reduction buff. You can see yours in your lord details page.

Values for speed (train speed) and reduction (cost reduction) must be input as they are percents. (forexample for 300% troop train buff you should write "speed:300")

### Building

Information about buildings.

```markdown
/building (name)
```

**[Become My Patron](https://www.patreon.com/winterbot)**
