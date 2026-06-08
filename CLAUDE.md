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
    1.tex–80.tex      — Episode write-ups (session recaps, campaign goes to ep 80)
    9a.tex            — Die Hard Part 3 / Death of Otoria (formerly 9.tex)
    9b.tex–9d.tex     — Kolo's Tale (interlude episodes after Ep 9, formerly 91-93)
    33-5a–33-5d.tex   — Book Burner flashback episodes (formerly 335a-335d)
    68a.tex           — Exme's Thoughts supplement
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
Lazarus (a devil in Hell) resurrects five dead strangers and tasks them with destroying the Church of the Seven — which has sealed the gods away from the world and is sending too many innocent souls to Hell. The party retrieves the Stone of Unthala, travels to Hope's Rest, founds the Gary Guild and a bank, crosses deserts and seas, raids the Tower of Ruh'Breks (gaining an airship and the Puzzle Die), fights through the jungles of South Africa and the civil war of Masuda. They return to the dwarven mountains seeking Excalibrum — the only metal that can harm the Church's Inquisitors. Kolo falls to the elder entity Kalimar, murders Delilah, and is killed by Riphard. The party regroups in Linderdorf, forges Excalibrum weapons, wins a giant robot in an arena fight, and builds an alliance army. They assault the Seven's Spire to break the Great Stone's seal and return the gods to the world, becoming demigods in the process.

## Content Status

### Complete
- All episode write-ups (eps 1–80, 9b–9d, 33-5a–d, 68a) — campaign goes to episode 80
- Character pages for all main and secondary characters
- World overview, gods, groups/factions, locations
- Gear section (airship, STANRI, weapons, misc items)
- Cast page and cover

### Remaining Work
- Episodes 38-80 and 68a are plain text, not yet formatted as LaTeX — need wrapping in dndbook episode structure to compile
- Episode 59 is empty (title only: "Listing Heavily")
- Episode 80 notes: "NOTE WE NEED TO GRAB THE FINAL ENDING NOTES WHERE THEY BECOME DEMIGODS!!!" — final campaign ending not yet written up
- Episodes are informal session recaps, not narrative prose — the players prefer the original voice
- Some images still use placeholder files (xxx.png/xxx.jpg) — need real art
- Could add appendices for custom classes (noted in original TODOs)
- LaTeX figure environments are nested oddly (figure inside center) throughout — works but not best practice

## REFERENCE.md — Campaign Knowledge Base

The file `REFERENCE.md` (in repo root) is a comprehensive index of the entire Velterra campaign, built by reading all ~90 episode files and all content files. It contains:

- **Player Characters**: Full profiles with player mapping, episode ranges, key moments, relationships
- **Secondary Characters**: ~40 NPCs with roles, key details, and source files
- **Factions & Groups**: All organisations with members, descriptions, and episode appearances
- **Locations**: Every named location across all continents with key events and episode links
- **Items & Gear**: All weapons, artefacts, vehicles, and equipment with stats and descriptions
- **The Seven Gods**: Complete pantheon including the secret eighth god (Synne)
- **Key Lore & Terminology**: In-world terms, concepts, and campaign-specific vocabulary
- **Episode Index**: One-line summary of every episode (1-80, 9b-9d, 33-5a to 33-5d, 68a) with source file links
- **Campaign Arc Summary**: 14-phase plot overview from resurrection to the Seven's Spire assault

### How to Use REFERENCE.md

1. **Before reading episode files**: Search REFERENCE.md first to find which episodes/files contain the information you need. This saves significant tokens vs reading all episodes.
2. **For character questions**: Look up the character in the Player Characters or Secondary Characters section to find their source file, episode range, and key details.
3. **For lore/world questions**: Check the Locations, Lore & Terminology, or Gods sections for quick answers, then read source files only if more detail is needed.
4. **For "what happened in episode X"**: Check the Episode Index for a one-line summary and the source file path.
5. **When adding new content**: Use the reference to check for consistency with existing characters, locations, items, and plot points.
6. **When the user asks to add characters or lore**: Cross-reference REFERENCE.md to identify where they appear in episodes, then read those specific episode files for full detail.
7. **Keep it updated**: When new content is added to the book (new characters, locations, items, etc.), update REFERENCE.md to keep it current.

## Change Log

### 2026-06-08 (Session 2)
1. Added 30+ new episode files (38, 40, 42, 44, 46, 48, 50, 52, 54, 56-80, 68a) — plain text, not yet LaTeX formatted
2. Renamed episode files: 9.tex→9a.tex, 91-93→9b-9d, 335a-d→33-5a to 33-5d
3. Updated velterra.tex to reference renamed files and include all new episodes
4. Fully rewrote REFERENCE.md with all new episode summaries, characters, locations, items, and campaign arcs 10-14
5. Updated CLAUDE.md with new episode structure, campaign summary, and remaining work

### 2026-06-08 (Session 1)
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
