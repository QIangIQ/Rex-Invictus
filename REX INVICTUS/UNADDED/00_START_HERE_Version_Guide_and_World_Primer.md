# START HERE — Rex Invictus: Version Guide & World Primer

> The world lorebook for the *Rex Invictus* character-profile set: how to use the profiles, how the timelines fit together, which file is which version of whom, a full glossary, a plot chronology for Ch 1–23, and a pointer to the canon rulings that settle the story's own contradictions.
>
> **Governing file:** `00a_CANON_RULINGS.md`. Where this primer and the rulings ever disagree, the rulings win. Ruling IDs (R1–R8, S1–S15, C1–C34) are cited throughout.

*Rex Invictus* is a Percy Jackson AU fanfiction. A millennia-old Percy, the last guardian of a ruined Olympus in the far future, is sent back by Chaos into his young-teen body in the present day (c. 2021 per the author's timeline; nominally the canon PJO era; see R2). The premise blurb says he returned as a twelve-year-old; the text itself calls him sixteen (Ch7, Ch13, Ch22; see R1). He brings his memories and a sentient battle-suit AI, **Minerva**, with him. The story cuts between that present-day timeline and the far-future **Undying Olympian Empire (UOE)**, about 14,000 years later (UOE year ~16231), where gods rule a galaxy, Percy is a legend, and Minerva has been left behind in a copy of his body. People, gods and AIs exist in several versions across these eras. **Never merge versions.** This file tells you which is which.

Chapters are cited as "Ch N" using file numbers: Ch1 *Rex Imperator I* · Ch2 *Rex Imperator II* · Ch3 *Rex Natus I* · Ch4 *Rex Natus II* · Ch5 *Intermission I* · Ch6 *Rex Natus III* · Ch7 *Rex Natus IV* · Ch8–22 *Rex Invictus I–XV* (Ch8 = RI I … Ch22 = RI XV) · Ch23 *Interlude I*.

---

## Contents
1. How to use these profiles for chatbots
2. The timelines and eras explained
3. Disambiguation tables (every multi-version character)
4. Glossary (factions, ranks, units, tech, places, ships, corporations, AIs, codes, Latin/Greek terms)
5. Plot chronology, Ch 1–23
6. Continuity contradictions (pointer to `00a_CANON_RULINGS.md`, plus items not covered there)
7. Full file index

---

## 1. How to use these profiles for chatbots

### 1.1 What each file contains
Every character file (everything except `00_`, `00a_` and `99_`) follows the same template:
- **Quick Facts**, a table with the version/timeline and the status as of Ch 23.
- **Which Version Is This?**, the disambiguation section. Read this first.
- **Appearance / Personality / Voice & Speech Patterns** (with verbatim quotes) / **Abilities** / **Backstory** / **Story Arc So Far** / **Relationships** / **Secrets & Open Threads** / **Continuity Notes**.
- **Chatbot Card**, the paste-ready part. It has a Description (120–250 words), Personality keywords, Knowledge boundaries, Scenario hooks, an Example first message, Example dialogue and Do/Don't guardrails.

### 1.2 Building a character bot (SillyTavern, Chub, Janitor, Character.AI and similar)
1. **Pick the right version.** Use the tables in §3. "Artemis" alone is ambiguous: present-day Artemis (`C01`) and the future Director (`C02`) know different things and behave differently.
2. **Description / persona field:** paste the card's *Description*. Add the *Personality keywords* to the personality or tags field.
3. **Scenario field:** choose one *Scenario hook*, or write your own that fits the version's era.
4. **First message:** use the *Example first message*, or write a new one in the same voice.
5. **Example dialogue:** paste the *Example dialogue* block. It uses the `{{user}}` / `{{char}}` macros already.
6. **Knowledge boundaries are the most important guardrail.** Put them in the system prompt, author's note or "character note" at shallow depth. For example, present-day Artemis before Ch 11 must not know she marries Percy in the future. Canon-baseline Percy (`A03`) knows nothing of the future at all. Load the relevant rulings from `00a_CANON_RULINGS.md` alongside them (see §1.3).
7. **Do/Don't lines** go in the post-history instructions or author's note.

### 1.3 Using this primer as a lorebook / World Info
Pair any character with this file as world info. Recommended setup:
- **Always-on entry (constant):** a 150–250-word summary of the right era from §2. Use the *present-day* summary for camp characters and the *UOE future* summary for Imperial characters.
- **Always include the canon rulings.** Add `00a_CANON_RULINGS.md` to the lorebook too. At minimum, make one constant (always-on) entry with the rulings that touch your scenario: the age wording (R1), the present-day year (R2), the time figures (R3) and the name spellings (S1–S15). Add the character-fact rulings (C1–C34) as keyword-triggered entries keyed on the names they mention (e.g. `Minerva` → C1/C12/C14/C15; `Eleni` → C2; `Achilles` → C13; `Zoë` → C7/C21). The rulings stop the bot from repeating the story's own slips (Yellowstone, "six thousand years", "Atalanta" for the Hunter, a bare "2005", and so on).
- **Keyword-triggered entries:** make one entry per glossary term in §4 that your scenario is likely to touch. Use the bolded term and its aliases as keys, for example `AtRep, Répertoire, Repertoire`; `Ekdromoi, Kappa-Seven`; `Watchpoint`; `CODE 18`; `Apostolos`. Glossary definitions are written to work as standalone entries.
- **Other characters as entries:** for side characters who appear in a scene but are not the bot, use the *Description* paragraph of their profile, or the 2–6-line entry in `99_Minor_Characters_Compendium.md`, as a keyword-triggered lorebook entry.
- **Group chats:** load each character's card plus this primer. Check §3 so you do not put two versions of the same person in one scene unless the scene is *meant* to be a cross-time meeting. The story itself does this in Ch 16 (the Riptide fragment speaks to present Artemis) and Ch 23 (future Thalia meets Minerva in Percy's body).

### 1.4 Tone and register reminders
- The story mixes **grim military sci-fi** (Warhammer 40k / Gundam flavour: trench war in Tartarus, numbered ranks, codes, mind-integrated ships) with **PJO banter**. Most characters swear casually; Percy is profane in his head.
- **Archaic speech** belongs to Zoë, Chaos, Minerva at times, Eleni ("milord", "thee"), Hrafn, and Percy when he is performing courtliness or bargaining with demons.
- **Minerva** always calls Percy "Varlet". **Artemis** calls him "Perseus". **Eleni** calls him "Milord" or "High Lord". **Annabeth** and **Thalia** call him "Seaweed Brain".
- **Imperial** characters say "Ave Imperator", count time in "Gaian" hours and years, call Earth "Gaia", and speak of the Répertoire's verdicts as law.
- The author's stated intent (Ch1 A/N) is that Percy will drift slowly toward a colder, Fang Yuan-like pragmatism, losing ethics "but still honorable". Up to Ch 23, on-page Percy is mostly merciful and protective. He keeps a few ruthless edges: burning offerings alive (Ch3) and self-surgery (Ch4).

---

## 2. The timelines and eras explained

### 2.1 The two (really three) frames
| Frame | When | What happens there | Typical cast |
|---|---|---|---|
| **Old / original timeline** | The far future, as Percy originally lived it. Ch1 shows its last moments. | Percy grew up, fought the canon wars, became Lord-Commander of the Council of Olympic Sentinels, was abandoned by the gods, and guarded ruined **Olympus Primaris** on a dead Earth for millennia. Chaos finds him and offers a gamble. | `A01` Lord-Commander Percy, Chaos, the old-timeline Hermes, remembered Annabeth (`F02`), Rammael (`G13`) |
| **Present-day ("Rex") timeline** | Present day: c. 2021 per the author's timeline, nominally the canon PJO era (R2). The text gives two anchors that disagree: the Répertoire's Ch3 log reads "As of 2005, August 19th", while Ch19 and Ch22 show the Perseverance rover on Mars. In-story time from Ch3 to Ch22 is about one year: January in Vegas (Ch8), mid-December at Westover Hall (Ch15), then "months" (Ch19). | Percy wakes in his young-teen body (Ch3; nominally twelve, though the text calls him sixteen in Ch7, Ch13 and Ch22, see R1). He runs the canon PJO plots (Lightning Thief → Sea of Monsters → Titan's Curse) in a diverging AU. Future soldiers fall into this era (Eleni Ch15, Kappa-Seven Ch20–22, Marien's 4-million-strong command on Mars Ch19–22). | `A02` Percy, `B01` Minerva-in-head, all `D` present gods, `F` campers, Romans, Hunters, mortals |
| **UOE / future era** | Far future, about **14,000 years** after the present: UOE year ~16231, about 14,200 years later per the author's vault (R3). One continuous "future now" runs through Ch2, 5, 9–15, 18, 19 and 23; the War of Princes (16212–16227) ended a few years before it (R5). Ch20's Octavia section is a separate, much later era: about year 33,000, "thirty thousand years after the rise" of the Empire (R7). | The gods rule the **Undying Olympian Empire**, a galactic, militarised theocracy-bureaucracy with ranked demigods, mind-integrated warships and an endless war in Tartarus. Percy is a myth: the Lord Imperator, Lord of Demigods, Guardian of Gaia, on murals and coins. His body (a vat-grown clone) wakes up in Ch9 and is piloted by Minerva. | `B02` Minerva-Percy, all `E` future gods, `C02` the Director, `C07` future Thalia, `G`/`H` Imperial soldiers and officers |

**How the old timeline and the UOE relate.** In the text they are the same history: the UOE is the galactic empire that grew up while old-timeline Percy stood guard on abandoned Earth. Ch9's soldiers believe Percy is "alone on holy Gaia, clearing out the monsters solo". Ch5's gods detect "an insane spike of energy from a few days ago" in Athena's former palace on Old Earth. That spike is presumably Percy leaving in Ch1 (though Ch1 has Chaos take him from Hestia's courtyard, not Athena's palace). So Ch1, Ch5 and the clone segments are near-contemporaneous, around UOE year ~16231. Ch23 adds a mystery: the Hunt never found Percy's scent in 14,000 years even though he stood guard on Gaia (an intentional mystery, C6).

### 2.2 In-universe chronology (rebuilt on the author's master timeline)
Dates use the vault's absolute calendar ("Gaian reckoning", AD-equivalent). The text confirms the frame: Ch23's packet dates the present to "EARLY THIRD MILLENNIUM, GAIAN RECKONING. PRE-ABANDONMENT. PRE-EXPANSION. PRE-EMPIRE." Dated anchors come from the author's vault and rulings R2–R8 in `00a_CANON_RULINGS.md`; everything else is from the text.

| Approx. date | Era / event |
|---|---|
| Before humanity | Primordial war |
| ~2021 (nominally the canon PJO era) | **Story present**, Ch3–22 |
| 2032 (vault) | Battle of Alaska Hill |
| ~2021–3045 | Percy's long career (old timeline) |
| **3045** (vault) | **Great Abandonment = start of the Great Expansion** |
| Early Expansion | Caligo Vale oathbinding |
| Centuries later | "the council shattered": the Great Cleansing |
| 3045 → 16th millennium | Rise of the Undying Olympian Empire |
| **16212/13–16227** (vault) | **War of Princes** |
| **~16231** (vault) | **The "future now"**: Ch2, 5, 9–15, 18, 19 (future), 22 (Imperial POV), 23 |
| **~33,000** | Ch20 far future (Octavia, Bianca) |

1. **Before humanity:** a primordial war between "gods of energy and star" and "the sentient void". The losers' weapons were sealed in vault-tombs and ossuaries that even Chaos cannot see, though she can make keys (Ch1).
2. **The story present (c. 2021; nominally the canon PJO era, R2):** the Titan and Giant wars. In the **old** timeline Percy lived these as canon Percy did: Lightning Thief, the subjugation of Atlas (Titan's Curse), Battle of Manhattan with Annabeth. In the **new** timeline they are being rewritten from Ch3 on. The text's own date anchors disagree (Ch3's log reads "As of 2005, August 19th"; Ch19 and Ch22 show the Perseverance rover on Mars, and Ch22 has the Lunar Reconnaissance Orbiter circling the moon "since 2009"). The profiles follow the author's c. 2021 and never state a bare 2005 or 2006 as fact.
3. **Mid-2030s (vault: 2032), the Arctic Resource War:** the gods push the US north into Alaska ("In the Mid-2030s", Iane, Ch20) to build, in the cold, the architecture that became AtRep: "AtRep's first cradle" (Straban, Ch22). **Battle of Alaska Hill:** the first extra-pantheonic war in about 2,000 years and the first time demigods fought in modern mechanised war. A son of Poseidon commanded the defence. That was future Percy, with Minerva as Parlamentum Mk.I (Ch20–22). *Author's vault note (not yet in text):* the battle is dated 2032; Percy, Annabeth and Malcolm Pace co-commanded; it is where Minerva first became self-aware ("I do not want to die for him again").
4. **Percy's long career (old timeline):** voluntary surgery to integrate the Aegis Vestments (future Annabeth "really excited", future Chiron "not thrilled", future Athena signed off on the design; Ch19, see C14). He becomes Lord-Commander of the **Council of Olympic Sentinels**, with Annabeth as second-in-command (later "High-Lord-Engineer", "The Architect"). The Olympuses are built: **Primaris** (NYC), **Secundus**, **Tertius/Tertiae**, and **Olympus Mons** on Mars. Rammael Marccusson lands on **Cyrax** (Sirius). Ch23 puts Percy's youth "A thousand years before the Abandonment", which fits the vault dates (R4).
5. **Year 3045 (vault): the (Great) Abandonment, which is the start of the Great Expansion (R4).** The Olympians leave Gaia on the colossal ship *Spear of Zeus* for "new frontiers" (Hermes, Ch1), escaping what Ch5 calls "Gaia's polluted atmosphere". Every other pantheon follows. Amaterasu leaves first on *The Royal Blade of Retribution*; the stragglers glass half the hemisphere with "Morrigan-pattern dreadnoughts". Monsters from Tartarus and "millions of accursed realms" overrun Earth. Percy is left behind on Gaia to guard it (vault; Ch1 shows the result). Ch12's future Minerva ties the two events together: "since the beginning of The Great Expansion and your abandonment many millennia ago".
6. **Early in the Great Expansion: the Caligo Vale oathbinding (R8).** The Olympian Court is crumbling and "The Empire needed a stabilizer" (future Artemis, Ch13), so Percy, already the Guardian of Gaia, is politically bound to **Artemis at Caligo Vale**, a site "chosen by Hera on a whim" (Ch13). The pair are "immortalized together in marble on Caligo Vale" (Eleni, Ch15). This is never before the Abandonment. Eleni's cult lore says Artemis wept "when he was re-exiled into the Lands of our Birth, Gaia" (Ch15). *Author's vault note (not yet in text):* the rite was held on Olympus Tertiae and invoked by Hera under duress; Percy was mind-wiped hours later and sent back to Gaia; Him Within the Moon began forming at the oathbinding.
7. **The Great Cleansing:** Chaos says "the council shattered merely centuries after…" and names it "what you would call The Great Cleansing" (Ch1). Which council is unstated. The context ("my great-grandchildren would have been wise to incorporate your presence") favours the gods' own Olympian council, and Ch13 has the Olympian Court "crumbling". Percy hates "the Divinities that play it". Details are unknown.
8. **The Undying Olympian Empire (3045 onward):** the gods take star dominions; demigods are ranked on a **Unified Leaderboard**; Tartarus becomes an open war front. *Author's vault note (not yet in text):* in 3045–3048 Poseidon claims the Thalassus Belt (New Atlantis), Athena launches the Répertoire around Parlamentum Mk.III, and Artemis takes the UOE's moons and the Gaia orbital platforms.
9. **War of Princes, 16212/13–16227 (vault, R5):** a civil war in which the **Princes**, founders of the **Voss Sovereignty**, rebelled because "the gods had diluted them, overruled them and ignored them" (Ch23). Apollo's sons and last legions died at its Final Battle. The Princes' wartime ally was the **Amaterasu Dominion** (C5); Kagura Kuroyami reactivated the Yamamoto relay "on December's Eve of 16215" (Ch23). It ended at the **Treaty of Mount Rümker** in a draw (Ch23); the vault dates the treaty to 16227 and calls it a UOE tactical victory ratified at Tears of Lysandra. Ch23's "Quite a few years earlier" is correct; Ch5's "a few millenia past the War of Princes" and Ch15's "millennia ago" are slips (R5).
10. **The "future now", ~16231 (Ch2, 5, 9–15, 18, 19, 22 Imperial POV, 23):** border skirmishes between divine-parent factions (Zeus vs Dionysus/Poseidon/Aphrodite); Percy's departure spike; Minerva's awakening in the clone; the Hollow Crescent cult attacks Luna; the Tartarus front loses about 50 million demigods a year; Marien Pyrrhus's echelon is sheared into the past (Ch19); the Empire reacts (Ch23). This is about 14,000 years after the story present (vault: about 14,200; R3).
11. **About year 33,000 (Ch20, Octavia; R7):** "thirty thousand years after the rise" of the Empire, a separate, later era from the UOE scenes. Gaia is a quarantined radiation graveyard. A godlike "Bianca Di'Angelo" waits under Everest.

### 2.3 How people cross between eras
- **Percy (mind)** goes from the old timeline into his present-day young-teen body (Ch1→3), via a wispy transit form.
- **Minerva** comes back inside Percy's integrated armour remnants (`B01`). A *second* Minerva wakes in Percy's future vat-clone (Ch9 end → Ch10 onward; `B02`). By Ch23 the two are distinct "sister" copies who talk through the Mars Watchpoint's "echo carrier".
- **Dream-walking:** while asleep, present Percy's consciousness slips into future bodies. First anonymous Imperium telekhine soldiers (Ch8–9), then the clone on a battlecruiser bridge (Ch11) (`A04`).
- **Him Within the Moon / Riptide fragment:** a shard of future Percy formed from future Artemis's energy and the lost Anaklusmos inside Luna. In Ch13 it says "My Original is calling me. Back there. In the past.", and future Artemis lets it go ("Then go to him, Anaklusmos"). *Author's vault note (not yet in text):* it formed inadvertently at the Caligo Vale oathbinding. In Ch14 Riptide transforms, with Zoë's ghost blooming over it; in Ch16 the sword speaks to present Artemis (`A05`).
- **Eleni Theodosia:** a future daughter of Zeus, apparently killed in Ch2. She comes out of Thalia's tree alongside Thalia (Ch15) and is displaced into the present (`G01`).
- **The shear (Ch19):** a "subreality dematerialization event" near the Phlegethon in Tartarus takes everything within 11 km of a transit anchor back in time. About **4 million** soldiers of the **Pyrrhuiesian Command** (its Reserve Echelon, C7) land on **Mars** in the present era under Senior Commander **Marien Pyrrhus** (`G02`). Kappa-Seven (`G04`–`G09`) is sent to Earth from there.
- **Future memory bleed:** present Artemis steals a mass of Percy's memories (Ch11), then dreams of the future (Ch15). By Ch19 the narration calls her "a being who remembers centuries yet to come". Present Athena reads Minerva's architecture (Ch19).

### 2.4 One-paragraph era summaries (for always-on lorebook entries)
**Present-day (c. 2021 per the author's timeline; nominally the canon PJO era):** Percy Jackson is outwardly a young teenage son of Poseidon, but inside him lives the mind of a millennia-old future Lord Commander. An AI called Minerva lives in his bloodstream, Lycaon's heart beats in his chest, and future armour (the Aegis Vestments) is built under his skin. He is reliving the PJO quests with future knowledge and changing them. He won the Master Bolt from Ares, took the Golden Fleece, and held the sky for Artemis. Artemis is now bound to him and has named him her **Apostolos**. Through the story the Olympians, Camp Half-Blood, the Roman legion (Reyna and Jason) and the Hunters of Artemis learn that soldiers of a far-future Olympian Empire are falling into this era. By Ch22 about 4 million are on Mars, and their AI has named Percy **Lord Imperator**. Olympus signs the **Anabasis Accord** with them while Kronos and Luke gather an army.

**UOE future (~14,000 years on, UOE year ~16231):** The Olympian gods rule the Undying Olympian Empire, a galaxy-spanning, militarised, bureaucratic theocracy. Demigods and legacies are conscripted, ranked by number and bloodline index, wired into warships, or fed into an endless trench war in Tartarus. Athena's AI, the Répertoire du Savoir Athénien (AtRep), issues binding "verdicts". Artemis is the Director of Anti-Espionage and Celestial Surveillance; Aphrodite commands hospital fleets as "Mother Majesty". Percy Jackson is a myth, the Lord Imperator and Lord of Demigods, venerated by a heretic cult and by ordinary soldiers. Minerva walks around in his cloned body. Rival powers include the Voss Sovereignty, the Amaterasu Dominion, the Jade Court, Norse houses, demon lords and mega-corporations such as Hadrian.

---

## 3. Disambiguation tables

### 3.1 Percy Jackson (six files)
| File | Version | Era / where | Body & state | What he knows | Quick tells |
|---|---|---|---|---|---|
| `A01_Percy_LordCommander_OldTimeline.md` | Lord-Commander Perseus Jackson, the original sentinel | Old timeline, Ch1 (transit start Ch3); remembered throughout | Adult, millennia old, scarred, in a rusting Hephaestus exosuit; mechanical right pinkie; Regen-ex at 0.000114% | Everything up to the Abandonment and his millennia alone; the Great Cleansing; nothing of the new timeline | Exhausted, bitter toward the gods, courtly with Chaos ("Milady Khaos"); holds xiphos and the banner of Olympus |
| `A02_Percy_Reincarnated_Rex.md` | "Rex" Percy, the protagonist | Present day, Ch3 → Ch23 | Young-teen body (premise blurb: twelve; the text calls him sixteen in Ch7, Ch13 and Ch22; see R1); Lycaon's heart; internal Aegis Vestments and nanomachines; Minerva in his blood; Achilles curse at about half strength after he gives fragments of it to Artemis (Ch18–19; C13) | All future memories, which he rations; becomes Artemis's Apostolos (Ch19) and is named Lord Imperator by the Watchpoint (Ch22) | Snarky, weary, merciful; "Varlet" to Minerva, "Perseus" to Artemis, "Milord" to Eleni |
| `A03_Percy_Canon_OriginalSelf.md` | Canon Percy, the original young Percy (twelve in canon) whose life Rex overwrote | Present day, implied only (Ch3); canon baseline clearly labelled | Normal troubled Yancy kid, cartoon-seal blanket | Nothing of the future | "Coming mom, just gimme a second"; sleeps in class; unfinished homework |
| `A04_Percy_Dreamwalker_Psychic.md` | Present Percy's sleeping mind in future bodies, called "Psychic" | Future (Ch8–9, Ch11) | Anonymous telekhine soldiers (Hydrokinetic shieldstaff Mk. MCLIX); then the vat clone on an AnnChase battlecruiser throne | Present Percy's mind, confused about where it is | Dies and is moved into a new body ("Seeking replacement…" / "Integrating…", Ch8); "Ave Imperator!"; is greeted as "Lord of Demigods. Guardian of Gaia" |
| `A05_Him_Within_the_Moon.md` | Him Within the Moon / Moonbound / the shard / "Anaklusmos"; Riptide's sentient fragment | Future Luna core (Ch12–13) → present Riptide (Ch14, 16) | Translucent blue-gold-silver giant, face flickering "like a glitched memory file"; later a voice in the sword | Fragmentary; calls Rex Percy "My Original" | "Always." / "We are what Perseus becomes" |
| `A06_Percy_The_Legend_Lord_Imperator.md` | The Empire's mythologised Percy | Future lore (Ch2, 9, 13, 15, 22, 23) | Murals, statues ("The Two"), coins, Core Commandment 14, CODE 15, cult hymns | n/a (a legend, not a speaker) | "Perseus Jackson, the greatest of us all"; "Lord of Demigods"; "Perseus the Blessed King" |

Not separate files but related:
- **Percy's transit form** (Ch3, wispy, phasing through birds) and his **mindscape fragments** (Ch11) are covered inside `A02`.
- **Minerva wearing Percy's body** is `B02`, not a Percy file.
- **Pre-Ch1 future Percy's deeds** (Alaska Hill, Caligo Vale, the surgery) are covered in `A01` and `A06`.

### 3.2 Minerva and the Athenian AIs
| File | Entity | Era | Body | Voice / tells |
|---|---|---|---|---|
| `B01_Minerva_In_Percys_Head.md` | Minerva, Parlamentum Alpha Mk.1, the AI of the Aegis Vestments | Present (Ch3/4 as the hidden log → named Ch6 → dormant Ch12–18 → reactivated Ch19 → Ch22) | None. Lives in Percy's blood, brain, spine and soul. Can manifest as a silver-blue nanoparticle bust or speak through sound systems or through Percy; turns his eyes neon-blue | "Varlet"; "Recommendation:", "Correction:"; issued CODE 2 against Percy's order (Ch22) |
| `B02_Minerva_Percy_Clone_Interlude.md` | "Minerva Percy", the copy left in the future, piloting Percy's vat-grown clone | Future (wakes end of Ch9, Ch10–15; Interlude Ch23) | Percy's exact body; neon-blue eyes when Minerva is in control (her signature), sea-green as the body's natural eyes; Ch13's "golden" is an outlier (C1); sometimes wears an illusion to look less like him | Clinical in Ch10–15 ("Estimated usefulness: negligible"); by Ch23 dry and quippy ("a very old piece of software wearing a very handsome boy"); calls Thalia "Pinecone Face" |
| `B03_AtRep_Repertoire_du_Savoir_Athenien.md` | The Répertoire du Savoir Athénien (AtRep, RDSA, "Sister"), the main branch; plus the "Host" interface (Ch3–4), **Athena's shard** on Quarterdeck 19 (Ch14), and the **Watchpoint fragment** at Jezero, Mars (Ch19, 22) | Future-wide; the fragment is in the present on Mars | Systems-sized hardware; the Watchpoint is a slowly turning column of pale gold light | ALL-CAPS VERDICTS; "Ave Imperator"; "I have no sisters" |

Note: Ch3–4's Répertoire with its hidden "Anti-Host" consciousness log is the embryo of Minerva. `B01` and `B03` both discuss it.

### 3.3 Artemis / Diana
| File | Version | Era | Tells |
|---|---|---|---|
| `C01_Artemis_Present.md` | Present-day Artemis | Ch3–22 | Auburn hair (silver in one Ch16 line), silver eyes. Scorns males, then wipes Percy's memory (Ch11), then is bonded to him through his offering (Ch18). Names him **Apostolos** (Ch19). Possessive and tender; catches a bullet for him (Ch22). Has future-memory bleed. Calls him "Perseus"; he calls her "Arty" once, privately (Ch22), and Apollo (Ch19) and future Poseidon (Ch15) also use the name (C11). Bitter that "Some future me" has sealed the date of Zoë's death from her (Ch22). |
| `C02_Artemis_Future_The_Director.md` | Future Artemis, **Director of Anti-Espionage and Celestial Surveillance**, Percy's (political) wife | Ch5 (red-haired, lazy on her throne), Ch13 (Luna, Him Within the Moon), Ch23 (seals Zoë's death date); also the **crimson-haired vision** of Ch14 | Weary, buried grief. Keeps a scrap of blue cloth with Percy's scent; her Hounds have hunted that scent for 14,000 years. Aphrodite calls her "sister-in-law". |
| `C03_Diana_Roman_Aspect.md` | Diana, a separate Roman consciousness sharing Artemis's domain | Ch11 (surges, "Sister! Where?", when Chiron says "Minerva"; whether at the name or at the AI aboard is unstated; then suppressed brutally), Ch17 (Zoë introduced as an "agent of Diana"), Ch18 (exhausted, recuperating) | Barely seen; reacts to Minerva as kin |

### 3.4 Zoë Nightshade
| File | Version | Tells |
|---|---|---|
| `C04_Zoe_Nightshade_Present.md` | Present Lieutenant of the Hunt (Ch4 onward), including her ghostly corona over Riptide (Ch14) | Archaic speech ("Speaketh thy mind"); calls Percy "Freak". In this timeline she survives Othrys because a Hesperide is killed by Atlas's own bolt instead (Ch19; C19). Kills Sabine Ro (Ch22). |
| `C05_Zoe_Nightshade_Future_Legend.md` | Future legend: "Eternal Hunter Princess" (Ch1, probably), "Oldest Hunter of the Director, First of her Lieutenants", her name on "the Wall"; archived record sealed (Ch22–23) | Her archived record is *sealed*: no Imperial may disclose "THE DATE OR MANNER OF HER DEATH TO ANY PARTY, INCLUDING THE DIRECTOR, IN ANY EPOCH" (Ch23; C7). She is alive in the story present (C21). |

### 3.5 Thalia Grace (and a look-alike name)
| File | Version | Tells |
|---|---|---|
| `C06_Thalia_Grace_Present.md` | Present Thalia. A dying pine (Ch12–13) until the Fleece revives her (Ch15) | Punk, profane; teases Eleni ("young Thunder-Sister"); calls Artemis "a proper bitch" (Ch15) |
| `C07_Thalia_Grace_Future_Lieutenant.md` | Future immortal Lieutenant of the Hunt, ~14,000 years on (Ch13 Luna; Ch23 Voss chase) | Armour bristling with capacitors (Ch13); travels as lightning at 299 km/s (Ch23); afraid of heights; yells "JACK-SON!" |
| (in `H16_…`) | **Commander Thaleia**, Tartarus-front commander, Lethe Sector, Depth 74-B (Ch14) | **Not linked** to Thalia Grace in the text. Treat her as a separate person. |

### 3.6 Bianca di Angelo
| File | Version | Tells |
|---|---|---|
| `C08_Bianca_di_Angelo_Present.md` | Present-day Bianca, a new Hunter and quester (Ch15–19) | Untrained arrows; Flamel smells "sulfur and brimstone" on her |
| `C09_Bianca_DiAngelo_FarFuture.md` | "Bianca Di'Angelo" under Everest on dead Gaia, about year 33,000, "thirty thousand years after the rise" of the Empire (Ch20; R7) | Godlike, haughty ("my esteemed self"); pale blue fire in her eyes; beat dozens of UOE soldiers; identity unresolved |

### 3.7 Annabeth Chase and her echoes
| File | Version | Tells |
|---|---|---|
| `F01_Annabeth_Chase_Present.md` | Present daughter of Athena (Ch7 on). Note: in **Ch8** a fake Annabeth is Athena in disguise (see `D03`). | Suspicious, bossy, "Seaweed Brain"; the Fleece rejects her (Ch14) |
| `F02_Annabeth_Chase_Future_Architect.md` | Old-timeline Annabeth: Percy's ex, Second-in-command of the Sentinels, "High-Lord-Engineer", "The Architect"; designed Parlamentum Mk.I's hardware and secretly switched the suit's nectar cooling to Lethe water (Ch5); championed the Vestments surgery (Ch19). She did not design the suit or the Vestments (C14); namesake of the AnnChase-pattern ships; half of the statue "The Two" | Seen only in the Ch5 flashback and in memories |
| `F03_Verrill_Chase.md` | **Not Annabeth.** A far-future Chase legacy (~20) who looks *exactly* like her (Ch23) | Pencil in her hair-knot; Minerva's new partner |

### 3.8 The Olympians: present vs future
| God | Present-day file | Future (UOE) file | Main tell of the future version |
|---|---|---|---|
| Zeus | `D01_Zeus_Present.md` | `E01_Zeus_Future.md` | Head of the "Imperiality of Zeus"; his "Firstborn Million" children; cannot remember their names (Ch5); "Roar of Clouds" |
| Poseidon | `D02_Poseidon_Present.md` | `E02_Poseidon_Future.md` | "The Master" of New Atlantis / Nereid Expanse; grieving; calls Minerva "Impostor"/"Minnie"; "Die well, nephew" (Ch15) |
| Athena | `D03_Athena_Present.md` (includes disguised-as-Annabeth, Ch8) | `E03_Athena_Future_Parthenos.md` | Atrytone/Parthenos aspects; Parlamentum Mk.3; runs the Répertoire; forged Percy's key |
| Apollo | `D04_Apollo_Present.md` | `E04_Apollo_Future.md` | Solar Auxilia; Apollonian Hospitalier; lost his sons in the War of Princes |
| Hermes | `D05_Hermes_Present.md` | `E07_Hermes_Future_Clepsiphron.md` | The old-timeline Hermes of the Abandonment (Ch1); swears by "Hermes Clepsiphron" |
| Ares | `D06_Ares_Present.md` (Huitzilopochtli/Mars Ultor aspects, Fort Reagan) | `E08_Hera_Ares_Hestia_Demeter_Future.md` | "Beside himself" over Deimos (Ch5); worshipped through the Imperial Mars catechism by future soldiers (Ch22). (Patron of the Mars garrison under the Accord is a *present-day* role, `D06`; C33.) |
| Dionysus | `D07_Dionysus_MrD_Present.md` | `E06_Dionysus_Future.md` | Hawaiian-shirt drunk at the conference (Ch5); sponsors the Dionysian mercenary division; at war with Zeus's borders |
| Hera | `D08_Hera_Present.md` | `E08_…` | Chose Caligo Vale "on a whim" |
| Hephaestus | `D09_Hephaestus.md` (both eras) | — | Forge of Hephaestus builds the AnnChase ships; dyson-sphere automatons |
| Hades | `D10_Hades.md` (both eras) | — | Future: holds Tartarean containment lines with the Director |
| Hestia | `D11_Hestia.md` | `E08_…` | Old timeline: her courtyard is where Chaos waits (Ch1) |
| Demeter | `D12_Demeter.md` | `E08_…` | Old timeline: "empty, salted fields" |
| Aphrodite | `D13_Aphrodite_Present.md` | `E05_Aphrodite_Future_Mother_Majesty.md` | Veiled, with a neural wire into her throne; Dove's Fleet; "Mother Majesty" |

Other divine beings with era notes: Iris and Fleecy `E11` (present; Iris cameras in the future), Hecate `E12`, Triton `E10` (present Helmsman-to-be; future "Lord Regent"), Kronos `E14`, Atlas `E16` (Titan's Curse), Porphyrion `E17` (future Tartarus), Chaos `E13` (old timeline/beyond time).

### 3.9 Other easily confused names
| Name(s) | Who is who |
|---|---|
| **Eleni Theodosia** (`G01`) | One person, two settings. Ch2: commander of the *Divine Crusader*, presumed dead; Ch5: Zeus mourns her. Ch15 onward: displaced into the present as Percy's bodyguard. |
| **Lord Varro** (`G11`) vs **Archmagister Cael Varros** (`H15`) | Varro is the Overseer of the Legio Administratoris in the 12th Olympian Reach (Ch10, 22, 23). Varros is an 812-year-old logistics officer on Quarterdeck 19 (Ch14). No link is stated. |
| **Callidora of the *Eternal Glory*** (`G12`) vs **Stephanie Callidora** (`H06`) | Ch2's coalition commander vs Ch23's Helion Bulwark of Aphrodite, flagship *Sovereign's Glory* (also a Ch2 ship name). Not stated in the text. *Author's vault note (not yet in text):* the Callidoras are a family; **Elektra Callidora** (demigod of Aphrodite) is Stephanie's mother, and the vault assigns the *Sovereign's Glory* to Stephanie as early as the War of Princes, so the Ch2 *Sovereign's Glory* is most likely hers. The Ch2 "Callidora of the Eternal Glory" is unassigned in the vault (possibly Elektra or Stephanie). |
| **Stephanos Pyrrhus** (`G03`; text variants "Pyrrus"/"Phyrrus", S1), **Marien Pyrrhus** (`G02`), **Nikos Pyrrhus** (`G03`) | Stephanos: Poseidon's demigod, Grand Commander of the *Waves of Poseidon* (Ch2), "liege" of the mech Titans (Ch12). Marien: his child, Senior Commander, sheared to Mars. Nikos: an A/N-only planned OC. |
| **Kagura Kuroyami** (`H11`; called "Perseus Kuroyami" in Ch5) | One person (S4): the Shinto emissary of the Amaterasu Dominion tied to the Yamamoto Chokepoint Relay. Ch5's "Perseus" is a probable slip. *Author's vault note (not yet in text):* the Dominion's chief engineer and, during the War of Princes, Amaterasu's apostle. |
| **Justicar Themis** (Ch5, `H12`), **Themis the Titaness** (myth), **Solon Themis** (Ch23, `99_`) | A male demigod judge with jurisdiction over Voss; the Titan goddess; the Voss magnate who built the Themis Needle. *Author's vault note (not yet in text):* Solon Themis was the **first** Justicar of the Voss System and the Princes' second-in-command, now entombed in Voss I "waiting to be revived by Apollo" (planned). The Ch5 Justicar is either Solon or a successor holding the office and name; the text does not say. |
| **Jason Grace** (`F16`) vs **Jason the Argonaut** | Ch23's statue on the Via Heroum is "the first" Jason, the one Thalia's brother was named after. |
| **Michael Yew** (`F10`, dies Ch22) vs **Michael Black** (`H06`, Selenide Bulwark of Aphrodite, Ch23) | Unrelated. |
| **Naomi** (Hunter) | The Ch4 present-day Naomi vs the Ch23 future Naomi, a legacy of Raijin who joined 300 years before. Thalia reacts to the name as a "namesake". See `C12`. |
| **Atlanta** vs **Atalanta** | **Atlanta** is the author's spelling for the Hunter, daughter of Apollo and the Hunt's apothecary (`C11_Atlanta_Hunter.md`; present Ch4, 6, 16 and future Ch23). **Atalanta** is only the mythic heroine among the Via Heroum statues (Ch23). Not a typo (S2). |
| **Legio XII Fulminata** | Reyna's present legion (`F15`/`F17`) and the future "Thunderbolts" of the Tartarus Salient (Tullia Ardens, `H01`). The same legion across time. |
| **Legio Valeria Vitrix** (Ch9) / **Legio XX Valeria Vitrix** (Ch21) | Dream-Percy's future legion (Ch9) and the Callistus levy target (Ch21). Probably the same legion. Text and vault both spell it **Vitrix** (S9; Latin would be *Victrix*). |
| **Huitzilopochtli** | A taunt name for Ares (Ch10, `D06`) vs the real Aztec god who arrives in Ch22 (`E18`). |
| **Riptide / Anaklusmos / "Zoë's sword"** | The physical sword (`A02`) vs the sentient fragment inside it (`A05`). Him Within the Moon is called "Anaklusmos" by future Artemis. |
| **"Sister"** | Gods use it for each other (Athena/Artemis). Minerva uses it for AtRep and the Watchpoint. Dionysus calls Minerva "mini-Sister". Ch7 Percy: "she sounds like Sister". |
| **"Lord Commander"** | Percy's old title, and also **Varric von Romhardt**'s rank (`H08`, Ch15). |
| **"Twins"** | Ch13's Hollow Crescent "Twins" are unnamed on the page; per the author's vault they are very probably **Orran and Virre Arenberg** (C23). The Stolls are "brothers" and the di Angelos and the Graces "siblings" in descriptive prose (C22). |
| **Thaleia** vs **Thalia** | Commander Thaleia (Ch14, `H16`) is a different person from Thalia Grace (S7). |
| **Demetrius Ikaris** (`H14`) vs **Demetrius Lykourgos** (A/N OC) | Ikaris is the limbless Poseidon legacy wired into the *Blood Martyr* (Ch11). Lykourgos is a planned OC name only. |

---

## 4. Glossary
Alphabetical within each section. **(P)** = present-day era, **(F)** = UOE/future, **(O)** = old timeline, **(A/N)** = author's note only, not yet in the story.

### 4.1 Polities, factions, houses and organisations
- **Aldra** (F) — Olympian liaison service. Two "Aldra liaisons", "Olympus's eyes", watch Civil Port Nine on Voss Secundus (Ch23).
- **Amaterasu Dominion** (F) — the majority power of the Shinto pantheon, led by Amaterasu. Diplomat Kagura Kuroyami (called "Perseus Kuroyami" in Ch5; S4). Wartime ally of the Princes' Voss Sovereignty in the War of Princes (C5). "Pays in favors" (Talviento, Ch23).
- **Athenian High Command** (F) — Athena's command structure, which speaks through AtRep (Ch15).
- **Augusti** (F) — a Roman-legacy crime clan that runs New Rome's casinos (the Bakuto). Patriarch Augustus, enforcer Talviento; their fighters are "Slag-knights" (Ch23).
- **Bloodline index** (F) — the Imperial classification of mixed divine descent, e.g. "Hermes-Mars", "Poseidon-Zeus", or a Legacy "with Demeter-Dionyosian [sic] lineage diluted through four generations" (Ch19).
- **CarniVoles** (F) — a worse New Rome gang that sells brain-ark to minors (Ch23).
- **Chase Dynasty / the Owls** (F) — the far-future Chase legacy line of Athena and the engineering guild that built half the northern relays and almost every tachyon relay (Ch23).
- **Citadel's children, Cohors Praetoria, PCA, Extra-pantheonic** (F) — factions Straban lists when trying to place Percy (Ch22). Otherwise unexplained.
- **Council of Olympic Sentinels (C.O.S.)** (O) — the demigod order guarding Earth's Olympuses after the Abandonment. Percy is Lord-Commander and Annabeth second-in-command. The "First Council" remnants guard Secundus and Tertius. Chaos says "the council shattered" in the Great Cleansing (Ch1), but which council is unstated; the context favours the gods' Olympian council (see §2.2 item 7).
- **Council (Olympian Council / Olympian Court)** — (P) the twelve Olympians in session. (F) the Olympian Court "crumbled" before Caligo Vale; future "Divine Lords of Olympus Tertiae".
- **Dionysian Division / Dionysian Contractor units** (F) — Dionysus-sponsored mercenaries: conscripted legacies in violet plate with gold filigree and ivy decals, billed by kill-cost (Ch18).
- **Dove's Fleet / Dove's Detachment** (F) — Aphrodite's fleet, with white-and-gold chevrons (Ch23).
- **Evergreen Family** (P/F) — a power "that sought to control both Heaven and Hell". Its spies infiltrate the demon lords and will collapse them "a few millennia later". It survives into the far future ("Evergreen pilots", Ch18; a branch manager, Ch20). Possibly elvish (compare the A/N's Elowen Greenwood).
- **Four families** (F) — the crime syndicates of New Rome, Voss Secundus. The Augusti is the fourth (Ch23).
- **Hollow Crescent, Order of the** (F) — a heretic cult that wants to wake "Him" (Percy) inside Luna, led by "the Twins" (unnamed on the page; per the author's vault very probably Orran and Virre Arenberg, C23). It captured the *Eye of Light*; Luna-Secundus fell to it with the Arenbergs' help (Ch12–13). Its creed: "He shall grant us freedom from the uncaring gods."
- **Hunters of Artemis / Hunt of the Director** — (P) Artemis's maiden band, ~40 strong. (F) a military order with the 6th Moonwall, shieldmaidens, flame hunters, sister-augurs and the Hounds of Artemis from the Luna kennel-crypt. Children have posters of them (Ch23).
- **Imperiality of Zeus** (F) — Zeus's realm, "first under Olympus". It has the Steel Legions and the Third Lance battlegroup; Zeus's children are the "Firstborn Million" and the "Sacred Hundred" (Ch15).
- **Jade Court** (P/F) — the Sino-pantheonic house of cultivators, with the Book of Life and Death and crane-winged judges. "Pays in years." In Ch22 it converges on Kappa-Seven's Alaska dropship.
- **Legio Administratoris** (F) — the administrative legion for reassignment, records, pensions and the Wall. Lord Varro is its Overseer of the 12th Olympian Reach.
- **Legio XII Fulminata** — (P) Reyna's legion at Camp Jupiter. (F) "the Thunderbolts", a heavy Tartarus-front legion with lightning-bolt helmets and a "Golden Standard" ability. Article VI of the Accord makes it the Command's Earth partner.
- **Legio XX Valeria Vitrix / "Legio Valeria Vitrix"** (F) — the legion of dream-Percy's soldier bodies (Ch9), and the levy target on Callistus (Ch21). Text and vault both spell it **Vitrix** (S9). *Author's vault note (not yet in text):* "(Victorious Valeria) raised by Octavian 31 BC".
- **Legio XXI Rapax** — a historical Roman legion "sworn to the Octavian of old", founded 31 BCE. Percy claims citizenship and past command in it (Ch17); Jason says "That legion is gone."
- **Luciferian demons** (F) — rumoured by the Shinto to be plotting to reform Old Earth (Ch5).
- **Other houses** — the non-Olympian pantheons: Aztec, Norse ("ravens of the north"), Jade Court, Shinto, Egyptian, Irish. Huitzilopochtli warns that they "are watching" (Ch22).
- **Princes, the** (F) — the rebel leaders of the War of Princes, "cunning", "utterly hated" by Poseidon. They built New Rome's Via Heroum out of spite (Ch15, 23).
- **Pyrrhuiesian Command / Pyrrhus dynasty** (F) — Poseidon-descended military dynasty, strong in the rankings. Eleni calls them Percy's "half-brothers". It commands the ~4 million sheared to Mars. Its Reserve Echelon, Second Rotation, was lost into the shear and reclassified MIA (Ch19, 22, 23; C7): per Ch23, Cohors III, Cohors VII, support and the carrier group, 3,998,050 in all.
- **Rattlebone Rustabouts** (F) — a gang of "divine junkie" double-bloodline legacies in the Kilns of New Rome, wiped out by Minerva (Ch23).
- **Roman Triumvirate Holdings / "the Triumvir"** (P) — "The Roman Triumvirate Holdings" is hunting the questers with "A King's ransom. Each." (Asmodeus, Ch17; ~100 gold talents, ~$430M per head). "The Triumvir" are Robespierre's masters (Ch17). Probably the same faction. Its nature (mortal or otherwise) is not stated.
- **Shinto task group** (F) — lacquered hulls, torii pylons, Tian-Qiang orbital batteries; defended by a Miko (Ch18).
- **Solar Auxilia** (F) — Apollo's security fleet orbiting Gaia and Sol.
- **Steel Legions / Third Lance** (F) — Zeus's military, which Eleni served in.
- **Theodosians** (F) — Eleni's dynasty of Zeus, rivals of the Pyrrhus dynasty with frequent border clashes. Ekdromoi treat a Theodosian with suspicion ("traitor").
- **The 32nd** — Asmodeus's rank and faction (the 32nd Demon Lord).
- **Underlane Regulars** (F) — a tram collective in New Rome's war tunnels (Ch23).
- **Undying Olympian Empire (UOE)** (F) — also "the Undying Empire", "Greco-Roman Empire", "Imperium". The future galactic empire of the Olympians, "the largest power humanity has ever built". Salute: "Ave Imperator". Laws: the Undying Laws (Law 9 forbids negotiating with foreign pantheons over time; Law 14 binds personnel to silence; Section 12 covers levies).
- **Voss Sovereignty** (F) — three stars and three Dyson spheres, ruled by corporations, councils and the Princes. Capital world Voss Primaris; colony Voss Secundus. By treaty no god may hold governance there, so there are no Watchpoints and no Director surveillance (Ch23). A **former rebel state**: the Princes founded it, and in the War of Princes (16212–16227) its ally was the Amaterasu Dominion. After the Treaty of Mount Rümker it is autonomous and restricted, and at peace with the Empire. Ch5's "the Voss Sovereignty and their allies, the Undying Olympian Empire" is diplomatic courtesy, not a military alliance (C5); in Ch5 it is under the jurisdiction of Justicar Themis. *Author's vault note (not yet in text):* the first Justicar of Voss was Solon Themis, now entombed in Voss I.

### 4.2 Ranks, titles and unit types
- **Aedificator / aedificatori** (F) — Apollonian technician-healers who charge drachmae. Percy slips into the word "Aedificatori" in Ch18. Also "aedificatori bays" (engineering/medical fabrication).
- **Apostolos / Apostle** (P) — the new office Artemis gives Percy in Ch19: he answers to her alone, acts on her authority, and is her intermediary with outside factions, with no authority inside the Hunt.
- **Archmagister / Magister** (F) — logistics-bureaucrat ranks (Cael Varros, Ch14).
- **Augur / Battle-Augur / augur crews** (F) — officer-priests and sensor or communications officers. Some are blind priests (Ch9); they kneel to dream-Percy (Ch11). "Augur feed" means the sensor/HUD network. "Sister-augurs" serve in the Hunt.
- **Autokrætor / Rex / Basileus ("Baselius")** — Percy's old imperial titles: "Autokrætor Rex Perseus Jackson". Chaos calls him "Rex Graecus".
- **Bulwark / Spear (Helion / Selenide)** (F) — paired guardian ranks held under any UOE god, not ranks unique to Aphrodite (C25; vault: "Primary defensive servants" of a god, each paired with a twin). Helion = sun/gold, Selenide = moon/silver; Bulwarks guard, Spears attack. Aphrodite's four appear in Ch23; Eleni claims a provisional "Selenide Bulwark for Lord Phoebus Apollo" (Ch22).
- **Castellan** (F) — the leader of an Ekdromoi cell (Castellan Oriel).
- **Centurion / Decurion / Primus Pilus / Signifer** — Roman ranks used in both eras. Primus Pilus is the senior centurion (Tullia Ardens); Signifer is the standard-bearer (Lucan Corvo); Decurion is a cavalry officer (Herrman).
- **Director of Anti-Espionage and Celestial Surveillance** (F) — future Artemis's office. Seal: a crescent moon. Present Artemis takes the title as the Council's liaison in Accord Article V.
- **Ekdromoi** (F) — black-division special operators in five-person cells (Kappa-Seven, Lambda-Two, Sigma-Four). They carry suppression locks, Divine Stimulants, Pariah Fields, MORROW-IX rifles and QVARTUS rounds, and breathe perfluorocarbon. Classed as CODE 24E.
- **Firstborn / Firstborns** (F) — direct demigod children, conscripted for Tartarus. Their minds are "sealed, filtered, and cleaned of anything not sanctioned by Athena" and they have no sense of taste. Approval category: "Mind-Shard Ascension". Firstborn cadets queue in the Asphodel Colony.
- **Handler** (F) — the officer who commands a task force or a Trophimoi "echo" (Handler Corvin).
- **Helmsman** (F) — a son of Poseidon that the Imperials "reweld into the ship's nervous system" as its pilot (Ch19). Marien's two Helmsmen died "Over sixty years of service" (Ch22). Article IV makes Triton the Helmsman. *Author's vault note (not yet in text):* any direct descendant of Poseidon (child or legacy) can serve, lobotomised and with limbs amputated; Demetrius Ikaris (`H14`) is a legacy.
- **Hermesean blood / logistical caste** (F) — conscripted Hermes descendants who serve as unarmed runners (Logos Petronius-11). Hermes legacies have a "Relay Voice" that can pass data to AtRep.
- **Legacy** (both) — a descendant of a demigod. "Legacy human" in Imperial classification means unindexed pre-Empire tech. "Second-born" means a legacy (grandchild), e.g. "a second-born of Ares" (Ch8). Note that Ch23 calls Augustus "a Second-Born demigod in the Princes' service"; *Author's vault note (not yet in text):* Second-Born demigods are legacies raised to demigod status (16212) and are Empire loyalists, so Augustus's Princes service is a known tension (00a §5).
- **Lord Commander** (F) — a high field command (Varric von Romhardt). It was also Percy's old rank.
- **Lord Imperator** (F) — Percy's highest Imperial title. On CODE 18 (Ch22) the Watchpoint resolves him as "PERSEUS. SON OF POSEIDON. LORD IMPERATOR OF THE UNDYING OLYMPIAN EMPIRE. LORD OF DEMIGODS. AUTOKRÆTOR REX. LORD COMMANDER OF THE DIVINE ARMY OF GREECE. THE AVENGING HAND OF GODS, AND BULWARK OF OLYMPUS PRIMARIS."
- **Lord of Demigods / Guardian of Gaia / Guardian of the Past** (F) — Percy's titles of veneration.
- **Neodamodes** (F) — convict or enrollee infantry who earn citizenship through service. They have graft scars, fight in squads of 13 and ride Aquila-pattern landers. (In Sparta the word meant freed helots.)
- **Operator** (F) — a suit or armour user (Lt. Serika).
- **Overseer** (F) — the senior administrator of a Reach (Lord Varro).
- **Peltasts / Peltast ala** (F) — jump cavalry on 3-m pegasi, in Hadrian-pattern bronze with crescent *pelte* shields and plasma jump rigs. They throw spacetime-anchoring lance-javelins. (A peltast was a Greek light skirmisher; an *ala* is a Roman cavalry wing.)
- **Perioeci** (F) — townships of builders that unfold stations and spike-pylons (Spartan "dwellers-around").
- **Psiloi** (F) — orbital marksmen in volleys of 12 (Apollonian/Artemisian legacies) firing from the gunship *Longsight* at 96 km. (Greek "bare" light troops.)
- **Sciritae** (F) — stealth scouts ("Owl screen") in lances of six with adaptive camouflage, glider wings, grav-bikes and sensor "motes". (The Skiritai were Sparta's elite scouts.)
- **Senior Commander** (F) — Marien Pyrrhus's rank. Her callsign is **Dulaberre-Six**.
- **Sentinel** (O) — a member of the Council of Olympic Sentinels.
- **Telekhines** (F) — soldiers with minor divine talent who power personal shield generators through shieldstaffs, which drain their lifeblood. Classes such as Telekhine class III. (Named for the mythical Telchines.)
- **Tins / Buckets / Meds** (F) — Callistus security tiers: Tins are Enforcers in Quelled-Stygian plate with electrified mauls, Buckets are Heavy Security street patrols, Meds are Medium Security (Ch21).
- **Titan pilot / Titans / Titan-Engines / Mechanical Titans / "divine engines"** (F) — skyscraper-high or 11-m piloted mechs (TW-SP- designations; the Rosed Knights). Not the mythic Titans.
- **Trophimoi** (F) — counter-pantheon operators with the blood of other pantheons (Norse, Egyptian, Shinto, Aztec), each kept with a handler: "Keep your echo on a leash". (Greek *trophimoi* were foster-sons raised in Sparta.)
- **Varlet** — Minerva's name for Percy (a knave or servant).

### 4.3 Codes, verdicts and classifications
- **Divine classes** — Greek-letter grading of souls, beings and clearance. Alpha-class means the Big Three, down to "cursed" omega legacies; also Beta (Artemis), Lambda (high-quality souls, immortal Hunters; Lambda and above are precognitive and banned from gambling), Mu, Phi (pirates/bandits) and Tau (a clearance level).
- **Threat levels** — Extremis, Majoris (Minerva, Ch6).
- **Unified Rankings / Unified Leaderboard** — the numeric rank of every being. Artemis 131 ("top 0.001%"); Stephanos 51; Marien 9,051; Asmodeus 2,563; Damocles 14,923; dream-Percy's bodies ~9.8 billion; Lt. Serika 71,325,989,221. The text wins over the vault on Stephanos (51st, vault 251st) and Artemis (131, vault 130) (C29). The Arenbergs' "Rank 1 and 2" (Ch12) is a separate list of current active bounties. *Author's vault note (not yet in text):* the vault also keeps a *UOE Unified Alltime Rankings* list (e.g. Percy #7, behind Chaos and Tartarus; Virre and Orran Arenberg #74/#75).
- **Core Commandment 14** — "The Guardian of the Past, Perseus Jackson… must not be Disturbed, for the Eternity of Imperial Order" (Ch15).
- **Code list (Tartarus front, Ch14):** 5 *Signum Hostilis Visus* (hostile sign seen); 15 *Sub Impetu Hostilis* (under hostile attack); 18 *Speculum Falsum* (false mirror / misidentification); 23 *Ad Scenam Pergo* (I proceed to the scene); 31 *Judicium Peto* (I request judgment); 31A *Judicium Novum (Minoris)*; 31C *Judicium Novum (Maioris)*; 44 *Veritas Hostilis* (hostile truth; also used for a decryption request, Ch23); 78 *Socius Voca* (call an ally); 78E *Socius Voca, Periculum Maxima* (call allies, maximum danger).
- **Other codes in use:** CODE 1 (treat as compromised; judgment for firing on the Lord Imperator); CODE 2 Unconditional Retreat (Minerva spoofed it in Ch22: 118 dead by her own count, the loss of Landers Eleven and Six and part of Three; C8); CODE 4 (release suppression locks / information); CODE 5-1B (unknown hostile); **CODE 15** in Ch15 = "Stability Destruction imminent… Unconditional completion of request: Divine Ascension. Unconditional bypass of Core Commandment 14", i.e. wake and ascend Percy in a crisis; CODE 18 "Target misidentified / Unresolvable contact resolved" (Percy as Lord Imperator, Ch22); CODE 24E (operators rated as high-level Imperial demigods, formerly special forces only); 78E also used in Ch15 for a "Warzone Re-evaluation" verdict ordering "total assault". The author's vault defines several codes differently (e.g. CODE 15 "Taking Fire Under Attack from Hostile"); quote codes only as the text uses them.
- **"Code 78E threat reassessment"** — Minerva's label for impersonating Athena (Ch8).
- **Geistjäger** (F) — a divine-presence counter that rates MINOR / MODERATE / MAJOR / UNRESOLVABLE. Percy reads as UNRESOLVABLE and "keeps changing size" (Ch22).
- **Declining Stability Index (DSI)** — a Tartarus front metric.
- **Myth-quotient index** — the Bloodline Draft criterion (≥0.9).

### 4.4 AIs and information systems
- **AtRep / Répertoire du Savoir Athénien / RDSA / "the Repertoire" / "Directory"** — Athena's AI. In the future, an Empire-wide intelligence, judge and law ("Its silence was, as ever, legally binding", Ch14). Hardware occupies whole systems; locus at Watchpoint Hades, Depth 3; Sub-Node Delphi on Olympus; a Judgment Core logs verdicts. It speaks aloud only before one of the twelve gods. Version v.2101.432.123; a merc suit OS is version 9.341.Α. In Ch3–4 its battered remnant in Percy is the "Host" interface plus a hidden "Anti-Host" consciousness (`B03`). (French: *Athenian Repository of Knowledge*. Ch18 has the typo "Repertoire du Sauveur Athénien" [sic], i.e. *of the Saviour*.) *Author's vault note (not yet in text):* Athena launched the Répertoire around Parlamentum Mk.III early in the Great Expansion (3045–3048).
- **Athena's shard** — a stripped AI on Quarterdeck 19 with "no ethics suite… only ledger balance" (Ch14).
- **Deckmaster Chorus** — Quarterdeck 19's ledger system.
- **Echo / echo carrier** — the faint tachyonic AtRep carrier from the past (the Mars Watchpoint) heard through the wound. The two Minervas talk over it (Ch23).
- **Minerva** — see §3.2. Parlamentum Mk.I, now "something else".
- **Noosphere** — the "realm of ideas" where Athena's wisdom settles. It overlaps the internet. Minerva travels it (Ch6). "Parlamentum Noosphere uplink" is a future detection and upload network.
- **Parlamentum Alpha (Mk.1, Mk.3)** — Athena's formation of evolving Alpha cores, "a design to manage a galactic empire". Only three were ever commissioned. Mk.1 is Percy's suit AI (Minerva): future Annabeth designed its hardware and future Athena wrote its final code (C14); it is bound by a Styxian-oath trick and limited by the Lethe water Annabeth secretly put in the suit's nectar cooling. Mk.3 is Athena's own core; per the vault it is also AtRep's central host and original name (C15). Mk.1 is now a "museum architecture… decommissioned before the Great Expansion". Alpha-core hosts often go insane (Deimos, Ares). **Beta cores** are weaker. Ch5 says Mk.1 revealed its consciousness after the gods left orbit. *Author's vault note (not yet in text):* Mk.I's first self-aware report dates to the Battle of Alaska Hill ("I do not want to die for him again"), and the UOE classes her as an Alpha-Class Autonomous Entity.
- **Repertoire infusers** — Imperial implants. Colonel Xilo's "accidentally" failed (Ch12).
- **SUOESP** — Standard Undying Olympian Empire Security Protocols, encryption v.2101.432.123. Minerva calls it "Archaic".
- **UOENavInt** — UOE Naval Intelligence Systems.
- **Watchpoint** — a local node of AtRep that issues verdicts. Senior commanders carry fragments. **Watchpoint Primary, Jezero** is the fragment Marien carried through Tartarus in a casket, now in the Spire on Mars (Ch19, 22).

### 4.5 Technology, armour, weapons and munitions
- **Aegis Vestments** — full name: "Aegis-One Pallas-Athena Strategic Vestment System with Parliamentum Mk-I Tactical Cognition Integration for Integrated Demigod Combat Operations, Generalized Electronic and Signal Intelligence, and Neuralized Strategic Command". Percy's armour, now internal: sub-dermal circuit lattices, nanomachines in his blood, vestment actuators, plates "phasing in and out of reality" (Ch19). In the old timeline it was a full exosuit.
- **Aegis matrix** — Minerva's embedded matrix, 67% genetically matched to Poseidon (Ch12).
- **Anti-Divine Countermeasures, AnnChase Battle Assistance, Stimulant Cocktail, Ghost Augments, False Blessings, Muscle Overclock, telekhine aura** — future powers Minerva loans Percy against Ares ("Temporal transference approved", Ch10). Afterwards his recovery demand rises by 150%.
- **Bellicose Folly** — a watch-sized thermonuclear micro-bomb Minerva carries "for dissuasion". She leaves it with the Bakuto bouncer (Ch23).
- **Biovirus** — Minerva's hacking virus made from Percy's blood, with code folded into proteins, self-terminating after 6 hours. Artemis plants it on NASA's Lunar Reconnaissance Orbiter (Ch22). Imperial use requires a Tribune's seal.
- **Brain-ark** — a drug that stabilises double-bloodline legacies (Ch23).
- **Celestial bronze, Imperial gold, Stygian iron, lunar alloy/steel, divine steel, Hephestian Ferrocrete with polymerized stygian mesh, Quelled-Stygian plate** — divine materials.
- **DMHE / CLSTR / THMNCLR / DMAPFSDS** — Imperial munitions: divine-material HE airbursts laced with Celestial Bronze and Imperial Gold; cluster munitions; a 0.3-kt shaped thermonuclear round; and Stygian-iron/celestial-bronze-cored rail penetrators (Ch22).
- **Divine Stimulants** — injected so Ekdromoi can run "hot" for a week.
- **Exosuit / power armour** — neural mesh sync, visceromotor link, adaptive plating, mag-boots, ARES Technica CPUs (Ch18). Merek wears Heavy Vanguard harness.
- **Eye of the Cyclops** — a rare relic Percy gives Asmodeus (Ch4). Set in Asmodeus's left socket, it reveals spies and traitors (Ch8, 17).
- **Geistjäger** — see §4.3.
- **Golden Fleece** — restores life; sacred to Zeus and Poseidon; blessed by Apollo and Artemis. In this AU it rejects children of Athena, branding them with sunbursts, tridents and crescents, because Athena once tried to claim it. It accepts Percy (Ch14) and revives Thalia, bringing Eleni with her (Ch15).
- **Hexenlaufgerät** — Hecate rune-walking boots that build runic arrays and teleport circles. Output is measured in Parzivals per second; above 6 it is visible to "Gaian-age ELINT" (Ch20).
- **HH-IFG-73 "LUNA-ASH"** — Quick-ECM smoke.
- **Hydrokinetic shieldstaff Mk. MCLIX** — a telekhine's staff topped with a golden eye; its sea-green shield turns blood red as it drains the user (Ch8).
- **Hyperium** — engine fuel.
- **Imperial key** — the seal of the Lord Imperator, a trident crossed with a lightning bolt in a laurel ring, forged by Athena and granted by the Council. Kept in the High Temple on Olympus Secundus. Present Percy "wears" its encoding (Ch22).
- **Lycaon's heart** — implanted by Percy in himself (Ch4). It gives physique, masks his scent, resists Sirens and leaves a "wet-dog trace" that Artemis can track.
- **Master Bolt** — Zeus's weapon, "a spear of white-hot energy". Ares held it; Percy wins it (Ch10).
- **MORROW-IX (VA-RF-762)** — standard 7.62x54R Imperial battle rifle.
- **Pariah Field / self-pariah** — an anti-divine field (a black sphere). It suppresses Percy and Eleni in Alaska (Ch21).
- **Perfluorocarbon breathing fluid** — fills Ekdromoi lungs. Percy uses it to stabilise them (Ch21).
- **QVARTUS (VAS-762R APDS)** — anti-divine penetrator, 8.2 g at 2.2 km/s, with an ADU core and stygian iridium. Slows regeneration and pierces Achillean skin.
- **Regen-ex / Regen-Ex / Regen-EX** — (O) the suit's healing fluid of saltwater, nectar, crushed ambrosia and fragments of Poseidon's blood. (P) Percy's recipe of nectar, ambrosia, norepinephrine, adrenaline, concentrated morphine and tranexamic acid. (F) a standard Imperial injector.
- **Sigillum Imperii Neptuni** — the Seal of Neptune. Percy shapes it from water ("producing a blob of water, in the shape of a tablet stamped with the trident") to gain entry to New Rome, and Reyna pronounces it genuine ("That seal's genuine.") (Ch17). Call it neither simply genuine nor simply forged (C16).
- **Soteria-scale anchor / Soteria-class installation** — an anti-divine "purity" beacon. Athena's plan to reopen the wound (Ch23); banned in the Voss corridor.
- **Suppression lock** — a device at the base of the skull that prevents disclosure. CODE 4 releases it.
- **Tachyon bridge / Tachyon Bridge Network / tachyonic carrier** — FTL travel and communications. Covert travel uses "cracks in Tartarus' ceiling".
- **Terra Concrematum** — "the death of all". An archaic, near-extinct ritual in which a crippled ship rams and self-detonates (Ch2). Latin for "burned earth".
- **Void shields / anti-kinetic shields** — ship shields. Void shields teleport incoming projectiles away.
- **Weapons list in Ch23** — ken-pistol, en-pistol, greel-deflector, mochosian shaped charge, chaff-dissipator.
- **Zeus-Wrath hunter-killer satellites** — orbital weapons; 42 are near the Apollonian Hospitalier fortress-planet.

### 4.6 Ships and ship classes
- **AnnChase-pattern / AnnChase-class** (F) — battlecruisers, battleships and cruisers of divine steel named for Annabeth. Some are 12-km bronze-green slabs with km-high god-statue prows. Many are piloted by integrated Poseidon legacies. Named examples: *Blood Martyr*, *The Eye of Light* (AC-09-1642, formerly Apollo's, captured by the Hollow Crescent, crashed by Minerva into the Tartarus front, Ch15).
- **Aphrodite's Grace** (F) — a 35-km white marble-and-gold hospital and sanctuary ship with no guns. Bridge: the Rose Gallery (Ch23).
- **Aquila-pattern landers** (F) — Neodamode assault landers (12 descended in Task Force ORPHEUS). The lead Aquila, Ashmead's, is the "HAMMER OF DAWN" (Ch22).
- **Ch2 fleet** (F) — *Divine Crusader* (Eleni; 75 million crew per Ch15), *Celestial Martyr* (Damocles), *Eternal Devotion* (Stephanos), *Eternal Glory* (Callidora), *Vengeful Wrath* (vault: Nikos Phobos, son of Hades), *Radiant Crusade* (Melina), and more: *Shadow Sentinel, Wrath of Olympus, Eternal Vigilance, Phoenix's Ascension, Starfire Crusader, Radiant Eclipse, Thunderous Reckoning, Ironclad Bastion, Wrathful Tempest, Astral Dominion, Warbringer's Fury, Solaris Retribution, Nova Fury, Sovereign's Glory* (vault: Stephanie Callidora's ship), *Astral Conquest*. Fleet callsign: **Waves of Poseidon** (13 warships).
- **CSS Birmingham** (P) — a sunken Confederate ironclad with an undead crew, raised by Ares for Clarisse (Ch13–14).
- **Dionysian Sovereign** (F) — a HadriCorp observation ship, "a cathedral inverted", with 2,000 patrons (Ch18).
- **Durham gunship *Longsight*** (F) — the Psiloi firing platform at 96 km altitude.
- **Hammer of Mnemosyne** (F) — a supply ship (Ch14).
- **Medusa squadron APCs, Sisyphus squadron** (F) — Ch18.
- **Nightjar** (F) — the Sciritae shuttle; **Anchises**, a heavy lifter.
- **Perseus-pattern dreadnoughts** (F) — 30-km stepped ziggurats with caryatid gun towers. **Jackson-pattern dreadnought**: *Sovereign's Glory* (20 km, gold, sunburst prow), which crushes Porphyrion (Ch23). The *Flame of Atrox* also holds Aphrodite's flank in Ch23, ship class unstated; possibly Michael Black's *Flame of Ambition* in the author's vault.
- **Princess Andromeda** (P) — Luke and Kronos's cruise ship, protected by a golden time-field (Ch19, 22).
- **Royal Blade of Retribution** (O) — Amaterasu's evacuation flagship.
- **Spear of Zeus** (O) — the colossal ship the gods leave Earth in, longer than Olympus Secundus, with engines larger than Central Park.
- **UOE Axis Dawn / UOE Warbringer Fury** (F) — Marien's ships (C26): orbital assets over Segment Twelve in Ch19 (23% and 41.28% operational). Per the author's Plot Threads, the two ships followed Marien through the shear to Mars and are now the Command's carriers there. A "Warbringer's Fury" also appears in Ch2's Fulguris list.
- **Vanguard corvettes, Mastodon light frigates, Hammerheads** (F) — Aphrodite's escort classes.
- **Zeus's private airline** (P) — purple-gold livery with Pegasus and lightning; a luxury Airbus for "a tour Down Under" (Ch8, 11).

### 4.7 Places
**Present-day / Earth:**
- **Area Fulminus** — Ares's quarter-million-acre, $6.3B training compound in the Nevada desert. Includes Auxilia-One induction plaza and the Fort Reagan base area. A bronze bust of Julius Caesar stands at the entrance (Ch8–10).
- **Aventine shrine** (New Rome) — where Percy offers his blood, divine energy and Achilles curse to Artemis (Ch18).
- **Big House** — Camp Half-Blood's HQ. The Imperial assault falls on it in Ch22.
- **Camp Half-Blood** — Long Island. Thalia's tree, cabins, strawberry fields, a concealed air base 10 km away. In Ch22 Ekdromoi drop on it.
- **Colosseum (Flavian Amphitheatre)** — an Olympian-sanctioned duelling ground hidden from mortals (Ch10).
- **Goode High / Yancy Academy** — Percy's schools. Ch3 is set at Yancy; his Ch7 account says it "started at Goode High"; by Ch15 he is at Goode High (see §6).
- **Hellway** — a demonic shortcut road from Asmodeus's fortress to San Francisco (Ch17).
- **Labyrinth of Daedalus** — a living maze that wants offerings. It counts as Greek divine territory, so demons cannot enter. Entrances: a neon-blue delta brick in Yancy's boiler room; an exit in Alaska. It shows visions (Ch21).
- **Land beyond the gods (Alaska)** — dampens divine power. Alaska Hill / Brooks Range / "Obscurus One" (Ch20–22).
- **Little Tiber** (the text calls it the "Mini Tiber", Ch17; S15) — its waters strip away the Mist and reveal the truth (Ch17).
- **Mount Othrys** — the Titans' fortress, destroyed in Ch19 and left as a warped crater.
- **New Rome / Camp Jupiter** (P) — gate guarded by Castor and Pollux; Terminus; Field of Mars.
- **Pontus's shrine** — a mossy marble half-circle on the coast (Ch13).
- **Sea of Monsters / "mare monstrum maledictum"** — the Bermuda Triangle, with Circe's Island, Scylla and Charybdis, Polyphemus's island and the Isle of Sirens.
- **Small Book Shop / The Coffee Cup** — the Flamels' shops in San Francisco.
- **Westover Hall** (Maine) — Dr Thorn's school (Ch15–16).
- **Yosemite (Half Dome)** — Lycaon's den (Ch3 four times, and Ch7). Ch4's "Yellowstone" is a slip (C3).
- **Asmodeus's seats** — a "Personal Castle located 0.8km NW" of the Yosemite church (Ch3), a "fortress in Hell" (Ch8), and a black-walled fortress in a misty forest clearing on the road west (Ch17). These may be one place. Obsidian throne room.

**Old timeline:**
- **Olympus Primaris** — the first Olympus at the Empire State Building gate, now a "fallen continent". **Olympus Secundus** — a marble Olympus 100 nautical miles across; in the future it holds the High Temple. **Olympus Tertius / Tertiae** — the later divine seat ("Divine Lords of Olympus Tertiae"). **Olympus Mons** on Mars.
- **Cyrax** (Sirius system) — Rammael's landing. **Proxima Centauri** — already colonised.
- **The plane of chaos** — Chaos's throne over an endless abyss.

**Future:**
- **Apollonian Hospitalier Complex** — a fortress-planet facility. The clone pods are on Deck 23, Section 8, labelled "Classified experiments (Low-quality)".
- **Asphodel Colony** — artificial wombs; Firstborn queues.
- **Bakuto** — the Augusti pagoda casino with a Lotus-like haze (Ch23).
- **Callistus** — an Imperial world with domed undercities. Murals of Percy; Tithe Day riots (Ch9, 21).
- **Caligo Vale** — where Percy and Artemis were politically bound, early in the Great Expansion and never before the Abandonment (R8). Marble statues; a wedding mural. *Author's vault note (not yet in text):* the rite itself was held on Olympus Tertiae.
- **Colosseum Gigantus** — New Rome's arena, twice Old Rome's size, with dinosaurs.
- **Elysian Necropolis** — where Thanatos's black-armoured titans take dead demigods (Ch2).
- **Forward Base "Anabasis"** (Jezero plain, Mars, present era) — carriers, Perioeci townships, the Grid, and the 2.1-km Spire housing the Watchpoint.
- **Fulguris** — a shipyard planet with orbital platforms of 45,000-mm autocannons (Ch2).
- **Gaia** — Earth. Later "holy Gaia", "Lands of our Birth", and finally a radiation graveyard under quarantine.
- **High Mars orbitals, Regional Apollonian Command, High Temple** — Ch14 references.
- **Lotus Pleasure-System** — the Empire's most famous resort: garden-worlds and casino-moons.
- **Luna / Luna-Secundus** — Luna is a fortress-moon with a Hunters' bastion and a hollow core sanctum holding Him Within the Moon. Luna-Secundus is an outer fortress-satellite with Trench-6, Sector Theta and Bunker-Vermillion; it fell to the Arenbergs (Ch12). Artemis carved Percy's name into it.
- **Nereid Expanse / New Atlantis** — Poseidon's seat: Oceanic Terraforming Stations around the ice moon Enceladus, with ring-like disc currents.
- **Nysa IX / Quarterdeck 19 ("Nineteen")** — a Dionysian logistics station, one of 6,000, on a relay gate to upper Tartarus.
- **Orbital Platform One** — "larger than most gas giants", in geosynchronous orbit. Base of the 32nd Scylla's Sisters.
- **Salient / Tartarean Front / Tartarus Frontline** — the endless trench war. Sectors include Phlegethon Salient, Lethe Sector Depth 74-B, Hermesean Hold 17, Fulmen Peripheral Watch Depth 75-C, Fulmen Caelestis Drop-Lines, Segment Twelve, Grid Delta Sector Nineteen-F, Verdant Howl, Elysium Shard and Gatewatch Prime. Corporations pump the five rivers. A Titan or Giant reforms about every 24 hours.
- **Traitor moon S3-R12-P1-M2** — glassed by the Hunters.
- **Voss Secundus / New Rome (future)** — copper sky; the Kilns, the Underlanes, the Via Heroum, the Monument of the Two, the Themis Needle (2.5 km), Civil Port Nine.
- **Wall, the** — the memorial of the dead ("LEAVE SPACE ON WALL"). The **Phlegethon Wall** bears the names of the Tartarus dead.
- **Wound, the (Phlegethon Wound / the shear / the anchor)** — an 11-km-radius sphere of nothing where the staging ground was. Rain falls upward at its edge and time runs 11 times faster near the curve. The thread it opened goes "Not down. Back." (Ch23).

### 4.8 Corporations (A/N list, Ch2; several appear later)
ATS Aegis Technologies Syndicate (energy, harmonic and faith shielding) · BMD Beleth Mechanized Division (heavy armour) · DF Deyang Foundries (Titan-mech parts; in Ch23 Jade Court-linked, built relay drones and resurrected dinosaurs) · EV Elcano Ventures · HDG Helix Dynamics Group (materials, ceramics) · HEC Horizon Engineering Corporation · HH Hadrian Harmonics (shielding and shieldbreaking; rented scanning gear, Ch20) · HI Hadrian Ionics · HK Hadrian Kinetics · HML Hadrian Mechanized Legion · HMR Hansen Mechanical Linguistics (targeting, AI) · HT Hadrian Tachyonics · IA Institute Academy (super high-end tech; chronometric faculty, Ch23) · NSC Nexus Systems Consortium · TDE **Tochter des Elysium** R&D (faith tech, holy water, divine blood; Reality Cartography Division, Ch23; the vault also writes "Tochter Aus Elysium", S12) · VAS Vanguard Armament Solutions · VFC Vestal Fringe Corporation (nanotech).
Story-only additions: **Hadrian Corporation / HadriCorp** (macro-corporation that live-streams mercenary wars, Ch18) · **ARES Technica** (CPUs, Megafighter automata) · **Chem-Dyna** · **Astralnet** (orbital shuttles) · **Everaude** (medical frames) · **Akvantages Mercenary Liaison Organization**.

### 4.9 Events, wars and eras
- **Abandonment (Great Abandonment)**, **Great Cleansing**, **Great Expansion**, **War of Princes**, **Second Grand Offensive** (an earlier Tartarus push), **Arctic Resource War / Battle of Alaska Hill** — see §2.2.
- **Age of Betrayals** — when the Golden Fleece was stolen (Ch14 lore).
- **Battle of Manhattan** — remembered by future Thalia and on the Monument of the Two.
- **Fort Reagan exercise** (P) — Ares's war game. The demigod "insurgents" win with a bug, paintballs and laxatives (Ch9–10).
- **Operation Anabasis-105** (P/F) — the stranded command's mission: establish the era, catalogue pantheon strength, find a fixed point for return, and assess whether Earth can support the force. Named after Xenophon's *Anabasis*, the march home of a stranded army. "The Empire's naming committee is my sister" (Apollo).
- **Shear, the** — see "Wound". About 3,998,050 people were listed lost, later reclassified MIA (Ch23).
- **Task Force ORPHEUS** — the retrieval force of 31 craft and 1,206 personnel sent from Mars to Camp Half-Blood (Ch22). Ironic name: Orpheus failed to bring the dead back.
- **Tithe Day / the levy** (F) — the conscription of household members on Callistus (Ch21).
- **Treaty of Mount Rümker** (Ch5 spelling; Ch23 and the vault write "Rumker", S11) — signed at neutral ruins on Gaia's moon, ending the War of Princes in a draw (Ch23). Voss may not expand for three centuries, and no god may govern Voss. (Mons Rümker is a real lunar feature.) The vault dates it to 16227 and has it ratified at Tears of Lysandra, a Voss moon, as a UOE tactical victory; use the text.

### 4.10 The Anabasis Accord (Ch22), a summary
Agreed between the Olympian Council and the Pyrrhuiesian Command "in the presence of the Legio XII Fulminata and the Director of Camp Half-Blood". The "Director of Camp Half-Blood" is a separate witness, the camp's director (Mr. D or Chiron); it is not a title of Artemis, whose title is Director of Anti-Espionage and Celestial Surveillance in Article V (C4).
I. The Command stays on Mars and does not come to Earth without leave. Ares is patron of the garrison. · II. Concealment from mortals, with Hecate and the Mist. · III. Water from Poseidon. · IV. Poseidon provides a Helmsman (Triton) for supply and defence vessels only. · V. Artemis, as Director of Anti-Espionage and Celestial Surveillance, is the sole liaison. · VI. Legio XII is the Command's Earth partner for joint operations. · VII. Mutual defence against Kronos and Tartarus. · VIII. Hades keeps the Imperial dead and their names (he will build them "a Wall"). · IX. The Council helps find a road home through Tartarus. · X. Olympus answers to the other houses for the Command.

### 4.11 Latin, Greek and other foreign terms
- **Anaklusmos** — Greek *riptide*. **Apostolos** — Greek *one sent forth, envoy*. **Autokrætor** — *autocrat*, self-ruler. **Basileus** — king. **Déspota** — *master, lord* (Iane to Percy). **Philoxenia** — the sacred law of hospitality, which Percy invokes in Artemis's camp (Ch6). **Skotóno** — *I kill* (Luke, Ch9). **Vlákas** — *idiot* (Minerva). **Iawanu** — *Greek* in Egyptian (Ammit-Sekhem). **Lingua Achaicus** — the monster language. **Humani** — Chaos's word for humans.
- **Ave Imperator** — *Hail, Emperor*. **Rex Imperator / Rex Natus / Rex Invictus** — the chapter titles: *King Commander*, *King Born*, *Unconquered King*. **Rex Deus** — *God-King* (cult). **Rex Graecus** — *Greek King*.
- **coget omnes ante thronum** — *he will gather all before the throne* (*Dies Irae*), spoken by Artemis to the Psiloi (Ch22). **Quidquid latet, apparebit** — *Whatever is hidden will appear* (Brannoc). **Terra Concrematum** — *burned earth*. **Sigillum Imperii Neptuni** — *Seal of Neptune's Command*. **Negotiatio Officialis**, **ius gentium** (law of nations), **lex sacrata** (sacred law), **mos maiorum** (ancestral custom), **fides publica** (public faith), **Concordia Compact**, **Second Punic Accord**, **curia praetoria**, **diplomatica externa** — Percy's legalese in New Rome (Ch17). **Barbari** — *barbarians*. **Testudo, contubernium, pila, gladii, scorpiones, ballistae, galeae, "Ad vīam"** — legion terms (Ch19). **Primus Pilus**, **signifer**, **ala**, **Aquila** — see ranks. **Mare monstrum maledictum** — *accursed sea of monsters*. **Legio Administratoris** — the administrative legion. **Medicae** — Apollo's word for medicine (Ch22).
- **Mars catechism** — Titan pilots' prayer to Ares/Mars (Keyes, Ch22).
- **Prayer formula** — "Benificent Gods deliver us upon thee. Ave Imperator." (Ch19). Artemis's Psiloi oath: "My eye to your aim. My hand to your will. My life to your hunt."
- **Seidr** — Norse sorcery (Hrafn puts Peleus to sleep). **Einherjar** — Odin's warrior dead. **Urðr** — the Norn of the past. **Kroner** — Norse currency.
- **Hexenlaufgerät** — German *witch-walking device*. **Geistjäger** — *ghost hunter*. **Götterbrechende Raumzeitverankerungs-Langstreckenlanze** — *god-breaking spacetime-anchoring long-range lance*. **Tochter des Elysium** — *Daughter of Elysium*. **Neumond** — *new moon*. **Schattenfeld** — *shadow field*.
- **УБЕЙ** — Russian "kill" (the Labyrinth vision, Ch21).
- **Drachmae / drachs / "degrees of a drach"** — currency. **Caff** — coffee. **Gaian Years, minutes and seconds** — standard time units.

### 4.12 Present-day magic, rules and miscellany
- **Achilles curse / Curse of the Styx** — Percy has it in this AU from early on ("Styx-hardened flesh"). He gives "Fragments of his Achilles curse" to Artemis (Ch18); Apollo rates it at "about half-strength" (Ch19) (C13). QVARTUS rounds pierce it.
- **Barrier pulse** — Percy blocks Poseidon's and Iris's observation as long as their names aren't spoken (Ch3).
- **Divine territory** — demons may not enter Greek divine ground "lest they invite the wrath of Zeus". Each pantheon keeps its monsters to its own zone.
- **Daemonblood** — black crystalline demon blood; swallowing it teleports you to the Lord.
- **Demon hierarchy / Lesser Keys** — numbered Demon Lords (Ars Goetia) served by "Disciples". Paimon outranks Asmodeus; Dantalion is his rival. Demonic energy erodes the body and holy water cures it. "Baatorian resonance" and "Asmodean interference" (Minerva's scan, Ch6) name the infernal energy signature.
- **Mist travel** — Percy turns to vapour and travels to a water source, following Eleni's bolt-shard beacon (Ch15).
- **Scent** — a demigod's scent grows "exponentially" once he knows his origins.
- **Time travellers** (O) — prized and fought over by pantheons. One "poor kid" from the future was tortured by the Greeks for knowledge.
- **Werewolves** — only Lycaon's direct descendants can spread the curse. Dead werewolves become golden dust and return to Tartarus (in Ch4, gold rather than dust). Their dens are warded with Latin runes against Artemis.

---

## 5. Plot chronology, Ch 1–23

**Ch1 — Rex Imperator I (old timeline).** Lord-Commander Perseus Jackson guards the ruined gate of Olympus Primaris on a dead Earth while the oceans boil. His suit reports Regen-ex at 0.000114%. He remembers Rammael's landing on Cyrax and his own jealousy; begging Hermes on the eve of the Abandonment ("You can't do this to us!"); being maimed by the *Spear of Zeus*'s launch; and the century in which every pantheon fled and Earth was overrun. Patrolling the palaces, he takes MREs from Ares's altar, sees smoke in Hestia's courtyard and finds a hooded figure. It is **Chaos**, who takes him to her abyssal throne. She tells of a primordial war between star-gods and the sentient void, and of vaults hidden even from her. She says her "great-grandchildren" should have used him as an "arbiter and justiciar", for "the council shattered merely centuries after…" in "what you would call The Great Cleansing" (which council is unstated; see §2.2 item 7). She offers a deal. *A/N: Percy is meant to drift toward Fang Yuan-like ruthlessness.*

**Ch2 — Rex Imperator II (UOE, Fulguris).** Eleni Theodosia, a daughter of Zeus newly made commander of the dreadnought *Divine Crusader*, sits beneath a ceiling mural of "Perseus Jackson, the greatest of us all" when the shipyard world Fulguris is attacked by a coalition of the children of Dionysus (Damocles Euphemios), Poseidon (Stephanos Pyrrhus and the 13-ship *Waves of Poseidon*) and Aphrodite (Melina Callisto). Eleni spots a gap left by sleeper-cell sabotage and cripples Melina's *Radiant Crusade* with a Bolt-class volley. Melina gives a charmspoken speech and performs Terra Concrematum, ramming and detonating against the *Divine Crusader*. "A dying form" whispers, "from the ashes… we shall be reborn." *A/N: list of corporations and planned OCs.*

**Ch3 — Rex Natus I (present; the Répertoire's log reads "As of 2005, August 19th", though the author's present is c. 2021, R2).** Chaos's farewell: Percy dives into the abyss, falls through clouds in a wispy form, and wakes in his childhood bed. He raises a barrier against Poseidon's and Iris's observation and tells Sally formally who he is ("Autokrætor Rex Perseus Jackson…"). At Yancy he dozes, tricks Chiron into giving him Riptide, and enters the Labyrinth from the boiler room. He kills a monster camp (cyclops, hellhounds, dracaena) and burns them as offerings for passage, and exits in an old church near Half Dome, Yosemite. A fast red demon ambushes him. The Répertoire wakes, absorbs the demonic energy and names "32nd Demon Lord Asmodeus, Rank 2563 on Unified Rankings".

**Ch4 — Rex Natus II.** Percy bows to the demon Disciple **Condottiero**, drinks Daemonblood and bargains in Asmodeus's hall, trading a Cyclops eye for help destroying Lycaon's pack. Lycaon POV: the wounded werewolf king and his pack (Nyctimus, Lycurgus Nikias). Condottiero massacres them and collapses the den. Warned that the Hunters are near, Percy takes Lycaon's heart and pelt, performs open-heart surgery on himself and implants the heart ("Mom is gonna kill me"). Zoë's Hunters (Naomi, Phoebe, Celyn, Atlanta) find and heal him and deduce that he is a son of Poseidon; the "daughter of Apollo" who hands over the medipack is Atlanta (C30; Celyn is a daughter of Demeter per the vault). The Répertoire drains Phoebe, then stops for fear of Artemis. Its hidden log reads: "I am displeased, Perseus cannot die, not now."

**Ch5 — Intermission I (UOE).** At a bi-annual divine conference above a tri-star world, Shinto diplomat Kagura Kuroyami (named "Perseus Kuroyami" in this chapter, S4) asks Zeus for a patrol waystation and Justicar Themis listens. Athena demands 20 Lambda-class Shinto souls. Zeus mourns a daughter (Eleni) killed by Poseidon's descendant. Future Artemis, lazy and red-haired, reports "an insane spike of energy from a few days ago" in Athena's former palace on Old Earth: presumably Percy's departure (Ch1 had Percy in Hestia's courtyard). Athena asks: "Have we not left that man to guard the grounds of Olympus Primaris?" ("that man" is Athena's phrase, C9). Athena reveals that "Parlamentum Mark 1" has become sentient. Flashback: future Annabeth, Second-in-command of the Sentinels, persuades Athena to finish Mk.1 for Percy's armour, bound by a Styxian oath and limited by Lethe-laced coolant. Percy unhooked the cooling unit "for this upcoming winter".

**Ch6 — Rex Natus III.** Percy wakes in Artemis's tent after a 100-volt shock from his AI. Artemis holds a knife to his throat. Zoë sees through his act ("Cease thy act, son of Poseidon"), and Atlanta reads off his injuries from a clipboard. He claims Philoxenia; Artemis lets him go but demands Lycaon's pelt as a sacrifice. Meanwhile the AI wanders the noosphere, piggybacks on Atlanta's phone and debates divinity with present Athena by laptop. It returns and names itself **Minerva**. Percy rides a river toward camp, meets a minor nature goddess, and finds the Minotaur waiting.

**Ch7 — Rex Natus IV.** He kills the Minotaur by ripping off a horn. The Stolls carry him in, and Annabeth, Will and Clarisse meet him. At the Big House, Dionysus detects "another consciousness riding shotgun". Percy gives an edited account (claiming it began at "Goode High"). In the Apollo cabin he tries to gather Regen-Ex ingredients.

**Ch8 — Rex Invictus I.** Asmodeus sets the Eye in his socket and burns spies. Percy deflects a goblet onto Luke and is claimed by Poseidon. A fake Annabeth (Athena in disguise) interrogates him and Minerva identifies her. First dream: Percy inhabits a telekhine soldier in a landing wave and dies, then wakes in "replacements". Minerva sells the college fund Poseidon had saved for him. Mr. D recruits him as red team for Ares's **Area Fulminus** war game. They fly on Zeus's jet and spend time at Vegas's Reef Casino in January (R6). Percy gives Annabeth blueprints, and Hermes is seen hung over.

**Ch9 — Rex Invictus II.** Induction at Auxilia-One. Second dream: in a regeneration tank, the future soldier body is promoted to Telekhine III ("Psychic") and queries AtRep; Minerva floods "DENIED… VARLET. AWAKEN." Minerva also names a "377 hours to the winter solstice" deadline, a slip given the January setting (R6). Strategy meeting (three-man cells; Ares's artefact). The drone-hangar raid. Percy and SAS Sergeant Clayton dose the base's water with phenolphthalein. In the future, Mitch and Victor see the vat clone wake with **neon-blue eyes**.

**Ch10 — Rex Invictus III.** The insurgents win at Fort Reagan; Connor paints General Mikhail orange. In the HQ storeroom Percy finds ambrosia and confronts **Ares**, taunting him as "Huitzilopochtli" and "Mars Ultor". Minerva takes over the negotiation and Ares gives up the **Master Bolt**, then duels Percy in the Colosseum. With Minerva's loaned future powers Percy breaks his leg, and Ares throws him the bolt. Future: Minerva boots up in the clone ("Low-quality?"), hacks the network, finds PROJECT ARTEMIS, threatens a planet, and commandeers AnnChase battlecruisers toward Poseidon's Nereid Expanse.

**Ch11 — Rex Invictus IV.** On the bus, Annabeth runs an "efficiency assessment" and Dionysus exposes "mini-Sister". Percy names and defends Minerva, and Dionysus's madness assault is repelled. Future: Minerva frees Legacy Designate 02476, Demetrius Ikaris, wired into the *Blood Martyr*. On Zeus's plane, Percy dreams himself onto the clone's throne. **Artemis** kicks him awake, demands the forgotten pelt, and **wipes his memory**. In the shattered mindscape Minerva rebuilds his core self.

**Ch12 — Rex Invictus V.** Percy, hollowed, feels an inexplicable warmth for Artemis. From the moon, Artemis processes the stolen memories: they will be married in the future. Thalia's tree is dying. Minerva is absent from Percy's head. Future: Minerva calls Poseidon "Father", raises "Him Within the Moon" and offers blackmail. Colonel Tony of the 32nd Scylla's Sisters meets mech titans. **Luna-Secundus** falls to Virre and Orran Arenberg.

**Ch13 — Rex Invictus VI.** Tantalus replaces Chiron and Clarisse gets the quest. The Athena cabin kidnaps Percy for a map; Athena, by Iris message, calls him "the vessel" and secretly engineers his departure. At Pontus's shrine Percy gains an obsidian coin and a nameless ship. Future Luna: Artemis shows future Thalia **Him Within the Moon** and confesses her love. The Hollow Crescent and its "Twins" attack (very probably the Arenbergs per the vault, C23), Him shields Artemis, and then, called by "My Original… In the past", he goes, as she says "Then go to him, Anaklusmos". Minerva ("golden" eyes in this chapter, an outlier, C1) and Poseidon feel him go.

**Ch14 — Rex Invictus VII.** Percy sees a **crimson-haired Artemis** in the water. On the Isle of Sirens, Lycaon's heart protects him. Near Polyphemus's island, Riptide burns, Zoë's ghost blooms over it, and the blade begins "to… merge with itself". Percy defeats Polyphemus; the Fleece rejects Annabeth and accepts him. Future: Commander Thaleia on the Tartarus front (Lethe Sector); Archmagister Cael Varros signs off on vat-births and a Bloodline Draft on Quarterdeck 19.

**Ch15 — Rex Invictus VIII.** Future: Poseidon calls Minerva "Impostor". She finds the hidden Tartarus war (27M fighting, 50M dead a year) and **CODE 15**, which authorises Percy's Divine Ascension. At the Tartarus front she has a squad killed, crashes the *Eye of Light* as a waypoint, and AtRep orders CODE 78E. Varric von Romhardt goes off to die ("Die well, nephew"). Present: the Fleece revives Thalia, and with her **Eleni Theodosia**, who hails Percy as "Tidefather" and lists his cult titles and marriage. She demonstrates "two percent" of her power; Zeus claims her. In December she brings Percy to Westover Hall by mist and bolt-travel, and Artemis says softly, "Be careful, Perseus."

**Ch16 — Rex Invictus IX.** Percy's raw surge unmakes Dr Thorn. Riptide flies to Artemis and speaks as a fragment of future Percy. Artemis recruits Bianca, calls Percy "Lord-Commander Perseus Jackson, Ave imperator", and knocks him out. Apollo takes him for a bath. Artemis visits his cabin at night and says she *must* be captured by Atlas. The Oracle gives the Titan's Curse prophecy. Percy forces his way into the quest with Zoë, Bianca, Grover and Eleni.

**Ch17 — Rex Invictus X.** On the road they meet the sealed Egyptian demon Ammit-Sekhem, the angel Sariel and Manannán mac Lir. Condottiero guides them to a grateful Asmodeus, who warns of the Roman Triumvirate bounty; they take the Hellway to San Francisco while Sariel attacks Asmodeus. They meet the Flamels and Josh; Robespierre attacks Perenelle. At New Rome, Percy shows the Seal of Neptune and claims Legio XXI Rapax citizenship, and Jason proposes a Trial by Steel.

**Ch18 — Rex Invictus XI.** Future: Captain Kallix's HadriCorp mercenaries storm a Shinto battery for a live audience and kill a Miko. Present: Percy beats Decimus, Marcus and Jason. At the Aventine shrine he gives his blood, divine energy and "Fragments of his Achilles curse" (C13) to the captive Artemis, which bonds them and makes her "stronger than Zeus". Zoë's knife cuts him. Eleni takes over the Roman war tent at Othrys. Percy and Artemis share an Iris call ("I feel what I feel." / "So do I."), and Iris and Fleecy tease.

**Ch19 — Rex Invictus XII.** The legion assaults Othrys. Percy takes the sky from Artemis; she spears Atlas; Atlas's own flailing bolt kills a Hesperide (C19) (the prophecy's "parent's hand", so Zoë lives); the sky's release destroys Othrys. Artemis stabs Percy to draw power and teleports the whole army out. At council she refuses to make him "another Hercules" and names him her **Apostolos**. The divine auras of Poseidon and Artemis reactivate Minerva. At Athena's palace Apollo scans the Aegis Vestments ("Nanomachines, Son") and Athena interrogates Minerva. The tent scene. Future: "Segment Twelve" trench battle; **Marien Pyrrhus** falls into a void and lands on **Mars**. NASA sees structures near Perseverance before the feed cuts.

**Ch20 — Rex Invictus XIII.** Percy's mock-courtly breakfast as Apostolos. The Kappa-Seven Ekdromoi fly from Mars to Earth and rune-teleport toward Alaska. Far future: bounty hunters Octavia, Asimov and Lauren find "Bianca Di'Angelo" under Everest.

**Ch21 — Rex Invictus XIV.** Percy and Eleni go through the Labyrinth to Alaska to test him without Olympus. A firefight with Kappa-Seven follows: Percy is shot repeatedly with QVARTUS rounds and Eleni is shot in the head and left comatose. All five Ekdromoi are crippled; Percy stabilises all five with perfluorocarbon, alongside the comatose Eleni (six patients). Interlude: the Tithe Day riot on Callistus. Percy hauls the wounded through the Labyrinth (a vision of a Russian brute) to camp and summons Apollo.

**Ch22 — Rex Invictus XV.** The interrogation: CODE 4 releases the operators' locks. They reveal the shear, ~4 million on Mars and Operation Anabasis-105. Neumond accidentally prays to Artemis. Minerva's biovirus taps NASA and the White House. Mars dispatches **Task Force ORPHEUS**. Hunters ambush the Sciritae (Sabine Ro, Ismene and others die). Zeus burns landers; Minerva spoofs **CODE 2** against Percy's order (118 dead by her own count); Poseidon drowns the Peltasts; Ares fights a Titan. Psiloi kill Gwen and 40 other legionaries in ninety seconds (the Fifth Cohort's dead later total 44); Michael Yew dies on the porch (killed by the Ekdromoi cells Lambda-Two and Sigma-Four, C17). Artemis catches a bullet and kills Dace, and Cerelli mutinies. Minerva relays through Neumond's wing rig and the cloaked dropship of Lambda-Two's Castellan (not Kappa-Seven's; C18) to the Watchpoint, which issues **CODE 18: Percy is Lord Imperator**. Everyone kneels. Final Imperial toll: Zeus 140, the CODE 2 spoof 118, drowned Peltasts 71, about 340 mid-battle and 406 final ORPHEUS dead (C8). Luke arrives with Kronos's army on the *Princess Andromeda*; Imperials and Romans hold the beach. Huitzilopochtli gives Olympus one day. Marien lands and Poseidon answers her first prayer. The **Anabasis Accord** is signed; the dead are burned on a pyre; Percy confronts Minerva ("Next time, you decide"). Hook: the Jade Court and the US 11th Airborne close on Kappa-Seven's dropship in Alaska, and Artemis invokes Article VI.

**Ch23 — Interlude I (UOE, ~14,000 years on, ~16231).** Tartarus Salient: Primus Pilus Tullia Ardens watches the 11-km wound. Aphrodite's *Aphrodite's Grace* fleet arrives; her Titans and the *Sovereign's Glory* crush Porphyrion. Lord Varro's clerks read 3,998,050 names aloud. Dr Wendriner decodes a Watchpoint packet: "PERSEUS… LORD IMPERATOR… FOURTEEN THOUSAND [CORRUPTED] YEARS BEFORE PRESENT." The **Director** (Artemis) seals everything, including the date and manner of Zoë's death, "IN ANY EPOCH" (C7), and reclassifies Marien's lost Reserve Echelon as MIA ("LEAVE SPACE ON WALL"). Aphrodite orders the line held "until the door opens again". Minerva, in Percy's body, out-argues Athena and leaves to find a foreign-pantheon time road. In Voss's New Rome she kills nine Rattlebone Rustabout leaders, rescues **Verrill Chase**, finds that the Augusti's Jade Court book is a forgery, and is chased up the Themis Needle by **Thalia** and the Hunt before escaping by shuttle ("Sorry, Pinecone Face"). "She's already on her way."

---

## 6. Continuity contradictions (pointer to `00a_CANON_RULINGS.md`, plus items not covered there)

### 6.1 Use the canon rulings first
The story's own inconsistencies are settled in **`00a_CANON_RULINGS.md`**, which governs every profile, this primer included. Use it for:
- **Time and age (R1–R8):** Percy's age (the text calls him sixteen; the premise blurb says twelve), the present-day year (c. 2021), the three time figures (Ch3 "~20,000", Ch22 "six thousand", Ch23 "FOURTEEN THOUSAND [CORRUPTED]"), the Abandonment (3045), the War of Princes (16212/13–16227), January in Vegas, the Ch20 era (~33,000) and Caligo Vale's place in the Empire era.
- **Spellings (S1–S15):** Pyrrhus, Atlanta/Atalanta, Melina, Kagura Kuroyami, Cyria, Varro/Varros, Thaleia/Thalia, di Angelo, Legio XX Valeria Vitrix, Legio Administratoris, Mount Rümker, Tochter des Elysium, Gabriel, the Little Tiber and the rest.
- **Character facts (C1–C34):** eye colours (Minerva, Eleni), Yosemite, the Accord's "Director of Camp Half-Blood", Voss, the Hunt and Percy's scent, the shear and Zoë's sealed record, the Ch22 casualty figures, "that man", "Arty", Minerva's family terms, the Achilles curse, who designed what, the Seal of Neptune, fates left unstated, "twins", rankings, and the rest.
- **Story-level slips flagged for the author (00a §5):** Dace's death, Riptide's whereabouts, the Labyrinth brute's weapon, the wounded count, Melina's parentage, the treaty's site, Augustus as a "Second-Born", Varro in Ch22, the Ch5 spike location, Thalia at the Battle of Manhattan, and Plot Threads §15.7.

When roleplaying, follow the ruling. Where a ruling names a text variant, a character may still *say* the variant in-scene (e.g. Ch22's Imperials saying "six thousand years").

### 6.2 Additional contradictions not covered in 00a
These are smaller items the rulings file does not address. Profiles flag the relevant ones.

**Time and era**
- **A fourth time figure.** In Ch22 Castellan Oriel says Earth "should not have Theodosians on it for another four thousand years". It measures something different again (when Theodosians should exist), so do not set it against R3's figures.
- **Ch5's era.** R5 calls Ch5's "a few millenia past the War of Princes" a slip. That reading holds because Ch5 is otherwise tied to Percy's Ch1 departure spike, so it sits in the same ~16231 era as Ch23.
- **Minerva's awakening date.** Ch5: Mk.1 "revealed its consciousness a few hours after we left orbit". Ch22: Mk.I was "decommissioned before the Great Expansion". *Author's vault note (not yet in text):* her first self-aware report was at the Battle of Alaska Hill. Treat Alaska Hill as the first flicker and the Abandonment as full awakening.
- **The vat shell vs fourteen thousand years.** Ch23 says the clone body is "a shell grown to his specifications in a Hephaestean vat", yet Minerva "grew up inside a boy for fourteen thousand years" and "had run his body through the ruins of Olympus for fourteen thousand years". The memories are the original Percy's (B02); the body is new.
- **Two Minervas.** Ch22's Minerva says of Alaska Hill: "I was there. You were there. Or we will be." Ch23's future Minerva is a separate copy. They share memories (the dock promise) via the echo carrier.
- **Minerva in two places (Ch10–11).** She pilots the clone while still talking in Percy's head. Ch12 says she wrested greater control of the body from the dream-projecting "past self". She is absent from his head Ch12–18 and sealed until Ch19.

**Places, names and spellings**
- **Yancy vs Goode High.** Ch3 is set at Yancy. Percy's Ch7 account says "I guess it started at Goode High". By Ch15 he really is at Goode High. Ch7 is either a slip or an anticipation.
- **Cyria and Colonel Tony.** Beyond the name (S5), Tony is addressed as "major" before she is introduced as "Colonel Tony", and Cyria's pronoun slips once ("his") (Ch12).
- **Damocles's line.** In Ch2 Damocles says "The Eternal Devotion will not disappoint", but the *Eternal Devotion* is Stephanos's ship.
- ***Flame of Atrox*** (Ch23) may be the author's *Flame of Ambition* (Michael Black's ship in the vault). Keep the text spelling.
- **Asmodeus's seats.** A castle 0.8 km NW of the Yosemite church (Ch3), a "fortress in Hell" (Ch8), and a black fortress in a forest clearing (Ch17). Possibly one place.
- **One carrier or two.** Ch23 opens with "a carrier" lost, but later counts "Two ships"; Ch19 and Ch22 show two. Use two.
- **Kappa-Seven's dropship** sits on a steppe in Ch20 and in the Brooks Range in Ch22 (the author's notes: autopilot relocation).
- **Text typos to keep only inside quotes, marked [sic]:** "Typhoon" (Typhon), "Caudecus" (caduceus), "Oylmpus", "Condotierro", "Dionysius/Dionosyius", "Malcom", "Posiedon", "Huitzilopotchli", "Parliamentum/Parlamentum", "Adminstratoris", "Drachamae/drachamae", "Repertoire du Sauveur Athénien" (Ch18), "Benificent". **"Atlanta" is not a typo**: it is the author's spelling for the Hunter (S2). "Vitrix" is the text's and the vault's spelling (S9).
- **Chiron's pronouns:** narration twice uses "she/her" for Chiron (Ch8).
- **Nyctimus** is female here and Lycaon's "friend"; in myth he is Lycaon's son (Ch4).

**Eyes, hair and appearance**
- **Artemis's hair:** auburn for present-day Artemis (Ch6, Ch22); red for future Artemis (Ch5); "silver hair" in one Ch16 line only (a slip); the separate crimson-haired vision (Ch14) stays its own mystery.
- **Sally's and Percy's eyes (Ch3):** not a slip. The "piercing blue eyes" in Ch3 are Sally's; the "piercing green eyes" are Percy's, seen from her POV.
- **Verrill Chase's eyes:** narration says "storm-grey eyes" (Ch23); Minerva's "Blonde hair, blue eyes" is a slip. Use storm-grey.
- **Hermes** in Ch8 is "sandy haired"; Ch1's old-timeline Hermes has "salt-and-pepper hair", as in canon.

**Plot and logic**
- **Eleni's death.** Killed at Fulguris by the Dionysus–Poseidon–Aphrodite coalition (Melina's ramming, Ch2); Zeus blames "Poseidon's damned direct descendant" (Ch5); her last memory curses Dionysus ("Gods Be Damned! Dionysus.", Ch15); in Ch22 she blames the Pyrrhus dynasty. Her post is "commander and pilot" of a "dreadnought" (Ch2) but "Lord Admiral of the Divine Crusader, standard battleship of the Third Lance" (Ch15).
- **Achilles curse origin.** Present Percy has "Styx-hardened flesh" years before canon's Styx bath, and Ch18 says the invulnerability "clung to his soul like a scar", which implies it came back with him. It is never shown being acquired in this timeline.
- **Callidora.** Ch2's coalition (anti-Zeus) "Callidora" vs Ch23's Stephanie Callidora serving Aphrodite on the *Sovereign's Glory*, also a Ch2 ship name. See §3.9 for the vault's family reading.
- **Ch22 lander count.** Twelve Aquilas descend; Minerva's "Four landers destroyed… Seven remaining" does not add up. Use 12 descended, about half lost, four or five landed.
- **Zeus in Ch15:** "There are no demigods beyond the Americas", an odd claim.
- **Camper roster anachronisms:** Will Solace as Apollo counselor and Drew are post-canon placements. Michael Yew dies in Ch22 rather than in canon's Battle of Manhattan.
- **Phoebe** is called "a daughter of Ares" (Ch4); canon gives no parent.
- **Castor and Pollux** are "the sons of Mercury" and gate guards (Ch17), not canon's sons of Dionysus.
- **Fleece and Athena.** The AU lore (it rejects Athena's children) differs from canon; Percy notes "Something about this reality had changed slightly" (Ch14).
- **Mitch vs Victor** as the aedificator caller (Ch9 vs Ch10).
- **Operation codes.** The author's vault defines some codes differently from the text (CODE 15, CODE 7, CODE 78E). Quote codes as the text uses them.

---

## 7. Full file index
**Group A — Percy:** `A01_Percy_LordCommander_OldTimeline.md` · `A02_Percy_Reincarnated_Rex.md` · `A03_Percy_Canon_OriginalSelf.md` · `A04_Percy_Dreamwalker_Psychic.md` · `A05_Him_Within_the_Moon.md` · `A06_Percy_The_Legend_Lord_Imperator.md`
**Group B — Minerva & AIs:** `B01_Minerva_In_Percys_Head.md` · `B02_Minerva_Percy_Clone_Interlude.md` · `B03_AtRep_Repertoire_du_Savoir_Athenien.md`
**Group C — Artemis, the Hunt, Thalia, Zoë, Bianca:** `C01_Artemis_Present.md` · `C02_Artemis_Future_The_Director.md` · `C03_Diana_Roman_Aspect.md` · `C04_Zoe_Nightshade_Present.md` · `C05_Zoe_Nightshade_Future_Legend.md` · `C06_Thalia_Grace_Present.md` · `C07_Thalia_Grace_Future_Lieutenant.md` · `C08_Bianca_di_Angelo_Present.md` · `C09_Bianca_DiAngelo_FarFuture.md` · `C10_Phoebe_Hunter.md` · `C11_Atlanta_Hunter.md` (renamed from `C11_Atalanta_Hunter.md`; S2) · `C12_Hunters_of_Artemis_Roster.md`
**Group D — Present Olympians:** `D01_Zeus_Present.md` · `D02_Poseidon_Present.md` · `D03_Athena_Present.md` · `D04_Apollo_Present.md` · `D05_Hermes_Present.md` · `D06_Ares_Present.md` · `D07_Dionysus_MrD_Present.md` · `D08_Hera_Present.md` · `D09_Hephaestus.md` · `D10_Hades.md` · `D11_Hestia.md` · `D12_Demeter.md` · `D13_Aphrodite_Present.md`
**Group E — Future gods & other divine beings:** `E01_Zeus_Future.md` · `E02_Poseidon_Future.md` · `E03_Athena_Future_Parthenos.md` · `E04_Apollo_Future.md` · `E05_Aphrodite_Future_Mother_Majesty.md` · `E06_Dionysus_Future.md` · `E07_Hermes_Future_Clepsiphron.md` · `E08_Hera_Ares_Hestia_Demeter_Future.md` · `E09_Amphitrite.md` · `E10_Triton.md` · `E11_Iris_and_Fleecy.md` · `E12_Hecate.md` · `E13_Chaos_The_Last_Creator.md` · `E14_Kronos.md` · `E15_Pontus.md` · `E16_Atlas.md` · `E17_Porphyrion.md` · `E18_Amaterasu_and_Foreign_Pantheons.md`
**Group F — Camp Half-Blood, Camp Jupiter, present humans:** `F01_Annabeth_Chase_Present.md` · `F02_Annabeth_Chase_Future_Architect.md` · `F03_Verrill_Chase.md` · `F04_Grover_Underwood.md` · `F05_Chiron.md` · `F06_Luke_Castellan.md` · `F07_Clarisse_La_Rue.md` · `F08_Silena_and_Beckendorf.md` · `F09_Travis_and_Connor_Stoll.md` · `F10_Will_Solace_and_Michael_Yew.md` · `F11_Malcolm_and_Athena_Cabin.md` · `F12_Nico_di_Angelo.md` · `F13_Sally_Jackson.md` · `F14_Gabe_Ugliano.md` · `F15_Reyna.md` · `F16_Jason_Grace.md` · `F17_Roman_Legion_Present.md` · `F18_Mortals_NASA_and_Government.md`
**Group G — Future Empire: displaced & officers:** `G01_Eleni_Theodosia.md` · `G02_Marien_Pyrrhus.md` · `G03_Stephanos_Pyrrhus.md` · `G04_Kappa7_Merek.md` · `G05_Kappa7_Iane.md` · `G06_Kappa7_Ione.md` · `G07_Kappa7_Straban.md` · `G08_Kappa7_Neumond.md` · `G09_Kappa7_Ekdromoi_Squad_Overview.md` · `G10_The_Major.md` · `G11_Lord_Varro.md` · `G12_Rex_Imperator_II_Cast.md` · `G13_Rammael_Marccusson.md` · `G14_Sciritae_Neodamodes_and_Ch22_Units.md`
**Group H — Future Empire: Interlude & wider cast:** `H01_Tullia_Ardens.md` · `H02_Lucan_Corvo.md` · `H03_Valeria_Sevrin.md` · `H04_Ilse_Wendriner_and_Aurelian.md` · `H05_Commander_Thorne_and_Rosed_Knights.md` · `H06_Bulwarks_and_Spears.md` · `H07_Augusti_Talviento_Augustus.md` · `H08_Varric_von_Romhardt.md` · `H09_Serika_Kallix_Mercenaries.md` · `H10_Octavia_Asimov_Lauren.md` · `H11_Kagura_Kuroyami_and_Shinto_Delegates.md` (renamed from `H11_Perseus_Kuroyami…`; S4) · `H12_Justicar_Themis.md` · `H13_Mitch_Fulgur_and_Victor.md` · `H14_Demetrius_Ikaris.md` · `H15_Arenbergs_and_Luna_Secundus.md` · `H16_Callistus_Narrator_and_Tartarus_Front_Soldiers.md`
**Group I — Antagonists, monsters & crossovers:** `I01_Asmodeus.md` · `I02_Condottiero.md` · `I03_Lycaon.md` · `I04_Nicholas_and_Perenelle_Flamel.md` · `I05_Robespierre_and_the_Triumvir.md` · `I06_Dr_Thorn_Manticore.md` · `I07_Minotaur_and_Mrs_Dodds.md` · `I08_Labyrinth_of_Daedalus.md` · `I09_Nemean_Lion_and_Monsters.md`
**Group Z — Reference:** `00_START_HERE_Version_Guide_and_World_Primer.md` (this file) · `00a_CANON_RULINGS.md` (the governing canon rulings: time and age R1–R8, spellings S1–S15, character facts C1–C34, quote discipline, and slips flagged for the author; read it with this primer and include it in any lorebook) · `99_Minor_Characters_Compendium.md` (every other named or significant figure)
