A big one: mail, the Compendium, the Tracker, sounds, the map in words, new map tools, new vitals arrangements and a new layout, and the fixes from your reports on 0.9.3. Thank you!

**Download:** Geas-Mushclient.zip below. Updating: close MUSHclient, unzip and drag the six folders into your MUSHclient folder again (Replace): this version adds **sounds** and **geas_settings**. Your settings and maps are kept. Open your world; new plugins are added by themselves (save the world when it says so).

## New
- **The Geas menu** (#69): the package's own right-click menus: no item limit, long lists scroll, and `gm` lists any window's menu as numbered text (`gm map`, `gm map find inn`), for the keyboard and screen readers.
- **Sounds** (#82): a sound for game events (tells, hits, low health, exits ...), ambience by area, your own sounds for any line, and sound packs. Silent until you put WAV files in `sounds\geas\default\` (none are shipped). `geas sound`.
- **Settings export and import** (#84): all your package settings to one file and back (another PC, a new character).
- **Mail helper** (#83): write mail in a window and send it safely, line by line; read, reply, forward, and keep mail.
- **The Compendium** (#90): your texts in folders (sermons, songs, notes, books), sent safely into the game's editor. **People and Journal** (#87): notes on the people you meet and a journal.
- **The map in words** (#89): `map words` describes your surroundings: the landscape, roads, services and areas nearby. The Map window can show the words instead of the drawing.
- **Missile and thrown weapons** (#85): Load, Shoot and Unload buttons for a wielded bow, crossbow, sling or blowpipe; your ammunition counted, with a warning when it runs low; Collect after a fight; thrown weapons to get back.
- **The Tracker**: playtime and what you do over time: kills, skill-ups, stat gains, explore points, deaths, fights, combat lines, missiles, miracles and spells, rooms and areas. Reports by command (`geas data kills last 12 months by week`) and in a window with tables and graphs (columns, bars, a line; rates per hour played), export to CSV or TXT for Excel or Google Sheets, Copy table, and backups. `geas data help`.
- **Armour**: what covers each body part, under Protection.
- **Map, off the map** (#92): trees, the Grimlock mine and the swamp are no longer stored as one shared room (walks used it as a shortcut, and ended in the wrong place). The map says where you are (Aside, Uncharted or Lost) and picks up again on the next real room.
- **Map, custom exits in one command**: `geas map cexit <commands>` runs them and links the room you arrive in. Exits can be drawn as another direction, solid or dotted, with or without a door; typing a direction takes an exit drawn that way.
- **Map, hidden exits**: an exit you found by searching stays on the map, dotted, when the room resets. Give it a reveal command (its menu: Reveal it with...) and walks use it: the command first, then the step.
- **Map, find and go**: `geas map find` lists your marks first, then rooms named so, notes, room names, and each area once (not hundreds of rooms). `geas map go <words>` walks to the best match when there is only one.
- **Map, every exit's length** (Settings > Mapper > Looks) and **terrain colours** in Settings (Mapper > Terrain colours; `geas map colour forest #88cc66`).
- **Stats window**: the text after each bar is any mix of the game's words, level, points and percent; your base compared as points or percent; a "Stat points" line under the rank (total, percent of all possible, change from base); a value above each column; level bands and ticks in the bars (#35).
- **Ability points** (#27): free, used and total in the Stats window, checked quietly at login and every 30 minutes (or only when you type `abilities points`), and an Ability points report in the Tracker.
- **Map, avoid roads** (#49): a road preference for outlaws and sneaking: walks keep off roads and paths when there is another way (tool bar "No roads", `geas map roads avoid`).
- **Vitals arrangements**: upright (vertical) bars; bars per line and lines as rows or columns (health, mana, stamina, fatigue on one row; hunger, thirst, intox, load on the next); the rows in your order; any bar in a window of its own; upright bars as tall as you drag the window. `geas vitals help`.
- **New layout, Stay Awhile**: two tall tabbed panels either side of the game text, with Physical and Mental as upright bars beside it (Settings > Layouts).
- **Your own height for any window**: right-click > Height fits its content (untick it) and drag the bottom edge: the Weapons window, for one, stops growing and shrinking with its alerts.
- **Weapons**: `geas weapons shield on` and `off` for aliases.

## Fixed
- **Vitals** (#91): the window no longer goes stale. Weight and volume update after you get, put or drop things, and vitals are asked for at least every 10 seconds (Settings > GMCP > Refreshing) even when you type nothing, for example in a fight.
- **Blindfolds and dark places**: while you cannot see, the game hides your inventory. The Inventory window keeps the last inventory you saw (with a note), coins stay, and Weapons no longer warns that your weapons "may have been dropped" or that you are out of arrows.
- **Your own highlight triggers** (#79): a highlight on a line's first word no longer makes the line show odd colours.
- **Closing windows while locked** (#80): Settings, the setup guide, the Tracker, Mail and the Compendium keep their x while windows are locked.
- **Settings window** (#74): the list on the left fits its names, can be dragged wider, and scrolls when the window is short.
- **Setup guide**: the window grows with a bigger font (#73); the old-world step is MUSHclient's Import box, and copies your old script file if your old world used one (#76).
- **Settings**: "Stats and skills" (was "Character") (#75); "None yet: Save current as..." in Layouts is a button (#70).
- **Chat log**: the daily file has your name, so two characters' chats do not mix (#72).
- **Map**: the walk to resume can be forgotten (right-click Resume) and is forgotten when you get there another way (#77).
- **Tabs outside their dock** (#78, #57): a docked window found outside its dock is put back within half a second. If you still see it, send a report: it now records what happened.
- **Title bars**: a window whose title bar you hid keeps it hidden after you restart MUSHclient (#68).
- **Line colours**: "You think you sense exits to the ..." in the dark is coloured as room exits.
- **Combat**: a fight ends at once when the last foe was killed; a big kill list imports in a moment; races of more than one word ("pale one") are kept whole.
- **Skills**: skill lines are read whatever their level words hold.
- **Ability points**: a character too young to use them is told so in the Stats window, and the game's answer stays hidden.

## Known
- Room connections can be hard to see in some themes (#81): to be tuned with your feedback.

Something odd? Type `geas report` in MUSHclient and attach the file to a new issue.
