Fixes and changes from the first testers' feedback. Thank you!

**Download:** Geas-Mushclient.zip below. Updating: close MUSHclient, unzip and drag the four folders into your MUSHclient folder again (Replace). Your settings, maps and layouts are kept.

What changed:
- **A calmer start.** One line when the world opens, nothing at the login screen, and one welcome message after login: run the setup guide, plugins and their help, Settings, or Retry GMCP. It can be turned off (`geas welcome` shows it again).
- **A simpler first layout** (Default): chat on top, the game text, Vitals and the Map on the right. Everything else is in Settings > Windows.
- **Classic colour scheme**, the new default for new installs: black and greys with the classic MUD colours.
- **Windows:** an **x** on every title bar to hide the window; the title bar can be hidden per window (right-click) or all at once (`geas win titles hide`). A hidden title bar is cropped off, so windows snap right next to each other; drag them from inside.
- **Line colours window:** its buttons wrap to fit the window.
- **Fixed:** the rank in Stats ("You are a Champion"); "outer clothing" spilling into the condition in the Armour window; only one encumbrance line kept; foes shown twice in the combat window.
- **Combat:** "Kills today" can be turned off.
- **Specials:** a new view with one cooldown bar per action slot (Main, Hand, Foot, Head, Leg). Rename slots, change their bars, or add your own slots for other cooldowns; `geas specials slots start <slot>` starts one from your own triggers.
- **Your old xmarks and xnotes**, even from MUSHclient 4.94: import your old map, then right-click the map > Import > Marks and notes from an old MUSHclient, and choose your old world file. The old Map_Marker plugin is not needed (see the quick start guide).
- **Setup guide:** clearer steps, the game settings as a tick list, a "don't add my weapons" choice, your old xmarks and xnotes, fonts in 11 and 12 pt (for laptops) used for the windows too, and the guide window fits every step.
- **Installing over an old MUSHclient?** The package now warns if MUSHclient's plugins folder still points at the old copy, with the fix. The quick start guide explains it, and that the MUSHclient download link needs a right-click > Save link as.

Something odd? Type `geas report` in MUSHclient.
