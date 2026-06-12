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
    1.tex–108.tex     — Episode write-ups (session recaps; eps 81-108 are the 2022
                        continuation, scraped from r/Velterra)
    9a.tex            — Die Hard Part 3 / Death of Otoria (formerly 9.tex)
    9b.tex–9d.tex     — Kolo's Tale (interlude episodes after Ep 9, formerly 91-93)
    33-5a–33-5d.tex   — Book Burner flashback episodes (formerly 335a-335d)
    4a, 15a, 22a–d, 24a, 40a, 57a, 58a, 64a, 68a, 69a, 77-5.tex
                      — Interlude/supplement posts (in-character journals, musings,
                        side fiction, lore documents from r/Velterra)
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
- **Stephen Reddish**: Kolo Kozolski → Toni The Tiger → Martin Andleberger → Kolo (restored, eps 98+)
- **Joshua Rodell**: Lady Otoria Hearthrust → Gary → Myron
- **Jonathan Mann**: Exmerah Sliokzog (until erased from existence, ep 97)
- **Richard Pugh**: Riphard Obsidian Hardstone (departs ~ep 100)

The 2022 continuation (eps 81-108) added one new player, Natalie Southernden
(reddit handle /u/Thrawien), who played Erin then Gem. Jonathan Mann's new reddit
handle was /u/its_Samar; after Exme's erasure he played Bronwen. New-era characters:
Sgt Erin Devereux (dies ep 101), Bronwen (devil minder, ep 98+), Gem (silicate
spacefarer, ep 102+), Bucky McCaw (joins ep 104, after Burnie dies ep 103).

### Campaign plot summary
Lazarus (a devil in Hell) resurrects five dead strangers and tasks them with destroying the Church of the Seven — which has sealed the gods away from the world and is sending too many innocent souls to Hell. The party retrieves the Stone of Unthala, travels to Hope's Rest, founds the Gary Guild and a bank, crosses deserts and seas, raids the Tower of Ruh'Breks (gaining an airship and the Puzzle Die), fights through the jungles of South Africa and the civil war of Masuda. They return to the dwarven mountains seeking Excalibrum — the only metal that can harm the Church's Inquisitors. Kolo falls to the elder entity Kalimar, murders Delilah, and is killed by Riphard. The party regroups in Linderdorf, forges Excalibrum weapons, wins a giant robot in an arena fight, and builds an alliance army. They assault the Seven's Spire to break the Great Stone's seal and return the gods to the world, becoming demigods in the process.

**The Continuation (eps 81-108, played 2022)**: Four in-world years later, magic has returned but the gods stay distant. Lazarus — now ruling Hell as the Empire of the Eight — regathers the scattered party with new recruit Sgt Erin Devereux: the warlord Valkar Varg has made a pact with Kalimar and is brewing super-soldiers. The party infiltrates the Varg tribes, tracks Valkar north, and destroys Kalimar in his lava sanctum — Myron dies and is resurrected, Kolo is restored in a construct body, and Exmerah erases herself from existence with a forbidden wish. Then Kalimar's mate Canalon, an elder-god space dragon, descends and mind-controls the allied army and Hope's Rest. Erin (ep 101), Burnie (ep 103), Captain Stick and the airship Gary (ep 103) all fall against a githyanki Nautiloid. Myron leads the remnant (with devil Bronwen, spacefarer Gem and Bucky McCaw) by steam railway to Hope's Rest, heists the Black Rock bank vault, and claims the Armoury of Sin — the gear the god Sinn wore when he last fought Canalon. The written record ends at ep 108: "Well, we're off to fight a God." The final battle was never written up.

## Content Status

### Complete
- All episode write-ups (eps 1–108, 9b–9d, 33-5a–d, plus interludes 4a, 15a, 22a–d, 24a, 40a, 57a, 58a, 64a, 68a, 69a, 77.5) — all formatted as LaTeX. Eps 81–108 and the interludes were scraped verbatim from r/Velterra (June 2026)
- All main character pages: Kolo, Exme, Riphard, Pilcheur, Otoria, Gary, Mark, Burnie, Myron, Toni, Martin — fully written with Background, Personality, Relationships, Story, and DndSidebar sections
- All secondary characters in miscCharacters.tex: Delilah, Lazarus (expanded with continuation), Kiros, Kevin, Captain Stick (death noted), Vu Dong, Meredith, Trayvon, Ruh'Breks, Holly, Twins, Derek, King Oceani, Tiki Tuks, Garbigail, Arbigal, Daisuke, Archibald, Lillith, Dagenham, Google Von Maccherstein, Buck/Bucky McCaw (expanded with continuation), Lady Gharbighast, Rolltop Kandian, Lark, Mrs Ball, David, Valkar Varg, Krankle, Valklondar, Magrat, Zelat, Malkior, Reggie, Arbiter Giros, Badunkadonk, Shroomy. Minor figures tables for both campaigns.
- Groups/factions: Church, Jennies, SRA, Book Burners, Gary Guild, Bank, Hearthrust Society, Inquisition, Varg (updated with Valkar/Pact warriors/Chesney Hawks), University of Assassins, Alliance Army (updated with Canalon mind-control), Hell Inc./Empire of the Eight (updated), Githyanki (new)
- Locations: All Main Land locations (Hope's Rest (updated with Canalon occupation), Vathos Boundary, Temple of Unthala, Riverfall, Seven's Spire, Logarsk, Great Expanse, Port Averdale, Tom'ardy Mountains, Linderdorf, New Abbergast, Golding's Bay, Varg Lands (updated), Bright Bart Forge, Jecede, Midnight Pearl, Kalimar's Lair, Black Rock, Fishy Library, Jecede Railway, Erdun's Well), plus Nanduan, Masuda, South Africa, Hell
- Gods: All seven gods with descriptions, Synne filled in, Kalimar sidebar (updated: dead), Canalon sidebar (new)
- Gear: Airship (with hyper-speed and destruction), STANRI (with continuation/headmaster), all weapons (CEDRIC, Godbringer, Black Sabbath, Iron Maiden, Kolo's Mechanical Bow, Stone Knife, etc.), misc items (Puzzle Die with all functions and Wish used, Inthun, Excalibrum, Armoury of Sin, Kalimel, Rings of Mind Shielding, etc.)
- World overview, cast page, cover
- Story chapter (background.tex): fully expanded with "About This Book" (updated for both campaigns), "The World", "The Mission", "The Five Strangers", restructured 16-arc campaign narrative (Arcs I-XI original campaign, Arcs XII-XVI continuation), "In Memoriam" sidebar (all deaths including continuation), "Campaign by Numbers" (108 eps, 6 players, 16 PCs), "Themes of the Campaign" (with continuation coda), "The Continuation" as its own section

### Remaining Work

#### Three Missing Battles (needs player/DM input)
These pivotal scenes were never written up by the players and cannot be reconstructed from episode text alone:
1. **Campaign 1 finale** (post-ep 80): The actual breaking of the seal at Seven's Spire and the party becoming demigods. Ep 80 ends mid-assault; ep 81 opens "We are gods to be."
2. **Exme's sacrifice** (during ep 97): The full scene in Kalimar's lava sanctum. What happened: Kalimar nearly killed everyone. Myron was critically injured, paralysed and dying. Exme used the Puzzle Die's Wish function (the only wish in existence, 10,000-year cooldown) to give up her own life to restore Kolo AND heal Myron, because she could not choose between them. The wish was accepted, but because the ask was so extreme, she was erased from all reality: no resurrection, no godhood, no afterlife, no Hell. The episode text covers the battle but the emotional weight of the wish itself deserves fuller treatment. Jonathan (Exme's player) later suggested in Discord that Exme may have been moved to a reality that exists inside Mrs Ball (each Ball contains a universe, and Mrs Ball's people restore broken ones). This has not been established as canon but could be included as a rumour or whisper.
3. **Campaign 2 finale** (post-ep 108): The battle with Canalon wearing the Armoury of Sin. Ep 108 ends "Well, we're off to fight a God." The outcome was never written up.

#### Continuation Updates (COMPLETE)
All continuation content has been folded into the book:
- All 11 main character pages updated with continuation stories (Session 7)
- background.tex restructured to 16 arcs (I-XI original, XII-XVI continuation), all sidebars/stats updated (Session 8)
- groups.tex updated: Varg (Valkar/Pact warriors), Alliance Army (mind-controlled), Hell Inc. → Empire of the Eight, Githyanki added (Session 8)
- locations.tex: 7 new-era locations added, Hope's Rest and Varg Lands updated (Session 8)
- theGods.tex: Kalimar updated (dead), Canalon sidebar added (Session 8)
- Gear files: Airship destruction, STANRI headmaster, Kolo's Bow, Armoury of Sin, Kalimel, Rings of Mind Shielding all added (Session 8)
- miscCharacters.tex: Lazarus expanded, Buck McCaw expanded, 8 new NPCs (Valklondar, Magrat, Zelat, Malkior, Reggie, Giros, Badunkadonk, Shroomy), new minor figures table (Session 8)
- Discord RP content woven into character pages (Session 7)

#### Other
- New-era character pages (Erin/Bronwen/Gem) now have art for Bronwen; Erin and Gem still have no portrait art
- All placeholder images (xxx.jpg/xxx.png) have been resolved: 2 replaced with real images (eps 55, 57), 18 episode placeholders and 3 weapons placeholders commented out (Session 9)
- All 8 previously unused images now placed: garygrave.png, incognitoMyron.png, ladyHaramxe.png, plan.png, esmeBlack2.jpg, mainLand.png, kolo.jpg, excal1.jpg (Session 9)
- 69 episodes still have no images (all continuation eps 81-108, all interludes, and ~41 original campaign eps). See plan file for prioritised art wishlist.
- Could add appendices for custom classes (noted in original TODOs, needs DM input)
- LaTeX figure environments are nested oddly (figure inside center) throughout — works but not best practice

### Ideas for Future Enrichment
- **Campaign Timeline**: Chronological table of major events with in-world dates (if DM established any). Could go in Chapter 1 or Chapter 2 alongside world/locations.
- **Glossary/Terminology Appendix**: In-world terms (Gabrins, CC, Sundering, Excalibrum, Emancipation, etc.) are documented in REFERENCE.md for AI use, but a printed glossary in the book would help human readers navigate the episodes.
- **Character Relationships Section**: Diagram or table of connections — romances (Riphard/Delilah, Exme/Myron, Daisuke/Archibald, Burnie/Trayvon), mentorships (Burnie/Kevin), rivalries, family ties (goblin twins, Hardstone/Hardthrust dynasty, Myron's family).
- **DM's Notes / Afterword**: Meta-commentary from Michael Williams on designing the campaign, memorable moments, what he'd do differently. Needs DM input but would be a brilliant capstone to the book.

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

### 2026-06-12 (Session 9)
1. Placed all 8 previously unused images: garygrave.png (Gary's memorial, gary.tex), incognitoMyron.png ("NOT MYRON" disguise, myron.tex), ladyHaramxe.png (Lady Gharbighast portrait, miscCharacters.tex), plan.png (campaign collage, background.tex), kolo.jpg (additional Kolo art, kolo.tex), mainLand.png (continent map, locations.tex — uncommented existing reference), esmeBlack2.jpg (goblin archer, replaced xxx in ep 55), excal1.jpg (metal ingots, replaced xxx in ep 57).
2. Commented out all 21 remaining xxx placeholder image blocks: 18 episode files (eps 27, 31, 33, 41, 43, 45, 47, 48-5, 51, 53, 61, 63, 65, 67, 73, 75, 77, 79) plus template.tex, and 3 weapon entries in weapons.tex (Black Sabbath, Iron Maiden, Hammer of the Gods). Captain Stick placeholder no longer appears in printed book.
3. Updated CLAUDE.md: Content Status updated to reflect image work, art wishlist documented in plan file, session changelog added.

### 2026-06-12 (Session 7)
1. Placed 5 new images: bronwen_temp.png (Bronwen portrait), ExmeOlderPortraitFinal.png (Exme campaign 2), ProfStanri.png (Stanri as headmaster), SchoolLogo.jpg (TDHSFEGGTEIEAE crest), MrsBall.png (Mrs Ball entry in miscCharacters).
2. Updated all 9 character pages with continuation content (eps 81-108):
   - Exme: Status → "Erased from existence (ep 97)". Full continuation story (broken drunk, school, Kalimar lair, the Wish, erasure). Mrs Ball rumour sidebar. Relationships updated. Creations sidebar updated (Stanri as headmaster).
   - Kolo: Status → "Dead (ep 68), restored in a construct body (ep 98)". Continuation story (restoration, Mr Robot, mechanical bow, eulogy from Discord RP, fighting through to Armoury of Sin).
   - Burnie: Status → "Dead (ep 103)". Continuation story (Fishy Library, swallowed by Kalimar, Synne speech from Discord RP, charging elder brain alone, death/cremation).
   - Myron: Full continuation (arbiter army, Zelat duel, killed by Kalimar, resurrected by wish, Erin's posthumous honours, accepting leadership, leading remnant to Armoury of Sin).
   - Riphard: Status → "Departed (~ep 100)". Continuation (Black Rock, Pope of Skeleton Giants, departs in Jecede).
   - Martin: Status → "Faded from the story (~ep 99)". Continuation (Inquisitor hunting, teaching, exploded by Buchra, feeblemind, fades when Kolo returns).
   - Erin: Added player (Natalie Southernden), Discord RP moment with Kolo, Myron's posthumous honours.
   - Bronwen: Added player (Jonathan Mann), Discord RP rallying speech.
   - Gem: Added player (Natalie Southernden).
3. Fixed player-character mapping: /u/its_Samar = Jonathan Mann (new handle); /u/Thrawien = Natalie Southernden (new player). Erin and Gem both played by Natalie; Bronwen by Jonathan.
4. Updated CLAUDE.md remaining work with three missing battles (Campaign 1 finale, Exme's sacrifice detail, Campaign 2 finale), Discord RP content notes, and detailed continuation update checklist.
5. Read and analysed extraRPnotesafterExmeDead.txt (Discord in-character RP between sessions). Key content woven into character pages: Kolo's eulogy, Burnie's Synne speech, Erin's moment with Kolo, Bronwen rallying the group, Myron's honours for Erin.

### 2026-06-12 (Session 8)
1. Restructured background.tex campaign narrative: merged overlapping arcs (I+II → Arc I, XI+XII → Arc IX, Book Burner Flashbacks folded into Masuda), fixed episode boundary overlaps (Tom'ardy/Kolo's Descent), renumbered to 11 arcs for campaign 1. Added "The Continuation" as its own \section with 5 new arcs (XII-XVI: One More Time, Among the Varg, Destruction of the Creator, Canalon Descends, The Last Heist). Updated "About This Book" (108 eps, 6 players, two campaigns). Replaced placeholder ReadAloud with ep 108 quote. Updated In Memoriam (added Exme erased, Riphard departs, Erin, Burnie). Updated Campaign by Numbers (108 eps, 16 PCs, "1 bank heisted (same bank)", "1 deal with a devil. Then another one."). Added continuation line to Themes sidebar.
2. locations.tex: Added 7 new-era locations (Jecede, Midnight Pearl, Kalimar's Lair, Black Rock, Fishy Library, Jecede Railway, Erdun's Well). Updated Hope's Rest (Canalon's occupation) and Varg Lands (continuation infiltration).
3. groups.tex: Updated Varg (Valkar, Pact warriors, Chesney Hawks, Buchra, Eric), Alliance Army (mind-controlled by Canalon), Hell Inc. → "Hell Inc. / The Empire of the Eight" (Lazarus ruling, Bronwen sent). Added Githyanki (Nautiloid, Ulitharid, elder brain, Erin/Burnie/Captain Stick deaths, Gem's rescue).
4. theGods.tex: Updated Kalimar sidebar to past tense (dead, killed by Mrs Ball, Kolo freed by Wish). Added Canalon sidebar (elder-god space dragon, mind-control, Canilon tattoo connection, Gem's people, Armoury of Sin).
5. Gear files: theGary.tex (added Destruction section: ep 103, Captain Stick's sacrifice). STANRI.tex (added Continuation section: headmaster of Exme's school, ProfStanri.png image, fixed "conciousness" typo). weapons.tex (added Kolo's Mechanical Bow). misc.tex (updated Puzzle Die with Wish used note, added Armoury of Sin, Kalimel, Rings of Mind Shielding/Jetpacks).
6. miscCharacters.tex: Expanded Lazarus (tripled: war room, communication style, Arbigal rivalry, Empire of the Eight, astral projection, rings/jetpacks gifts, vol-au-vents, Kolo's HR ticket). Expanded Buck McCaw (continuation as Bucky: plague doctor mask, farewell letter, train fights, scouting bank). Updated Captain Stick (death). Added 8 full new-era NPC entries: Valklondar (lich, games room, Pope of Skeleton Giants), Magrat (giant chieftain, eats a man whole), Zelat (tiger-monk, full duel with Myron), Malkior (monkey-beast, feeblemind, flayed to mist), Reggie (ghost in dogtags), Arbiter Giros (joint Lord Commander), Badunkadonk (telepathic octopod, standoff), Shroomy (sentient mushroom narrator). Added new-era minor figures table (Jeremiah, Buchra, Eric, Krum, Ragnor & Vesh, Calista & Michelle Devereaux, Adam-ants).
7. Updated CLAUDE.md: Content Status fully updated to reflect all continuation work complete. Remaining Work section updated.

### 2026-06-12 (Session 6)
1. Added pages for the new-era party members: content/chars/erin.tex (Sgt Erin Devereux), bronwen.tex, gem.tex, wired into the Characters chapter after toni.tex. No portrait art exists for them: the 2022 continuation posted only episode text and one unreachable reddit gallery (s3shrh), so these pages ship without images.
2. Added miscCharacters.tex entries for Mrs Ball, David, Valkar Varg and Krankle.
3. Removed every LaTeX em dash (---) from the curated prose (chapters: chars, story, world, gear): 331 became commas, 12 definition labels became colons, and three pull-quote attributions in background.tex became right-aligned italic lines. Episode files (content/eps/) were left untouched per the verbatim-preservation rule, so player-written em dashes remain there. En dashes (date ranges, recovered-document extracts) were left as-is.
4. Book rebuilds clean at 319 pages.


### 2026-06-12 (Session 5, continued — image scrape)
1. Scraped all images from r/Velterra posts (64 direct downloads; 12 were already in the repo under other names — confirmed by perceptual comparison; e.g. krokokolo.png = "Good night my sweet prince", koloShield.png = "Myron's New Shield", velterraMap.png = "Map as of Episode 71").
2. Added 36 new images to content/img/reddit/ (resized to ≤2000px, ~26MB), each placed with its original post title as an italic caption.
3. Replaced 5 episode placeholders (xxx.jpg): ep 39 (Myron vs. 15 Orcs), ep 49 (Deal with it), ep 59 (Map as of Ep 59), ep 69 (Half a World Between Us map), ep 71 (existing velterraMap.png).
4. Added figures to episodes: 9a (A Hero's Grave), 9b (four Clan Stanri portraits), 9c (DeadlySeaSnake, Tree Octopodicus, Forest Death Hippo, Dane'O'Saurus), 9d (Gabrin life), 10 (Hope's Rest Times), 18 (Guild HQ, Humans need not apply), 19 (G-AMRC Apothecary, #exmelab selfie), 23 (MVG barrel), 26 (Goodnight Sweet Prince), 29 (inside the crocodile), 58/64 (campaign maps), 70 (Google's map), 72 (Colourblind Crashnic).
5. Added art to character pages: Otoria (original Feb 2017 art), Exme (with gun), Pilch (10% more emo; Howlov; recovered-from-fire parchment), Riphard (mini ready to paint), Toni, Myron (Arbiter Smord art), Gary (Officer Djago). Book Burner's Mask added to groups.tex.
6. Not retrievable: "Velterra - Where do you hail from?" (imgur, geo-blocked), "The Story so Far" imgur album, the Delilah Hardstone School reddit gallery, two GIFs (one converted: Book Burner's Mask), and subreddit-stylesheet images (%%dropbear%% etc.). 21 episode placeholders remain with no matching reddit art.

### 2026-06-12 (Session 5, continued — wiki augmentation)
1. Scraped the full r/Velterra subreddit wiki (48 pages via old.reddit: quests, locations, NPCs, groups, knowledge, bestiary, magical items, character pages, research documents).
2. New file content/world/archives.tex ("The Velterran Archives" section in Chapter 2): Chronicles of Rhu'Brex extract, the Vuthros pamphlet, Scraps of an Ancient Poem, the party's Magical Item Ledger (rumours table), the Quest Ledger, and the Bestiary of Velterra — all preserved verbatim from the wiki.
3. weapons.tex: added The Stone Knife (full wiki description of Burnie's stone dagger).
4. Character page merges from wiki: Burnie (Book Burner leadership, Killjoy hanging/faked death, Martha Mayfire, Battlemastermind style, full Augments and Arsenal subsection), Myron (full-legal-name sidebar), Mark (book imprisonment, Gary father-figure, Vu Dong champion trade, Meredith reconciliation), Pilch (itching bandaged arm, life-drain, crossbow Martha, killed by a Chuul, Quoth's white-raven rescue), Gary (built by the Ancients to protect; hacked down by TikkiTucks), Riphard (pastor's son, sheltered upbringing), Exme (gunpowder quote, healing salve), Otoria (eldest-child tradition).
5. World merges: vel.tex (main continent named Valeria), locations.tex (Hope's Rest guild heads, Vathos Boundary proprietors, Hollie Granger nepotism, Logarsk Inquisition motive, Codie the tower caretaker), miscCharacters.tex (Lazarus Goldstein; "Minor Figures from the Party's Records" table: Gerard, Hans Gruber, Diego's death, Henry & Henri, Hestor's caravan, Boa Sab, Terry/Trevor, Codie, Arbiter Killjoy, Martha Mayfire, Lady Haremxes).
6. Not merged (flagged): wiki lists Otoria's race bluntly as "Sex-bot" (book says "dwarven-crafted automaton"); "The Inscribed" faction page survives only as an edit-conflict error — name recorded in REFERENCE.md only; age discrepancies (wiki Riphard 43 vs book 58, Toni late-40s vs 42) left as the book had them.

### 2026-06-12 (Session 5)
1. Scraped all 218 posts from r/Velterra (via RSS) and added the complete 2022 continuation: episodes 81–108 (28 new episodes, including the out-of-order ep 97 and the untitled ep 93 "Its the girth not the length"), converted verbatim to LaTeX in the established episode style.
2. Added 13 interlude/supplement posts as new episode files: 4a (Kolos Plan, with comment thread), 15a (Pilch Journal), 22a–d (Musings on Sorcery/Lunch, Subjects please, Puzzle Die), 24a (Musings on Light), 40a (Church factions), 57a/58a (Adventures of Snark 1–2), 64a (Crumpled Parchment), 69a (We're all Synners here), 77-5 (Masudan Fan-Fiction, with comment thread).
3. Wired all 41 new files into velterra.tex (now 130 episode inputs); book builds clean at 306 pages.
4. Updated REFERENCE.md: continuation episode index (81–108), interludes index, arcs 15–19 + revised endgame, PC status updates (Exme erased ep 97, Kolo restored ep 98, Burnie dies ep 103, Myron leads, Riphard departs ep 100, Martin fades), new PC entries (Erin, Bronwen, Gem), New Era characters/factions/locations/items tables.
5. Confirmed eps 7 (Inflatable Cow), 13 (Fritzls Basement), 48-5 (Josie), 33-5d (Bobacious), 9b–d (Kolo's Tale) already in the book under different titles; skipped meta/admin posts (e.g. "Fixing Revised Ranger" homebrew — possible appendix material).


### 2026-06-09 (Session 4)
1. Major expansion of background.tex (story chapter): rewrote from ~30-line intro to full campaign overview (~300 lines). Added "About This Book" meta section, "The World" setting overview, "The Mission" section with Lazarus DndReadAloud quote, "The Five Strangers" party introductions with origTeam.png image, and complete 14-arc campaign narrative prose (Resurrection through The Battle & The Spire). Added "In Memoriam" sidebar tracking all PC deaths/departures, "Campaign by Numbers" DndComment stats box, and "Themes of the Campaign" sidebar.
2. Updated REFERENCE.md: added ✦ markers to all secondary characters with full book entries (Lark, Lillith, Arbigal, King Oceani, Dagenham, Buck McCraw, Google Von Maccherstein, Lady Gharbighast, Garbigail, Rolltop Kandian). Updated Synne gods entry (replaced "??? Domains unknown" with full details). Expanded weapon descriptions (Black Sabbath, Iron Maiden, Godbringer, Myron's Shield). Updated airship entry (bomb bays, Stonecast Mech cargo, STANRI systems).
3. Updated CLAUDE.md: added story chapter to Complete list, added "Ideas for Future Enrichment" section (timeline, glossary, relationships, DM afterword).

### 2026-06-09 (Session 3)
1. Converted all remaining plain-text episodes (50, 52, 54, 56-80, 68a) into proper LaTeX formatting
2. Full refresh of all main character pages: rewrote Kolo, expanded Exme (full late-campaign arc, creations sidebar), expanded Riphard (Dagenham, twins, mannequin delusion, Northern Rock sidebar), expanded Pilcheur (Book Burner flashback revelations), expanded Otoria (Hearthrust Society legacy), expanded Gary (Garbigail takeover, Battle of Hope's Rest), expanded Mark (VR storm machine, Meredith prom), expanded Burnie (IRIS, stone dagger, mania, full late-campaign story), expanded Myron (family background, full story through Spire, Piece of Shit sidebar), rewrote Toni (from stub to full entry), rewrote Martin (from stub to full entry with Mr Mouse sidebar)
3. Expanded miscCharacters.tex: updated Delilah (death), Kiros (capture/rescue), Kevin (expanded), King Oceani (full arc), Daisuke (sacrifice/romance), Archibald (romance), fixed Garbigail/Arbigal split. Added 7 new characters: Lillith, Dagenham, Google Von Maccherstein, Buck McCraw, Lady Gharbighast, Rolltop Kandian, Lark
4. Expanded groups.tex: added Inquisition, Varg, University of Assassins, Alliance Army. Expanded Hearthrust Society and Hell Inc.
5. Major locations.tex rewrite: expanded Hell, Hope's Rest (guild system), Vathos Boundary, Tom'ardy (Delvers/mines), Seven's Spire (full tower layout), Logarsk (Inthun), Great Expanse, Port Averdale. Added Linderdorf, New Abbergast, Golding's Bay, Varg Lands, Bright Bart Forge, Masuda
6. Updated theGods.tex: filled in Synne entry, added Kalimar sidebar
7. Updated weapons.tex: expanded CEDRIC, Godbringer (arena scene), Black Sabbath, Iron Maiden
8. Updated misc.tex: expanded Puzzle Die (new functions table), Stone of Unthala, Slab of Inthun
9. Updated theGary.tex: hyper-speed upgrade, Stonecast Mech cargo
10. Updated CLAUDE.md and REFERENCE.md to reflect all changes

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
