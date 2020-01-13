# About Winter!

Winter Bot is a legal bot made for the game "GOT: Winter is coming" that can help players with a variety of functions on discord.

Winter Bot is made to help players with Protocol officers queuing, offline calculations , game server management, Bubble reminder, Rally calculators, Buff calculators, Pack calculators and etc! Its also going to have a bunch of very cool online games for discord servers!

Most of the functions are free! To be able to make up for the hardware resources and host cost of this bot, and for future development, some are only available for Patreons. Winter needs your help! Join me on this journey and help winter to become the best!

## Support and Contact

Winter has expenses. I need money to be able to work on it properly! become my patreon and support Winter from today!

**[Become My Patreon](https://www.patreon.com/winterbot)**

You can also find Travtools discord channel [here](https://discord.gg/gVA9adu).

## Installation

To install Winter open the following link if you have the permission to do so (Server Management or Admin): [Install Link](https://discordapp.com/api/oauth2/authorize?client_id=626364547539664909&permissions=268435456&scope=bot)

Just choose your server and confirm the captcha and it's done :)

Reminder that you don't need to give Winter the administrator permissions :) Bot needs "Manage roles" permission if you want the Po functions to work properly though!

**[Become My Patreon](https://www.patreon.com/winterbot)**

## Protocol Officing Functions

### Setup a PO channel

Before using the PO functions, a server admin who is a veteran patreon (5$ or higher) must use the following command in the channel they want to setup as po requests channel.

```markdown
-setuppo```

This function is the only po function that is limited only to patreons, meaning after setting up a channel as PO channel, everyone will be able to use the rest of the functions for free unlimitedly.

After activating the channel as a PO channel, bot will send a confirmation message there and announces that it's party time!

**[Become My Patreon](https://www.patreon.com/winterbot)**

### Active/Deactive (for POs)

The players who have a PO role on server can use this following function to announce they are active to give away the buffs.

```markdown
-active```

And when they are going offline they can use the following function to announce they are gone:

```markdown
-deactive```

Winter will automatically mention the "Active PO" whenever its anyones turn to recieve the buff.

Note: To be able to use this function, define a server role called "PO" (caps characters are not important) and give the role to all the people who should have access to this function (that should be able to announce themself as active po)

Note: If you define a server role called "Active PO" (caps characters are not important); the bot will automatically give that server role to the active po and will remove it from them when they go offline. Change the color of that role and click on "Display this role seprately" so when the bot gives the current active po that server role, they show up on top with a different color! pay attention that Winter needs to have Manage Roles permission over that new server role (it needs to be higher in roles list on your roles page in server setting). Ultimately you can give Winter admin permission.

### Need (for Players requesting for buff)

The players can request for a buff using this simple command:

```markdown
-need [buffname]```

That way the bot will assume that their server nickname (display name) is their account name. Or they can request it for someone else (or input their account name manually):

```markdown
-need [buffname] [Account name]```

In this case the bot will mention the person who made the request whenever needed but will ask the Protocol officier to give the buff to the alternative name they provide.

Currently recognized buff aliases are (Not case sensetive):

Grand Measter: "Grand Measter", GrandMeaster, Measter, Research, Tech, Technology, GM
Chief Builder: "Chief Builder", ChiefBuilder, Builder, Build, Building, Construction, CB
Master of Whisperers: "Master of Whisperers", MasterofWhisperers, Whisperers, Train, "Troop Train", TroopTrain, MOW, Whispers, Whisper
Master of Ships: "Ship", "Master of Ship", "Master of Ships", "MasterOfShip", "MasterOfShips", "Speed", "March", "March Speed", "MarchSpeed", "Gather"

![img](https://cdn.discordapp.com/attachments/633666978783166474/666341816177786891/unknown.png)

Note: In image above the active po is also me, so the bot mentions me to ask me to assign the buff.

### Done (for Players when they are done with the buff)

Players can remove their requests whenever they want using this function.

```markdown
-done [buffname (optional)]```

![img](https://cdn.discordapp.com/attachments/633666978783166474/666342361873383434/unknown.png)

### Use (for PO after they assigned a buff)

A protocol officer can use this function to mention the player on top of the queue that they assigned the buff to them in game.

```markdown
-use [buffname]```

Note: Mentioning the buff is not optional.

### Next (for PO to skip someone in a queue)

A protocol officer can use this function to skip the person who is in top of the queue right now:

```markdown
-next [buffname]```

Note: Mentioning the buff is not optional.

### Queue (for everyone!)

Using this function you can see a priview of the current queue!

![img](https://cdn.discordapp.com/attachments/626365897941975052/666345061143019541/unknown.png)

## Information/Calulation Functions

### Troop

Information about troops.

```markdown
-troop [Troop Type] [Troop Tier] (-c [count] (optional))```

-c is for troop count.

![img](https://cdn.discordapp.com/attachments/633666978783166474/666336022816096296/unknown.png)

### Building

Information about buildings.

```markdown
-building [Building Name]```

![img](https://cdn.discordapp.com/attachments/633666978783166474/666336985438224404/unknown.png)

**[Become My Patreon](https://www.patreon.com/winterbot)**
