#Prism

*An incredible plugin for rollbacks, restores, and more.*

Prism is the ultimate grief management (rollbacks, restores, etc) plugin for your Bukkit server. It's amazingly fast, versatile, and a pleasure to use. Prism tracks 59+ events, boasts a vastly superior rollback engine, and offers tons of extra features. 

Prism is truly in a class of its own.


![Prism](http://dhmc.us.s3.amazonaws.com/prism.jpg)

### Users Say

"Just switched from CoreProtect to this. Totally worth it."

"The plugin is nuts. Switched over from LogBlock now and never looking back."

"This is definetly the best rollback plugin I have used"

"I love this plugin! Seemed so hard at first, then I used it."

## Official Website & Documentation

- [Official Site - Wiki, WebUI, Import Scripts, etc (discover-prism.com)](http://discover-prism.com/ )
- [Installation & Permissions](http://discover-prism.com/wiki/view/installation/)
- [Commands](http://discover-prism.com/wiki/view/commands/)
- [Troubleshooting](http://discover-prism.com/wiki/view/troubleshooting/)
- [Contribute](https://github.com/prism/Prism )
- [Get Help - IRC - irc.esper.net #prism](http://webchat.esper.net/?channels=prism)
- [Prism Bug Tracker](https://snowy-evening.com/botsko/prism/ )


## Some Videos

[Intro & Demo Video (Pre-Beta)](http://www.youtube.com/watch?v=3b6DQQvBp30)

[Video Tutorial 1: Lookups](http://www.youtube.com/watch?v=W8DpqKiiSJs)

[Video Tutorial 2: Rollbacks](http://www.youtube.com/watch?v=IRr-4r_LS2I)

[Video Tutorial 3: More on Rollbacks](http://www.youtube.com/watch?v=oHBXYzv7vWs)

## Donate to Vive


[![alt text][2]][1]

  [1]: https://www.paypal.com/cgi-bin/webscr?return=http%3A%2F%2Fdev.bukkit.org%2Fserver-mods%2Fprism%2F&cn=Add+special+instructions+to+the+addon+author%28s%29&business=botsko%40gmail.com&bn=PP-DonationsBF%3Abtn_donateCC_LG.gif%3ANonHosted&cancel_return=http%3A%2F%2Fdev.bukkit.org%2Fserver-mods%2Fprism%2F&lc=US&item_name=Prism+%28from+Bukkit.org%29&cmd=_donations&rm=1&no_shipping=1&currency_code=USD
  [2]: http://botsko.s3.amazonaws.com/paypal_donate.gif

Hey, I'm **viveleroi** and I'm responsible for 99% of Prism, the WebUI, the website, the documentation, responding to comments, IRC, and snowy tickets. But I also have a job and a family. Prism, and the rest of my plugins take an incalculable amount of time and that's hard to manage without any pay.

So please, *make a donation and make it easier for me to continue with these amazing plugins*.

## Features Overview

- Prism tracks 60 (and growing) different player, entity, and world events.
- Multiple tools and commands let you see exactly what happened.
- Rollback or restore events directly, or with a safer preview mode first.
- Extremely configurable
- Works for Bukkit, Spigot, MCPC+, Tekkit, etc - handles as best as possible on modded server
- Safe command defaults, very clean and fun to use chat messages.
- Smartest rollback/restore engine ever.
- A dozen extra grief management features that *NO* other rollback plugin has.
- Extremely fast. Takes a pounding. 
- Extremely configurable.
- Dozens of extra features you don't get from other plugins.
- **Requires MySQL** for best performance. sqlite support immature, but available and stable.

## Features Detail

### Events and Lookup

- Tracks 60+ player, entity, and world events.
- Includes block changes, container access, item inserts/remove/pickups/drops, entity deaths, shearing, and a LOT more.
- Related events tracked to causing player, like blocks falling, blocks detaching, trees growing, and much more.
- Smart logging and rollback of important related data like sign text, sheep color, wolf owner, animal age, villager profession, etc
- Tracks liquid flow and items that break because of it
- Tracks world edits (Beta2-17+, requires world edit 5.4.5+)
- Fine-tuned config allows you to control tracking of every single one.
- Incredibly powerful config/personalization system for all wands - set the mode, item, even allow users to personalize how their own wands work.
- Inspector wand allows you to find history for single blocks/spaces.
- Near command finds recent events around you.
- Lookup command is extremely powerful with our versatile parameters.
- Action names also have short-names for easier typing and can combine related actions.
- The radius command also accepts a world edit selection - for any /r/r/p/lookup actions.
- Very clean chat messages and paginated results to ease your burden.

### Rollbacks, Restore, Preview (R/R/P)

- Rollback and restore commands you know and love.
- Rollback or restore directly, or preview changes for _both_ modes first.
- Apply/cancel previews, or let them auto-cancel after a minute.
- Extremely safe default parameters make it harder for you to make mistakes, but can be overridden in-game when you absolutely need them, or can be disable entirely via config.
- You can even rollback killed entities, items taken from containers, and more.
- Sign rollbacks will restore their text (provided we tracked what was written)
- Rollbacks of burn events also extinguish fires.
- Rollbacks of tnt/creeper explosion events also remove the laggy item drops.
- We're CONSTANTLY testing to ensure that rollbacks are smart - problem items like doors, beds, cactus, sugar cane, and more are always restored properly! No half-doors!
- Rollbacks/restores can be alerted to nearby players, and to staff members (staff see actual rollback params).
- Rollback systems moves any players in the way to a safe position on rollback
- Rollback/restore world edits (Beta2-17+, requires world edit 5.4.5+)
- Advanced, optional flags give you ultimate control over the rollback/restore action at command-time.


### Web Search Interface

- Allows you to view/search your data through a website.
- Very clean, modern design makes it an awesome experience.
- We've worked hard to increase performance of the db/queries - databases with millions of records work just fine.
- Optional user authentication support allows you to require people to login before using.

![Prism](http://dhmc.us.s3.amazonaws.com/prism-web.jpg)


### Extra Features

- Alerts for staff when players find natural ores (configurable).
- Alerts for staff when players use flint and steel, place lava.
- Alerts for staff on configurable list of placed/broken blocks (like tnt).
- Alerts for staff for suspected piston xray cheats.
- Put out fires with the extinguish command
- Drain all liquids or just water/lava
- Profile wand shows you data about a block.

### Misc

- Consistently designed chat messages are easy to read, and never spam you.
- All commands are consistent and designed knowing a human will be using them.
- Config allows you to ignore creative mode, or a list of players, worlds, etc.

### Technical

- Multi-threaded queue system for tracking events, combined with a batch recording system makes event recording happen quickly and without impacting your server.
- Block r/r/p are queued for large changes to reduce chances of impacting the main thread.
- Extremely smart database design with a lot of time invested in structure optimization, query performance testing, and more.
- A dev server with 512M RAM, 2.7Ghz dual core processor, 9k blocks from a tnt explosion restored in 1.4 seconds - 1467 milliseconds from command to rollback completion. Most common rollbacks on the same machine tend to take < 200ms to restore. Similar results on relatively equal machines from shared bukkit hosting companies during initial tests.


       
## Get Help

IRC: irc.esper.net #prism

## License 

Attribution-NonCommercial-ShareAlike 3.0 United States

http://creativecommons.org/licenses/by-nc-sa/3.0/us/

           
## Credits

Prism, designed with experience from using competing products on DHMC, and dealing with nearly 19k players in a year and a half. 

- viveleroi (*Creator, Lead Dev*)
- nasonfish (*Contributor*)
- YeaItsMe (*Release QA*)
- nasonfish, Natman93, YeaItsMe, mafoan (*Alpha Testers*)
- mafoan, randox24, tacovan, nehocbelac, Shampoo123, cxmmy14, Palczynski, drac17, ollie2000, PGKxNIGHTMARE, allies333, DocVanNostrand, drfizzman123, 00benallen, rachaelriott, PheonixTamer, YeaItsMe, Natman93, Brazter, sydney2005, rsleight, napalm1, Teh_Fishman, and plenty more from DHMC (*Live Testers on DHMC*)
- WorldEdit block logging [#1](https://github.com/LogBlock/LogBlock/tree/master/src/main/java/de/diddiz/worldedit ) based on work by [Ammaraskar](https://github.com/ammaraskar )
- [Metrics](http://mcstats.org) class Copyright 2011 Tyler Blair. All rights reserved.
- Artwork by [LegendarySoldier](http://legendary-soldier.deviantart.com/


## COMMENTING?

- Do NOT post error logs here. We will delete them.
- **Instead**, make [a paste](http://pste.me) with and show us in [IRC - irc.esper.net #prism](http://webchat.esper.net/?channels=prism) or [file a bug](https://snowy-evening.com/botsko/prism/ )
- If you didn't read the [Troubleshooting](http://discover-prism.com/wiki/view/troubleshooting/) page, we'll delete the comment.
