


# Unnamed Server Documentation
This is a general information repository for all things Unnamed Servers.

Admins should utilize this information to conduct their responsibilities / processes while managing the squad server.

Note that these commands will not work for regular players, who do not have an administration account tied to the server.
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
### Claims Enforcement 
Our squad utilizes squad claims to manage team cohesion. Many servers run first-come-first-served basis, **we are not one of them.**
#### Chat Commands
- `!claims`  Responds with three global chat responses based on [trigger](https://www.battlemetrics.com/rcon/triggers/edit/bd3cb7e7-7e9c-43a5-8946-f0bf5363bd07)
	- Vehicles are done by Squad Names! Please read our rules at: theunnamedcorp.com. First named squad has priority. Discord has a list of all acceptable names.
	- Squads must be named after the vehicle name/type, and can claim multiple of the SAME assets (example LAV-25 can claim 2x LAV-25 if 6 crew, TANK = Tank Squad, etc.) 
	- Squads named "ARMOR" have no claims here and are forbidden, please utilize 1 vehicle type only. 

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

## Teamplay Enforcement
Playing an objective is the main part of squad, it's pretty much the reason for the games existence. To play as a squad  in a group of squads. 

What defines `Teamplay` can be open to interpretation, but here in our server we are looking for the following things: 
1. Supporting an Active Objective, whether it's on RAAS, or Invasion through defending, or attacking those selected points on the map via the in-game system. 
2. Supporting their team through logistical actions 
3. Supporting their team through distanced based armor support
4. Supporting their team through setting up mortar fobs 
5. Supporting their team 
