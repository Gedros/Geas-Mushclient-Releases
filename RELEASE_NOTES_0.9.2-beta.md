Fixes from the second round of tester reports. Thank you!

**Download:** Geas-Mushclient.zip below. Updating: close MUSHclient, unzip and drag the four folders into your MUSHclient folder again (Replace). Your settings and maps are kept. **Saved layouts:** layouts you saved with `geas win layout save` before this version were saved empty (a bug): arrange your windows and save them again.

What changed:
- **Invoking is no longer aborted.** The package's hidden checks of your foes could interrupt an invoke ("You abort invoking."). Now the package never sends one while you invoke, and only ever one hidden check at a time. `geas checks` lists the last ones.
- **No more doubled lines.** Two hidden checks at once could write the same line twice (combat messages, the "You are feeling ..." line). Each line is now written once.
- **Fewer hidden checks.** The Combat window checks your foes when a fight starts, after 10 s without a combat line, after a kill command, when a foe dies, a new one attacks or you move. During steady fighting it sends nothing.
- **Inventory:** no hidden `inv` any more, so your buff messages no longer appear by themselves. A worn backpack or belt is listed under Worn and wielded only. A single foe is now targeted as `foe` in the Combat window, so extradesc names work.
- **Weapons:** a weapon wielded two-handed is known as two-handed, so Specials no longer offers Slam for it. Two identical weapons show as one entry with "x2".
- **Saved layouts** now bring back every window, hidden ones too, and their title bars. Changing the font in the setup guide no longer moves your windows. A new preset: **Adventurer**.
- **Windows scroll** when their content does not fit (Armour, Stats, Combat settings, Weapons, Weapon sets, Specials): the mouse wheel, or the thin bar on the right. A window you open comes to the front.
- **Combat settings** shows every encumbrance line and your fight mode; its columns are no longer cut off.
- **Vitals:** choosing "One colour" in Settings now shows straight away, and each bar's text colour can be changed. The Combat window's health now matches Vitals.
- **Setup guide:** Courier New, Consolas, Lucida Console and Verdana in 9 to 12 pt.

Something odd? Type `geas report` in MUSHclient: reports now include the hidden checks.
