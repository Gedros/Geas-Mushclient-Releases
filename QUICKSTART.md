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
3. In the extracted folder you will see a **worlds** folder, a **lua**
   folder and this guide.
4. Drag the **worlds** and **lua** folders into your MUSHclient folder
   (for example C:\MUSHclient). If Windows asks, choose **Replace the
   files in the destination**.

## 3. Make your Geas world

1. Open MUSHclient.
2. **File > New World**.
3. Fill in:
   - World name: **Geas**
   - TCP/IP address: **geas.de**
   - Port: **3334**
4. Press **OK**. Change any of MUSHclient's own settings (font, colours,
   command line) as you like; the package does not change them.

## 4. Add the package (one plugin)

1. **File > Plugins...** > **Add...**
2. Open the **worlds\plugins** folder inside your MUSHclient folder and
   choose **Geas_Package.xml** > **Open**. Then **Close**.
3. In the game window you should see
   `[Geas] added 16 plugins: GMCP handler, window manager, ...`
4. **Save your world: File > Save** (or Ctrl+S). MUSHclient then
   remembers the plugins next time.

## 5. Connect and log in

1. **Game > Disconnect**, then **Game > Connect**. (Connecting again
   after adding the package lets it hear the game from the very start.)
2. Log in as usual.
3. Once you are in the game you should see `[Geas] GMCP active.` and,
   after a few seconds, the windows:
   - **chat** across the top,
   - the **game text** under it,
   - a **panel** on the right with tabs: Map, Status, Combat,
     Character, Gear.

If the line says `GMCP waiting` and stays that way once you are in the
game, click **Click here to start** on that line.

## 6. Five things to try

1. **Walk around.** The map learns rooms as you go. Click a room on the
   map to walk there.
2. **Right-click any window** for its options. Drag a window's title to
   move it, or onto another window to make tabs.
3. **`geas settings`** opens the Settings window: every window and
   option, colour schemes (Theme), layouts and the help.
4. **Lock the windows** when you like them: right-click > Lock all
   windows.
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
2. Download the zip again (same link), extract it, and drag **worlds**
   and **lua** into your MUSHclient folder again (Replace).
3. Open MUSHclient and your world. Any new plugins are added by
   themselves. Your settings, maps and layouts are kept.

## Used Geas plugins before?

The package turns off old plugins that would clash with it
(GMCP_handler_NJG, the old Geas mapper, Map_Marker, Geas_Weapon_Assist,
Geas_Kill_Counter) and says so. Your old maps, weapons and kills can be
brought in: type `geas map`, `geas weapons` or `geas combat` for the
import commands.
