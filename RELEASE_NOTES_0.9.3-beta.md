Fixes from the reports on 0.9.2, and a new view of the package's hidden checks. Thank you!

**Download:** Geas-Mushclient.zip below. Updating: close MUSHclient, unzip and drag the four folders into your MUSHclient folder again (Replace). Your settings and maps are kept.

What changed:
- **Hidden checks view:** Settings > Hidden checks (or `geas checks view`) lists every check the package sends for itself, what causes it and how often, with an on/off switch for each, a pause and an all-off switch.
- **Concentrating and repairs are no longer interrupted:** nothing is sent while you concentrate, or while a repairer asks "repair or resize". Add your own lines with `geas checks hold add`.
- **Combat window:** appraising a foe shows its appraised health. `team fatigue` and `team stamina` no longer replace health with "?" (optional gauges in Settings > Combat). Old bleeding marks clear. Row arrows are greyed out when you are not in a team.
- **Weapons:** the right verbs: hang morning-stars, slide spears and maces, sheathe swords.
- "Look at it" everywhere now uses `examine`.
- **Vitals:** weight before bulk, as the game shows them.
- **Moving:** `nwu` and similar are left to your own aliases.
- **Setup guide:** importing an old world is one step (MUSHclient's Import box); a new option recalls whole commands with Alt + arrow keys.
- **Menus:** "Services...", "Windows..." and other menus opened from a menu now open the first time.
- **Docks:** a tab clicked after switching programs no longer appears outside its dock.
- **Inventory:** right-click Carried or Worn to open or close every container there.
- **Your stats, skills and kill files** now live in your log folder, under `geas` (`geas set folder` to choose another). Existing files are moved there.

Something odd? Type `geas report` in MUSHclient and attach the file to a new issue.
