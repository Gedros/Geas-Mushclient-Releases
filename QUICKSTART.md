# Geas MUSHclient package: quick start

About 10 minutes. You need Windows and an internet connection.

## 1. Install MUSHclient 5.06

1. Download MUSHclient 5.06 from
   https://www.gammon.com.au/downloads/dlmushclient.htm and run the
   installer.
2. When it asks where to install, choose **C:\MUSHclient** rather than
   Program Files. (Windows stops programs saving files inside Program
   Files, and MUSHclient needs to save your maps and settings.)

Already have MUSHclient 5.06? Skip this step.

## 2. Add the package files

1. Download the package:
   https://github.com/Gedros/Geas-Mushclient-Releases/releases/latest/download/Geas-Mushclient.zip
2. Right-click **Geas-Mushclient.zip** > **Extract All...** > **Extract**.
3. In the extracted folder you will see four folders, **worlds**,
   **lua**, **logs** and **reports**, and this guide.
4. Select the four folders and drag them into your MUSHclient folder
   (for example C:\MUSHclient). If Windows asks, choose **Replace the
   files in the destination**.

   This adds the package's files to the folders you already have. Your
   worlds, saved settings, maps and other plugins stay as they are; only
   older copies of the package's own files are replaced.

## 3. Make your Geas world

Choose **A** (quickest) or **B** (your own MUSHclient settings).

### A. Use the ready-made world

1. Open MUSHclient: **File > Open World...**, open the **worlds** folder
   and choose **Geas (new world).mcl**.
2. **Save it under your own name straight away.** The setup guide (below)
   does it for you in step 4, or use **File > Save World Details As...**,
   for example `Gedros.mcl`. From then on open that one.
   (A new version of the package replaces "Geas (new world)", never
   your own world.)
3. It is set for geas.de port 3334, Courier New 9, the number keypad for
   Geas (below) and every plugin of the package. Skip step 4.

### B. Make your own world

1. Open MUSHclient.
2. **File > New World**.
3. Fill in:
   - World name: **Geas**
   - TCP/IP address: **geas.de**
   - Port: **3334**
4. Press **OK**. MUSHclient's own settings (font, colours, command line)
   stay as you choose; the package does not change them. See "Settings
   worth changing" below.

## 4. Add the package (one plugin; not needed with world A)

1. **File > Plugins...** > **Add...**
2. Open the **worlds\plugins** folder inside your MUSHclient folder and
   choose **Geas_Package.xml** > **Open**. Then **Close**.
3. In the game window you should see
   `[Geas] added 17 plugins: GMCP handler, window manager, ...`
4. **Save your world: File > Save** (or Ctrl+S). MUSHclient then
   remembers the plugins next time.

## The setup guide

Once you have logged in, a blue banner asks you to type **`geas setup`**.
That starts the **setup guide**: 16 short steps, about 10 to 15 minutes.
Each step shows **Step # of 16**:

1. Welcome
2. Screen reader (yes or no)
3. Your character's name
4. Save your world under your name
5. Typing and keys (command stacking with `;`, auto-repeat, arrow keys,
   Tab completion, the Geas keypad)
6. Font
7. Layout
8. Colour scheme
9. Map style
10. Your old map
11. Your old world (triggers, aliases, timers)
12. The game's recommended settings
13. Line colours
14. Weapons
15. Problem reports
16. Done

- The recommended choice is marked; any step can be skipped.
- It sets up the basics only. Each step says where to fine-tune later.
- Steps 12 to 14 need you logged in. If you run the guide before logging
  in, they wait and go on by themselves once you are in the game.
- Every step is also printed in the game window with numbered links and
  commands (`geas setup choose <number>`, `next`, `back`, `skip`,
  `stop`). With a screen reader, answer **Yes** in step 2: the guide is
  then text only.
- The banner shows at each login until you run the guide or click
  "Don't remind me". `geas setup` runs it any time; `geas setup step 9`
  goes to one step.

## Settings worth changing

If you skipped the guide, these are the important ones. All in your
world's settings: **Game > Configure** (or Alt+Enter).

- **Your character's name** (please do this): **Connecting** page, in
  **Name**. The combat window uses it to know which team member is you.
  A password is only needed if you want MUSHclient to log you in by
  itself.
- **Font**: **Output** page > **Font**. Popular with MUD players:
  Courier New 9, Consolas 10, Lucida Console 9, Fixedsys (MUSHclient's
  own) or Dina (a free download).
- **Number keypad**: **Keypad** page (Num Lock on). For Geas: 8 north,
  2 south, 4 west, 6 east, 7 northwest, 9 northeast, 1 southwest,
  3 southeast, + up, - down, 5 look. With **Ctrl** held: look in that
  direction (Ctrl+8 sends `look north`, and so on). World A already
  has these.
- **Command line**: **Commands** page. "Auto-repeat command" keeps your
  last command in the box after you send it (MUSHclient leaves it off),
  if you prefer that.

## 5. Connect and log in

1. **Connection > Disconnect**, then **Connection > Connect**.
   (Connecting again after adding the package lets it hear the game
   from the very start.)
2. Log in as usual.
3. Once you are in the game you should see `[Geas] GMCP active.` and,
   after a few seconds, the windows:
   - **chat** across the top,
   - the **game text** under it,
   - a **panel** on the right with tabs: Map, Status, Combat,
     Character, Gear.

If the line says `GMCP waiting` and stays that way once you are in the
game, click **Click here to start** on that line.

## 6. Make it look the way you like (5 minutes)

Many windows at once can be a lot. Start here:

1. **Pick a layout.** Type `geas settings` and open **Layouts**. Press
   **Use** on one:
   - **Minimalist**: mostly game text; vitals as one line; map and chat
     in a narrow panel. Good to start with.
   - **Default**: chat on top, game text, a tabbed panel on the right.
   - **Explorer**: a big map. **RPG**: a bar along the bottom.
     **Full HUD**: everything on screen.
2. **Pick colours.** In Settings, open **Theme** and choose a colour
   scheme (21 of them, for example Charcoal, Midnight, Parchment or your
   guild's or faith's). Choose a border style there too.

   **Game text hard to read?** (Common if you used old colour scripts.)
   After your first login the package asks once: click **[Set up colours
   for me]**. Or later: type `geas lines` and press **Set up colours for
   me**. It saves your own game colours first, sets readable ones, fits
   MUSHclient's colours and command line to your scheme, and from then on
   changing your scheme in Theme recolours everything. **Restore my
   game-side colour settings** in the same window undoes it.
3. **Move and size windows.** Drag a window by its title bar; drag its
   bottom-right corner to resize it. Windows snap to each other's edges.
4. **Tidy up.** Drag a window's title onto another window's title to put
   them together as tabs. Right-click a window > **Hide this window** to put it away;
   Settings > **Windows** brings any window back.
5. **Lock it.** When you are happy: right-click any window > **Lock all
   windows**, so nothing moves by accident.

Changed your mind? Settings > Layouts > **Use** puts a layout back.

## 7. Five things to try

1. **Walk around.** The map learns rooms as you go. Click a room on the
   map to walk there.
2. **Right-click any window** for its options. Drag a window's title to
   move it, or onto another window to make tabs.
3. **`geas settings`** opens the Settings window: every window and
   option, colour schemes (Theme), layouts and the help.
4. **`geas package`** lists the package's plugins and their versions.
5. **Every command** is in Settings > Help: click one to put it in the
   command box.

## Something wrong?

Type **`geas report`**, say what happened, press OK, then click
**[Report it on GitHub]**. Drag the report file into the box and press
**Create**. (You need a free GitHub account.) The report never holds
your login, your password or the words of your conversations.

Quick fixes:
- A window is lost off the screen: `geas win reset all`.
- `geas package` lists the package's plugins and their versions;
  `geas package add` adds any that are missing.

## Updating to a new version

1. Close MUSHclient.
2. Download the zip again (same link), extract it, and drag its four
   folders into your MUSHclient folder again (Replace).
3. Open MUSHclient and your world. Any new plugins are added by
   themselves. Your settings, maps and layouts are kept.

## Used Geas plugins before?

The package turns off old plugins that would clash with it
(GMCP_handler_NJG, the old Geas mapper, Map_Marker, Geas_Weapon_Assist,
Geas_Kill_Counter) and says so. Your old maps, weapons and kills can be
brought in: type `geas map`, `geas weapons` or `geas combat` for the
import commands.
