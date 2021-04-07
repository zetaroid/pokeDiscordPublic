# How To Use and Play PokeDiscord

## Table of Contents
* [Features](#Features)
* [How To Play](#How-To-Play)
* [Game Guide](#Game-Guide)
* [FAQ](#FAQ)
* [Commands](#Commands)
* [Admin ONLY Command](#Admin-Only-Commands)
* [Legendary Calendar for Abandoned Ship](#Legendary-Calendar)
* [Errors](#Errors)

## Features
* Battle, catch, and trade Pokemon from across 7 generations
* Explore the Hoenn region, earn badges, take on Team Magma/Aqua, become the champion, and save the region from despair!
* A full RPG experience
* PVP and matchmaking!
* End game content including: shiny hunting, legendary battles/catching, trading, Battle Tower, and more to come!
* Majority of game is played command free after typing "!start". Interact with the world through emojis.

![PokeDiscord Banner](https://i.imgur.com/Ei2W65P.png)

## Trailer (click the image)
[![link to youtube trailer](https://imgur.com/PQ6co0m)](https://www.youtube.com/watch?v=E7rX2d7W3XI "PokeDiscord Trailer")

## How To Play
* Use command `!start` to start a session
* React to emoji to play the game
* The bot ends your session if you are inactive for a certain amount of time. While you are in battle, this time is 15 minutes, otherwise it is 10 minutes.

## Game Guide
* HELP! I don't know where to go next!?
  * I followed Pokemon Emerald very closely, please see this guide: https://bulbapedia.bulbagarden.net/wiki/Appendix:Emerald_walkthrough
* HELP! Where do I go next and the Emerald strategy guide isn't helping!!!???
  * I just beat my rival on Route 103...
    * The water on Route 103 blocks your path from continuing, head back to Oldale Town and then head west onto Route 102.
  * I just beat the first gym...
    * Head to Route 104 S and go to Dewford Town
  * I just beat the fourth gym....
    * Head back to Petalburg City for the 5th gym (oh...and good luck)
  * I just beat the fifth gym...
    * Go back to Mauville City and continue from Route 118 W to Route 118 E now that you can surf
  * I just got to Lilycove City!
    * Go back to Route 121 and head south to 122 and into Mt. Pyre if you haven't yet
  * I just did Mt. Pyre!
    * Go back to Jagged Pass and enter the Magma Hideout
  * I just did the Magma Hideout!
    * Go to Lilycove City and enter the Aqua Hideout!
  * I just beat the Mossdeep Gym but don't know what to do next!
    * Optional: Take down team Magma for good in the Space Center
    * Mandatory: Follow Team Aqua to route 128, go under, and go to Seafloor Cavern to stop them
  * I just beat Team Aqua in Seafloor Cavern!
    * Go to Sootopolis City (route 126, dive, then back up)
  * I just beat the Cave of Origin!
    * Go to Sky Pillar (from Sootopolis -> Route 126 -> 127 -> ... -> 131 -> Sky Pillar)
  * I just beat Sky Pillar!
    * Go back to Sootopolis and take on the 8th gym
  * I just beat the 8th gym!
    * Go to Route 128 and head for Ever Grande City and the Pokemon League
  * I beat the elite 4...now what?
    * Shiny hunt (1/100 odds, wow!)
    * Altering Cave (exchange 10 BP to change the Pokemon to any non-legendary!)
    * Catch legendaries (hint: check out Slateport Harbor, Route 115, Route 127, Route 134, and Route 108)
    * Gym leader rematches (lv 70 and lv 100)
    * Take on a harder elite 4 for an extra challenge
    * Battle Tower (go to Slateport Harbor -> Battle Frontier -> Battle Tower)

## FAQ
* How long did this take to make?
  * Two weeks worth of my time outside of work and sleep for the base. Then another three weeks to flesh it out.
* Will PVP be added?
  * Probably not, I made a mess of the battle code and not sure it's feasible.
* What is stamina?
  * Stamina is a feature disabled by default, but can be enabled by server admins.
  * With stamina enabled, making progress on a route or entering a battle will consume 1 stamina.
  * Stamina refreshes at midnight PST daily or can be bought for $2000 Pokedollars per stamina.
* Can you add gen4-7 Pokemon?
  * Not immediately evident, but I already did! Game is based on Emerald so you can't catch gen 4-7 Pokemon until post-game. You can find them in Altering Cave and can alter the Pokemon there with '!setAlteringCave' in exchange for 10 BP (BP is earned at the Battle Tower).
* Can you add gen8 Pokemon?
  * No
* Is there a move relearner/TM's?
  * Lilycove City has both.
* Can X be added?
  * Idk, ask me though!
* Why doesn't [insert move here] work as intended?
  * Because I didn't implement it. If you want it to work bad enough, shoot me a message.
* HELP! My game is really laggy!
  * I blame Discord. Or Notch from Minecraft. But most likely Discord's fault.
* What is the shiny rate?
  * 1/100, and yes trainers can have shiny Pokemon (I'm sorry).
* Can I catch legendaries?
  * Yes. And you can shiny hunt them.
* How do I save?
  * Game autosaves.

## Commands:
* `!start` (alias: !s)
  * start a new session. Will be active until AFK for 10 minutes (15 minutes in battle).
* `!guide`
  * links to this guide
* `!map`
  * displays region map
* `!nickname [party number] [nickname]` (alias: !nn)
  * sets a Pokemon's nickname
  * example: "!nn 3 Kippy" = rename Pokemon in slot 3 in party to "Kippy"
* `!swapMoves [party number] [move slot 1] [move slot 2]` (alias: !sm)
  * swaps two of a Pokemon's move slots
  * example: "!sm 3 2 4" = swaps moves in slot 2 and 4 for Pokemon in slot 3 of party
* `!moveInfo [move name]` (alias: !mi)
  * displays information about a move
  * example: "!mi Tackle" = displays info for the move "Tackle"
* `!profile [user]` (alias: !p)
  * displays a trainer's profile
  * example: "!p @user"
* `!trainerCard [user]` (alias: !tc)
  * displays a trainer's trainer card
  * example: "!tc @user"
* `!fly [location]` (alias: !f)
  * fly to a given location
  * example: "!f Littleroot Town"
  * *MUST HAVE BEEN TO THE LOCATION AND MUST HAVE RECEIVED HM FLY*
* `!trade [your party number to trade] [user to trade with]` (alias: !t)
  * trade with another trainer on the server
  * example: "!t 2 @user" = requests a trade with the Pokemon in party slot 2 with @user
  * follow the bot's prompts to confirm trade
  * *YOU CAN ONLY TRADE WHEN A SESSION IS NOT ACTIVE*
* `!getStamina [amount]` (alias: !gs)
  * trade 2000 Pokedollars for 1 stamina (in stamina enabled server only)
  * example: "!gs 2" = grants 2 stamina at a cost of $4000
* `!battle [user]` (alias: !b)
  * battle another trainer on the server, other user must also use this command
  * example: "!battle @user" = starts battle with user, other user must also use this command
* `!pvp`
  * match-make to find another user to PVP with
* `!battleCopy [user]`
  * battle an NPC copy of a trainer on the server
  * example: "!battleTrainer @user"
* `!evolve [party number] [optional: pokemon to evolve into]`
  * evolves a Pokemon capable of evolution
  * example: "!evolve 2" = evolves the 2nd slot in your party if able to evolve
  * example 2: "!evolve 2 Gallade" = evolves 2nd slot in your party into 'Gallade' if possible
* `!unevolve`
  * unevolves a Pokemon capable of un-evolution
  * example: "!unevolve 2" = unevolves the 2nd slot in your party if able to unevolve
* `!setAlteringCave [Pokemon name]`
  * set the Pokemon in Altering Cave to any non-legendary for 10 BP (earned from Battle Tower)
  * example: "!setAlteringCave Tyranitar" = sets Altering Cave to spawn Tyranitar at the cost of 10 BP (BP earned from Battle Tower)
* `!resetSave`
  * resets your save file PERMANENTLY
  * will prompt for confirmation before deleting
  * example: !resetSave
* `!endSession` (alias: !es)
  * ends your current seession
  * can only be used while in the overworld (not in battle or other menus)
  * example: !endSession

## Admin Only Commands
* `!disableStamina`
  * disables the stamina system for the server
* `!enableStamina`
  * enables the stamina system for the server
* `!grantItem [item] [amount] [trainer name]`
  * grants a given trainer an item in specifed amount
  * if item has spaces, replace with '\_'
  * example: "!grantItem Pokeball 2 @zetaroid" = grants zetaroid 2x Pokeball
  * example 2: "!grantItem Hyper_Potion 1 @zetaroid" = grants zetaroid 1 Hyper Potion
* `!removeItem [item] [amount] [trainer name]`
  * grants a given trainer an item in specifed amount
  * if item has spaces, replace with '\_'
  * example: "!removeItem Pokeball 2 @zetaroid" = removes 2x Pokeball from zetaroid
  * example 2: "!removeItem Hyper_Potion 1 @zetaroid" = removes 1 Hyper Potion from zetaroid
* `!grantStamina [amount] [trainer name]`
  * grants a given trainer stamina in specifed amount
  * example: "!grantStamina 2 @zetaroid" = grants zetaroid 2x stamina
* `!setLocation [user] [location]`
  * forcibly sets a players location (recommended to use when they do NOT have an open session, must use Discord name and NOT server name)
  * example: "!setLocation @zetaroid Littleroot Town" = sets zetaroid's location to Littleroot Town
* `!forceEndSession [user]`
  * forcibly removes as user from the active session list (does not actually end the session)
  * this command is to be used only if a user can no longer start a session after 5 minutes have passed (ie. something went really wrong)
  * example: "!forceEndSession user#1234"

## Legendary Calendar
* for post-game Mysterious Portal in Abandoned Ship off of Route 108
### Even Months
![even months](https://i.imgur.com/5QVxaeP.png)
### Odd Months
![odd months](https://i.imgur.com/SdNXuns.png)

## Errors
* For support and reporting errors, please use the "support" channel in the [support server](https://discord.gg/HwYME4Vwj9)
* If the game crashes and you are unable to start again after 5 minutes have passed, the game is borked for you and the developer will have to fix it.
* If the game crashes, an error message will be sent. Please report this to the developer.
* If you see Missingno...this is an error.
* If you see a wild level 100 Rayquaza, that is an error! Please let the developer know how this happened.
![Rayquaza Error](https://i.imgur.com/oujR9ek.png)
