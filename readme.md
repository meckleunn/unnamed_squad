# Unnamed Squad Server Documentation & Admin Guide
This is a general information repository for all things Unnamed Servers.

Admins should utilize this information to conduct their responsibilities / processes while managing the squad server.

Note that these commands will not work for regular players, who do not have an administration account tied to the server.

## General Player Commands Available
Players have access to the following commands, and their basic function 

- `!profile` provides link to the user profile based on `/profile` used in discord 
- `!onlyfans` provides patreon information
- `!admin` reports to admins 
- `!rules` displays rules locations
- `!discord` displays discord link 
- `!switch` switches player
- `!commands` displays above 
- 
## Server Profile Linking System
To facilitate automation, we have moved to [Squad Whitelister](https://github.com/fantinodavide/Squad_Whitelister)

Our Squad server runs the "Profile" link system, this ties your discord account (& roles) to your squad player account.

#### This is effective for all of the following player class(es)
- Members, Applicants
- Seeding Rewards
- Partnership Clans
-  Whitelist Patreons & Supporters
-  Community Contributors
- Admins [We will still *hardcode* admins into the server]

As of Wednesday, 25 January 2023 18:00 (MST), this will be the only way to gain a whitelist. If you previously had a whitelist, please make sure your profile is linked.

#### Step 1 - Linking your Profile
- To link your profile type `/profile` in any channel
- Press `Link Steam`
#### Step 2 - Login to our Squad Server
- You will be provided code via the message in the command
- Enter the code in our [Squad Server](https://www.battlemetrics.com/servers/squad/16023606) Chat (Press [J] or [K] or [L])
#### Step 3 - Verify your Squad Account is Linked
- The message should be updated, to show your verification and details
- You can check your profile link, in-game by typing `!profile`
- Note this may take a couple tries
#### Step 4 - That's it! 
- Your groups and seeding reward will show on your profile both in game and discord.

# Battlemetrics Basics
All Bans and Warnings, Kicks should be done within the Battlemetrics System so they are logged. This is not only for accountability, but more for other admins to look at the past record on the player. 
## Warning a Player
1. Click the Player Name 
2. `Warn Player` -> Enter Reason 
3. Execute Warning
## Kicking a Player
1. Click the Player Name 
2. `Kick Player` -> Enter Reason 
3. Execute Kick
## Banning a Player 
1. Click the Player Name 
2. `Add Ban`
3. You will be taken to another screen 
	3.1. Do not Edit "Banned on Server" 
	3.2. You may edit "Ban List", `The Unnamed` is our general ban list, `The Unnamed CBL` is community ban list. Note you MUST have evidence (video, or sufficient logs) to proceed with this
4. Leave all defaults 
5. Duration you can set with the drop down or leave blank for `Forever`
6. Reason: Our template is `Kicked for *PUT_REASON_HERE* | {{timeLeft}} | beunnamed.com`, please `put a reason` in `*PUT_REASON_HERE*`
7. Add any notes, however, we also would prefer notes to be added w/ evidence in #ban-evidence located on [Discord](https://discord.com/channels/836985182778556436/995744819295035422)
8. For "Banned Identifiers", please leave the default checked. 
**DO NOT CLICK ANY NAME**
9. Save Ban, the player is now banned for the duration selected

## Banning Players Guide
All player bans **MUST** be on **BATTLEMETRICS**. 

**Banning Players** 
Please read the following information in regards to banning of players, for **time**, **how-to**, **evidence template**. 

***Timeframe Guidelines***
This is up to the discretion of the banning administrator, here's a good guide that you could utilize to help with your banning template. 

**Egregious Banning Reasons** - Permanent Bans 
This can include things like, Racism, Homophobia, Hate Speech, Abusive Language, Slurs, Discrimination, Threats, Pedophilia, anything you would consider "Illegal"

In our server, we also wish to express permanent removal of
- Trolling
- Griefing Allies

**Server Violations** - Admin Discretion, however, here's a template
- `Teamkilling`: Intentional, Permanent 
- `Asset Wasting`: Intentional, 7 Day; Perm; ; Accidental, Day
- `Asset Claim Violations`: Intentional, 3 Day,  7 Day; Perm; Accidental, Kick 
- `Ghosting`: Permanent
- `Racism`: Permanent
- `Sabotage`: Permanent
- `Squad Baiting`: Intentional, 3 Days; 7 days; Perm; Accidental, Kick. Could also always ban them per day per squad created
- `Main Camping`: Warn First, then if they do not move, ban 3 days, if they do move, move on. If its a repeat offense, perm 
- `Helicopter Ramming`:3 Days, 7 Days; Perm 
- `Toxicity`: 3 Days; 7 Days; Perm
- `Seed Rule Violations`: Permanent, they'll just keep coming back and doing it. 
- `No SL Kit`: Demote; Kick; 3 Day; Perm. Admin Discretion, it'll auto demote after 6 minutes
- `Spamming`: 7 days
- `Streamsniping`: Kick, Perm if continued and proveable
- `Advertising`: Kick 
- `Albeism`: Permanent
- `Politics`: 3 Days; 7 Days; Perm 
- `Recruiting`: Kick
- `Glitching / Cheating`: Perm
- `Cheating`: Perm 
- `Mic Spamming`: 1 Day - to - Perm after Warning
- `Not playing objective`: Warn, 3 Days, 7 Days, Perm


**Evidence Template:** Please submit all ban evidence in`#📂︱ban-evidence. `

Every ban should have evidence to back it up, whether it be a log, notes, or video. When they come to appeal, I want all the information available. If you do not have time to submit this afterwards, please just have notes on the ban in battlemetrics. It should be good practice to use discord though. 

### For Community Ban List, we need video evidence / picture evidence

**Note:** If you want the player on the Community ban list, please tag meckle that you have completed a CBL ban selection, or just ping meckle to add in `#📂︱ban-evidence` with the following template, if not we'll just keep them on "The Unnamed" ban list* 

`**Name**`: 
`**SteamID64**`: 
`**Report Info**`: 
`**Description**`:
`**Evidence**`:

### The "Server Protection" Catch All

If you think the player is cheating, or violating server policies without enough evidence, or you name it. Please put the reason as **"Server Protection"**, and leave it as a local ban.

# Admin Commands
All Commands in this subset are to be used by administration staff. If the category marked by `User Commands` then all users (players) can utilize.
## Map Voting
#### User Commands

-   `!vote help`  - sends possbile commands to a player in the from of a warning
-   `!vote choices`  - sends choices to player in the from of a warning
-   `!vote results`  - sends player the results in a warning

#### [](https://github.com/fantinodavide/squad-js-map-vote#admin-commands)Admin Commands

-   `!vote start`  - Starts a vote with 6 layers, random modes
-   `!vote cancel`  - Cancels current round of voting
-   `!vote cancelauto`  - Cancel scheduled automatic start of vote
-   `!vote end`  - Gently ends the current vote and announces the winner layer
-   `!vote restart`  - Restarts voting with 6 random maps and modes
-   `!vote broadcast`  - Broadcasts current voting results - happens every 7m automatically

##### [](https://github.com/fantinodavide/squad-js-map-vote#vote-by-modes)Vote by modes

-   `!vote start *_raas`  - Starts a vote with 6 layers, all RAAS
-   `!vote start *_aas`  - Starts a vote with 6 layers, all AAS
-   `!vote start *_inv`  - Starts a vote with 6 layers, all INV

##### [](https://github.com/fantinodavide/squad-js-map-vote#vote-by-map)Vote by map

-   `!vote start yeh gor lash gor albas`  - Starts a vote with X maps, random modes

##### [](https://github.com/fantinodavide/squad-js-map-vote#vote-by-map--mode-mixed)Vote by map + mode, mixed

-   `!vote start yeh_raas gor_raas lash_inv gor albas_inv`  - Starts a vote with X maps, X modes

## Server Seeding
Joining the server with no population, will [automatically](https://www.battlemetrics.com/rcon/triggers/edit/daa92233-4d8f-4294-9e66-45b2c2de9982) push the server to change to a seeding map. To change this seeding map, please just contact @elijahjohn75 or @meckle to commit. Otherwise, administrators are free to change the seeding map upon the change. 

##### To Change the Maps 
1. Go to Battlemetrics
2. Go to [Servers](https://www.battlemetrics.com/rcon/servers/16023606)
3. Server Commands, press down arrow
4. "Set Next Map" - pick relevant map
5. Server Commands, press down arrow
6. "End Match"

#### Chat Commands
- `!seedrules` No weaponized emplacements allowed while seeding! Refer to the server rules for more info. Do not fob hunt! Do not move radio location in seeding. Avoid building Tarp/Camo net Buildings please.
- `!live` The server is now live! Please play out the map, and the next map will roll quickly! Thanks for seeding, visit us at theunnamedcorp.com
- `!tarps` While in seeding, please do not build observation towers, or hasco bunkers completely near central point. These tarped buildings are not fun for everyone, and can cause negative user feedback. Thank you for understanding
- `!thanksseed` Thanks for helping us seed! Visit theunnamedcorp.com if you want to become a regular, and gain whitelist!
- `!seedlink` Thank you for helping us seed! If you connect your profile on our Discord to your Steam ID, you can gain seeding rewards for playing here! beunnamed.com
#### User Commands
- `!seeding` *Warns Player*
	- While on a seeding map, please do not build observation towers, hasco bunkers, weaponized emplacements.
	- Fight over the middle points during seeding!
	- View our rules on our website or discord
## Admin Notifcation System
The [Admin notification](https://www.battlemetrics.com/rcon/triggers/edit/a826fadf-f4b0-4101-b111-da2e0cb4b2c4) system is a battlemetrics, squadJS triggers system utilized to alert administrators to a players request
#### User Commands
-`!admin` *[Request]* 

#### Automated Responses
 - `!admin` [With Message]
	- Warns Player
		- To expedite the process, please bring evidence to our discord.
		- If no response, request admin on discord in create-a-ticket
	- Logs Message on Battle Metrics `#ff9900`
		- "Admin Requested" applies `#ff9900`
	- Webhooks 
		- Discord Ping to protocol
		- application/json
		- Errors - Logs Only Errors 
```json
{
    "embeds":[
      {
            "title": "Battlemetrics Information : Admin Ping",
            "description":"**Name**: [{{player.name}}](https://www.battlemetrics.com/rcon/players/{{player.id}}) \n**Steam**: [{{player.steamID}}](https://steamcommunity.com/profiles/{{player.steamID}}) \n**Time Played (Server)**: {{player.server.timePlayed}}, \n**Message Body**: {{msg.body}} \n**Said in channel**: {{msg.channel}}",
            "color": 15844367,
            "timestamp": "{{timestamp.iso8601}}",
            "footer": {
              "icon_url": "https://i.imgur.com/pl43WhK.png",
              "text": "I am a bot, beep boop "
            },
            "thumbnail": {
                "url": "https://i.imgur.com/pl43WhK.png"
            }
            
        }
    ] 
}
```
##### Continued
 - Player Warning Flag > Trusted Reporter 
	 - If Player has Player Flag `Trusted Reporter`, then 
```json
{
    "embeds":[
      {
            "title": "Player is a Trusted Reporter",
            "description":"**Name**: [{{player.name}}](https://www.battlemetrics.com/rcon/players/{{player.id}}) \n**Steam**: [{{player.steamID}}](https://steamcommunity.com/profiles/{{player.steamID}}) \n **Is deemed to be trust worthy by admins** ",
            "color": 15844367,
            "timestamp": "{{timestamp.iso8601}}",
            "footer": {
              "icon_url": "https://i.imgur.com/pl43WhK.png",
              "text": "Battlemetrics Admin Service"
            },
            "thumbnail": {
                "url": "https://i.imgur.com/DNQWdNU.png"
            }
            
        }
    ] 
}
```
#### Automated Messages [cont'd]
 - If the player utilizes `!admin` and does not reflect continued wording [exact match], then the player will be warned with a response to add wording
##### Black Listing Automation
- Squad JS will ignore the warning if the message contains `switch` anywhere within the statement. Battlemetrics will **still** log the incident for recording reasons, but admins will not be pinged via the webhook

## Server Rules Automation and Chat Enforcement

Server Rules are available in the Message of the Day, on the [Unnamed Website](http://theunnamedcorp.com/squad.html#sqserverrules) and in our [Discord](https://discord.com/channels/836985182778556436/1063890894455054426). *Players have no excuse to not find our rules.*

For our most convuluded rules, here are some more enhanced admin direction these following incident types.
### Claims Enforcement 
Our squad utilizes squad claims to manage team cohesion. Many servers run first-come-first-served basis, **we are not one of them.**
#### Chat Commands
- `!claims`  Responds with three global chat responses based on [trigger](https://www.battlemetrics.com/rcon/triggers/edit/bd3cb7e7-7e9c-43a5-8946-f0bf5363bd07)
	- Vehicles are done by Squad Names! Please read our rules at: theunnamedcorp.com. First named squad has priority. Discord has a list of all acceptable names.
	- Squads must be named after the vehicle name/type, and can claim multiple of the SAME assets (example LAV-25 can claim 2x LAV-25 if 6 crew, TANK = Tank Squad, etc.) 
	- Squads named "ARMOR" have no claims here and are forbidden, please utilize 1 vehicle type only. 
- `!dual` Squads can not claim 2 different vehicle types. Ex: Bradley/Tank

To prevent "Armor" / "Vehicle" squads, the server has a built in [validation service](https://github.com/fantinodavide/squadjs-squad-name-validator)
- Admins can view the log of squad name validations [here](https://discord.com/channels/836985182778556436/1064237320435400726) for any failed responses
- The following is the current regex schema
```regex
/(a ?r ?m ?(?:o|e)? ?u? ?r)|(v ?i ?c)|(v ?e ?h ?i ?c ?l ?e)/gi
```
##### A Robust Vehicle Squad Name Listing is available [here](https://discord.com/channels/836985182778556436/1063890894455054426) 

### Main Camping
Main camping is always a hard topic to deal with, our rules allow for **complete admin discretion** when managing the main camping enforcement rule. It is a good rule of thumb, that if something is not really meant to be there based on game objectives, then they are most likely main camping. 

Rules state that "engaging enemies within an approximate "450m" from their main is considered main camping. This however cannot apply for all maps, therefore your discretion is paramount. 

First step is to "Warn" the player, either verbally or through the in-game warning system. 

#### To Warn a Player utilizing an Automated Flagging System (AFS)
1. Press Servers, select our [server](https://www.battlemetrics.com/rcon/servers/16023606) 
2. Select the Player Name, press the arrow 
3. Select "Main Camping" 
4. You will be asked to confirm the main camp warning, and the server will execute the following warning to the player 
	4.1. `Camping enemy mains is not allowed! Please remove yourself, and all deployed assets`
	4.2. `Failure to comply, will result in removal`
	4.3. Execute Player Flag Added > Main Camp 

#### Chat Command
- `!main` triggers two global chat responses
	- Main Base Camping is defined as positioning assets, infantry, or mines, at any distance, with the intent to destroy enemy assets entering or leaving main. 
	- We deal with Main Base Camping on our server on a case-by-case basis. Admin discretion is final, if there are issues or disagreements, bring them to discord.
- `!minemain` Do not mine, or camp the enemy main! Play the objective!!!

## Teamplay Enforcement
Playing an objective is the main part of squad, it's pretty much the reason for the games existence. To play as a squad  in a group of squads. 

What defines `Teamplay` can be open to interpretation, but here in our server we are looking for the following things: 
1. Supporting an Active Objective, whether it's on RAAS, or Invasion through defending, or attacking those selected points on the map via the in-game system. 
2. Supporting their team through logistical actions 
3. Supporting their team through distanced based armor support
4. Supporting their team through setting up mortar fobs 
5. Supporting their team that is in any justifiable way supporting their team, it's pretty obvious

#### What Isn't Teamplay 

6. Actively pushing off the flag into areas way off the main objective 
7. Camping mains 
8. Taking a full squad of 9+ guys into nowhere to go "Fob Hunting" or actively play off objectives, with some dumb flank scheme that makes no sense 
9. TOW Fobs with a full squad of 9 people for essentially what is 1 asset by 1 person. 
Use your discretion, we have an Auto Flag for Teamplay that tells the player `Your team needs you! Please play active objectives!` 

### Chat Commands
- `!teamplay` prompts two global chat messages 
	- This is a teamplay server, follow objectives, communicate, play together. Listen to your commander.
	- Failure to abide by this, can result in your removal.
- `!ptfo` Play the ACTIVE objective!!

## Squad Leaders
Either the most beneficial or damning thing to a team are squad leaders. 

**Our squad leaders must:**
1. Have a microphone 
2. Have a squad leader kit 
3. Must not lead a free kit squad, which essentially means no direction - "DO WHATEVER YOU WANT" 

### Chat Commands
- `!sl` Squad Leads must have a Squad Leader Kit, Microphone. They must lead their squad.
- `!lead` prompts two global chat messages 
	- You must lead the squad you create, lock the squad at appropriate players for your assets if necessary. 
	- Squads that are not being led, and utilized as a free kit squad will be disbanded.

## General Chat Commands for Admins
- `!afk` 

> All players must join a squad, or will be considered AFK and kicked
> for active players!

- `!tk` 

> Apologize for your Teamkills in All-Chat! [J] Failure to do so, can
> result in removal.

- `!int` 

> Intentional teamkilling of any kind is not tolerated, do not teamkill
> intentionally.

- `!toxic` 

> Toxic behavior will not be tolerated - be respectful to all players on
> the server

- `!language` 

> Abusive Language / Hate Speech is NOT Tolerated, you will be banned.

- `!politics` 

> Please do not discuss politics or other controversial topics in chat!

- `!clearchat` 

> Clear the Global Chat!

- `!ls` 

> No Locked squads under 4 unless named task such as LOGI, VEHICLE_NAME, HELI
> You must unlock your squad when asked by an Admin

- `!ram` 

> No Ramming With Helicopters, or their blades. You will be removed.

- `!bait` 

> Creating a squad you do not intend to lead leads to removal from our
> server. If your squad leader left, please either find a leader or
> disband the squad.

- `!ticket` 

> Do not share ticket info in all chat!

- `!submit` 

> If you are reporting abusive behavior, submit all evidence to our
> discord to expedite the process

- `!ghosting` 

> Ghosting is sharing information to the other team, do not share
> information intentionally. If you are caught sharing information, you
> will be permanently banned.

- `!solo` 

> Do not solo vehicles that require crewman kits to operate!

### Advertising 

- `!clan` 

> Are you a clan looking for a community to call home? Head to our
> discord today, talk to an admin about group whitelisting.

- `!thankyou` 

> Thank you for playing here! Hit up our community at
> theunnamedcorp.com! Feedback welcome!

- `!joindiscord` 

> Join our community today! discord.gg/unnamedcorp! Giveaways,
> Whitelist, Gaming Community, Maplesyrup pics.

- `!recruiting` 

> We're recruiting! Stop by our website at beunnamed.com!

- `!afterparty` 

> Join / Visit our community at beunnamed.com!

- `!enjoy` 

> Enjoying our server? Hop on our discord! Be apart of the community and
> gain whitelist! beunnamed.com

- `!whitelist` 

> Wanting to have a whitelisted slot? Head to our website for more info.
> theunnamedcorp.com

- `!fwl` 

> Do you SL or Command often?! We take note! You can get free whitelist,
> join our discord to learn more.

## Discord Channels Explained
*You may not have access to all of the channels below* 

**We allow you to mute these channels, so you do not get notification spam**

- `log︱maps` holds all map voting bot relations, including map votes called, round ended results, map vote results if duration is before server end 
- `log︱rcon` allows executive admins to directly issue rcon commands via Discord 
- `log︱kill-feed` all kills are logged, based on 
	- Attacker Name
	- Attacker Steam ID
	- Weapon
	- Victim Name 
	- Victim Steam ID
	- Community Ban List Link for Attacker
-  `log︱teamkills` all teamkills are logged based on 
	- Attacker Name
	- Attacker Steam ID
	- Weapon
	- Victim Name 
	- Victim Steam ID
	- Community Ban List Link for Attacker
- `log︱cbl` logs all bans added or removed to our community ban list
- `log︱squads` logs all squads created 
- `log︱seeders` logs all seeders who hit 5+ seeds in a month **Channel is Deprecated** 
- `log︱whitelists` logs all whitelist submissions **Channel is Deprecated due to Whitelister Activation**
- `log︱fob-explo` logs explosions on hab entities, not always great tool but it works when it needs to.... I guess? Kinda buggy. 
- `log︱sq-validator` will log all squads that are automatically disbanded due to forbidden wording

## Community Ban List Documentation 
For Banning Reasons, we need to have a like match to these banning reasons when submitting a ban. If the convention is not followed, it will come back with *Unknown*. 


**Ban Reasons**

``` Cheating: /cheat|hack|作弊|\bhile|trich|betr(ü|u)/i,
  Glitching: /glitch/i,
  Exploiting: /exploit|剝削|istismar|ausnutz/i,

  Teamkilling: /team ?kill|\btk|ITK|[0-9]x?tk|int?tk|team(be|ab)schuss/i,

  Trolling: /troll/i,
  Griefing: /gr(ie|ei)f/i,
  'Wasting Assets':
    /destroying assets|wast(e|ing)|taxi|israf|(friendly|dost) (asset|fob|hab)|sabotage|asset destruct|zerstör|verschwend|eigene(s)? (radio|fob|vehikel|fahrzeug|hab|hub)/i,
  Ghosting: /ghosting/i,

  Toxic:
    /disrespect|flam(e|ing)|har(r)?as(s)?|insult|language|offensive|rude|toxic|sayg(i|ı)s(i|ı)z|hakaret|irrespect|respektlos|beleidig(ung|en)/i,
  'Abusive Language/Hate Speech':
    /abusive|bigot|derogatory|discriminat|hate ?spe(e|a)ch|(homo|trans)(-| )?phobi|nazi|racial|rac(si|is)m|racist|sexism|sexist|(küfür|kufur)|mal(é|e)diction|種族主義|fluchen|semitism|nigg(a|er)|fag|slur|swastika|schimpfw(o|ö)rt|rassis(t|m)|missbr(a|ä)uch|(f|n)(-| )?(word|bomb)/i,

  AFK: /afk|unassigned/i,
  'Breaking Seeding Rules': /seed/i,
  'Breaking Vehicle Priority Rules':
    /priority|(ara(ç|c) (kural|ihlali))|(vic|vehicle|asset) (name )?claim|claim rule|ignor(ing|ed) claim/i,
  Camping: /camping|min(e|ing)/i,
  'Current or Recent VAC Ban': /vac ban/i,
  'Discussing politics': /politi(c|k|s)|siyaset/i,
  'Helicopter Ramming': /(ge)?ramm(ing|en|t)/i,
  Hindering: /(be|ver)?hinder(ing|ed|t|ung)/i,
  Impersonation: /impersonat|ausge(ge)?ben/i,
  'Locked Squad': /(locked|geschlossenes) squad/i,
  'No SL Kit': /sl kit/i,
  Recruiting: /recruiting|rekrutier/i,
  'Soloing Vehicles': /crewman|manning|solo|(1|one)(-| )?man/i,
  Spamming: /spam/i,
  'Squad Baiting':
    /bai(t|ting)|creat(?:ed?|ing)(?: a)? squad|pass sl|lead it|(of|to) lead|pas(s|sing)( |-)?SL/i,
  'Stealing Assets': /steal|çalma|(ge)?st(e|o)hlen/i,
  Streamsniping: /streamsniping|yayinc(i|ı)/i,
  'Sharing team info':
    /shar(e|ing) (ticket|team|hab|fob|info|game|enemy)|ticket (count|sharing)|(info|intel) shar(e|ing)/i,
  Advertising: /advertising|werb(ung|en)/i,
  Ableism: /ableis(t|m)/i```
```

## Appeal Structure


**User Appeals** 
1. If user is apologetic, and genuine: Remove Ban 
2. If user is an assclown, and it is a timed ban: Leave timed ban 
3. If user decides to become hostile in tickets: Perm ban, submit transcript in Evidence to upgrade ban to permanent from all services 
4. If user threatens server in tickets: Perm ban, remove from services, submit evidence to Offworld Industries

Banning Admin may be tagged in tickets, all admins have access to appeal tickets now. Tickets are tagged as 

```ban-user-####```

