# Velterra: Sinners Never Sleep

A D&D 5e campaign book built with the `dndbook` LaTeX class, documenting the complete campaign of Velterra.

## Project Overview

This is a LaTeX book in the official D&D 5e sourcebook style, covering a long-running D&D campaign (~2017-2019). The main entry point is `velterra.tex` which compiles all content.

The campaign was DM'd by Michael Williams. Players: Jonathan Mann (Exmerah), Richard Pugh (Riphard), Stephen Harland (Pilcheur/Mark/Vu Dong/Burnie), Stephen Reddish (Kolo/Toni/Martin), Joshua Rodell (Otoria/Gary/Myron).

## Build

- LaTeX project using the `dndbook` document class (included in repo as `dndbook.cls`)
- Supporting style files are in `lib/`
- Build with `pdflatex velterra.tex` (may need multiple passes for TOC)
- TeX Live packages listed in `packages.txt`

## Repo Structure

```
velterra.tex          — Main document, includes all content
content/
  cast.tex            — Cast page (players and their characters)
  story/
    background.tex    — Campaign introduction/summary
    theGods.tex       — The Seven Gods of Velterra
    groups.tex        — Factions and organisations
  world/
    vel.tex           — World overview, map, lore
    locations.tex     — Named locations with descriptions
  chars/
    kolo.tex          — Kolo Kozolski (Goblin Rogue/Ranger)
    exme.tex          — Exmerah Sliokzog (Goblin Artificer)
    riphard.tex       — Riphard Obsidian Hardstone (Dwarf Pastor)
    pilcheur.tex      — Pilcheur Gamont (Human Book Burner)
    otoria.tex        — Lady Otoria Hearthrust (Robot Fighter)
    gary.tex          — Gary (Stone Man)
    mark.tex          — Mark O'Synne (God/Avatar)
    burnie.tex        — Radburny "Burnie" Cinders (Human Book Burner)
    myron.tex         — Smaud Myron (Gnome Arbiter)
    martin.tex        — Martin Andleberger (Construct Bard/Sorcerer)
    toni.tex          — Anthony K Tigerius III (DesertCat Barbarian)
    miscCharacters.tex — Secondary characters (Delilah, Lazarus, Kiros, etc.)
  gear/
    theGary.tex       — The Airship Gary
    STANRI.tex        — S.T.A.N.R.I (Exme's mecha-bear)
    weapons.tex       — Named weapons (C.E.D.R.I.C, Godbringer, etc.)
    misc.tex          — Misc items (Die of Ruh'Brex, Stone of Unthala, etc.)
  eps/
    1.tex–55.tex      — Episode write-ups (session recaps)
    91.tex–93.tex     — Kolo's Tale (interlude episodes after Ep 9)
    335a–335d.tex     — Book Burner flashback episodes
    template.tex      — Unused episode template
  img/                — All character art, maps, item images
img/                  — Cover and background images
lib/                  — DnD book style files
```

## Rules for AI Assistants

### Do not edit episode files
The files in `content/eps/` are the original session write-ups written by the players during or after each game session. They are deliberately informal, irreverent, and full of in-jokes. **They must be preserved exactly as-is.** Do not correct spelling, grammar, tone, or content in any episode file.

### Character page structure
All character files follow this template:
- `\section{Name}` with portrait image
- `\subsection*{Details}` — Race, Class, Age, Status
- `\subsubsection{Background}` — Origin and pre-campaign history
- `\subsubsection{Personality and Traits}` — How they behave
- `\subsubsection{Relationships}` — Bonds with other characters
- `\subsubsection{Name's Story}` — Campaign arc summary

### In-world terminology
- **Gabrins** = Goblins (in-world term used by the players)
- **CC** = Church Calendar (campaign year is 6653 CC)
- **The Sundering** = The event where the Church sealed the world from the gods
- **Excalibrum / Starmetal** = Rare divine metal from meteorites
- **The Inthun** = Enchanted stone slab that grants immense power at great risk
- **Varg** = Northern warlord/barbarian alliance
- **Arbiters** = Church warrior-enforcers
- **The Inquisition** = Church's elite secret enforcement arm

### Player-character mapping
When a player's character died or departed, they rolled a new one:
- **Stephen Harland**: Pilcheur Gamont → Mark O'Synne → Vu Dong → Burnie Cinders
- **Stephen Reddish**: Kolo Kozolski → Toni The Tiger → Martin Andleberger
- **Joshua Rodell**: Lady Otoria Hearthrust → Gary → Myron
- **Jonathan Mann**: Exmerah Sliokzog (entire campaign)
- **Richard Pugh**: Riphard Obsidian Hardstone (entire campaign)

### Campaign plot summary
Lazarus (a devil in Hell) resurrects five dead strangers and tasks them with destroying the Church of the Seven — which has sealed the gods away from the world and is sending too many innocent souls to Hell. The party retrieves the Stone of Unthala, travels to Hope's Rest, founds the Gary Guild and a bank, crosses deserts and seas, raids the Tower of Ruh'Breks (gaining an airship and the Puzzle Die), fights through the jungles of South Africa and the civil war of Masuda, and works to gather the artefacts needed to break the seal and return the gods to the world.

## Content Status

### Complete
- All episode write-ups (eps 1–55, 91–93, 335a–d)
- Character pages for all main and secondary characters
- World overview, gods, groups/factions, locations
- Gear section (airship, STANRI, weapons, misc items)
- Cast page and cover

### Remaining Work
- Some episode numbering gaps (38, 40, 42, 44, 46, 50, 52, 54) — unclear if sessions occurred
- Episodes are informal session recaps, not narrative prose — a future pass could polish these but the players may prefer the original voice
- Some images still use placeholder files (xxx.png/xxx.jpg) — need real art
- Could add appendices for custom classes (noted in original TODOs)
- LaTeX figure environments are nested oddly (figure inside center) throughout — works but not best practice

## Change Log

### 2026-06-08
1. Removed template/example chapter (Template Guide, Text Boxes, Monsters, Colors) and unused LaTeX packages
2. Linked 14 previously unlinked episodes (36–55) into velterra.tex
3. Replaced all placeholder content ("Text", "XXX", "dfhgsfdghfsgh" sidebars) throughout
4. Wrote full character entries for Riphard, Pilcheur, Gary, Otoria, Mark, Burnie, Myron by mining episode content
5. Filled in all misc character stubs, all group/faction entries, location descriptions
6. Rewrote world overview (vel.tex) from gibberish to proper lore
7. Rewrote background.tex from Episode 1 duplicate to campaign introduction
8. Fixed gods section (placeholder sidebar → "The Eighth God", informal notes → narrative, typo fix)
9. Fixed The Gary airship section (3x duplicated paragraph → proper write-up)
10. Fixed STANRI typos and placeholder
