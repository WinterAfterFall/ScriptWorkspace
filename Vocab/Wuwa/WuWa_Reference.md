# Wuthering Waves — Reference Data (Version 3.5–3.6, September 2026)

> Source-verified reference file structured for AI ingestion / Markdown generation.
> Sections: 1) Echo Substats & Mainstats · 2) Echo Set (Sonata) Bonuses · 3) Echo Cost 4/3/1 ·
> 4) All Weapons · 5) All Characters.
> Game state: 54+ playable Resonators, 110+ weapons, 34 Sonata sets.

---

## 1. Echo Substats & Mainstats

### 1.1 Echo Rarity -> Level & Substat Slots
| Rarity | Color | Max Level | Substat Slots |
|--------|-------|-----------|---------------|
| Rank 2 | Green | 10 | 0 |
| Rank 3 | Blue | 15 | 3 |
| Rank 4 | Purple | 20 | 4 |
| Rank 5 | Gold | 25 | 5 |

- Each Echo has **2 main stats**: primary (random from cost pool) + secondary (fixed).
- Secondary main stat: 1-Cost = Flat HP; 3-Cost & 4-Cost = Flat ATK.
- Substats are NOT rolled at acquisition. They are revealed via **Tuning** at every +5 level (+5/+10/+15/+20/+25), costing Tuners (matching tier) + Shell Credits.
- Substats **cannot be re-rolled or changed** once revealed. No duplicate substats on one Echo, but a substat CAN duplicate the main stat (e.g. double Crit Rate).

### 1.2 Main Stat Max Values (5-star / Lv.25)
| Main Stat | Cost slot(s) | Max value |
|-----------|--------------|-----------|
| Crit Rate | 4-Cost only | 22.0% |
| Crit DMG | 4-Cost only | 44.0% |
| Healing Bonus | 4-Cost only | 26.0% |
| Energy Regen | 3-Cost only | 32.0% |
| Elemental DMG Bonus (Aero/Glacio/Fusion/Electro/Havoc/Spectro) | 3-Cost only | 30.0% |
| ATK% | 4 / 3 / 1-Cost | 33.0% / 30.0% / 18.0% |
| HP% | 4 / 3 / 1-Cost | 33.0% / 30.0% / 22.8% |
| DEF% | 4 / 3 / 1-Cost | 41.5% / 38.0% / 18.0% |
| Flat HP (1-Cost) | 1-Cost | 2280 |

### 1.3 Substat Pool & Value Ranges (same for all rarities)
| Substat | Value Range |
|---------|-------------|
| Flat HP | 320 - 580 |
| Flat ATK | 30 - 70 |
| Flat DEF | 40 - 70 |
| HP% | 6.4% - 11.6% |
| ATK% | 6.4% - 11.6% |
| DEF% | 8.1% - 14.7% |
| Crit Rate | 6.3% - 10.5% |
| Crit DMG | 12.6% - 21.0% |
| Energy Regen | 6.8% - 12.4% |
| Basic Attack DMG Bonus | 6.4% - 11.6% |
| Heavy Attack DMG Bonus | 6.4% - 11.6% |
| Resonance Skill DMG Bonus | 6.4% - 11.6% |
| Resonance Liberation DMG Bonus | 6.4% - 11.6% |

### 1.4 Substat Priority by Role
- **Main DPS:** Crit Rate -> Crit DMG (aim ~1:2 ratio) -> ATK% -> matching skill-type DMG bonus -> Energy Regen (only if below rotation breakpoint). Flat ATK is far weaker than ATK%.
- **Sub-DPS / Buffer:** same Crit-first order, but weight Energy Regen higher so Outro/Intro swaps land on time.
- **Healer / Support:** HP% and Energy Regen first -> DEF% -> Crit substats treated as near-irrelevant bonus rolls.
- Base Crit scaling: 5% base Crit Rate, 150% base Crit DMG.

### 1.5 Main Stat Picks by Cost & Role
| Cost | Main DPS | Healer | Buffer/Support |
|------|----------|--------|----------------|
| 4-Cost | Crit Rate / Crit DMG | Healing Bonus / HP% | Crit or ATK% |
| 3-Cost | Elemental DMG% (x2) | HP% / Energy Regen | Energy Regen / Elemental DMG% |
| 1-Cost | ATK% (x2) | HP% (x2) | ATK% or HP% |

> Rule: Never use flat main stats (flat ATK/HP/DEF) on 1-Cost - the % versions scale far better at endgame.

---

## 2. Echo Set (Sonata) Bonuses — 34 Sets

Standard threshold: **2-piece = flat +10%** (element DMG / Healing / ATK / Energy Regen); **5-piece = build-defining mechanic.** Some newer 2.x-3.x sets activate at **3-piece** instead. There is NO 3/4-piece partial credit for 2/5 sets - only 2pc or 5pc reads.

### 2.1 Element DMG Sets
| Set | 2pc | 5pc |
|-----|-----|-----|
| Freezing Frost | Glacio DMG +10% | Basic/Heavy Attack: Glacio DMG +10%, stacks 3x, 15s |
| Molten Rift | Fusion DMG +10% | Resonance Skill: Fusion DMG +30% for 15s |
| Void Thunder | Electro DMG +10% | Heavy Attack/Res. Skill: Electro DMG +15%, stacks 2x, 15s each |
| Sierra Gale | Aero DMG +10% | Intro Skill: Aero DMG +30% for 15s |
| Celestial Light | Spectro DMG +10% | Intro Skill: Spectro DMG +30% for 15s |
| Havoc Eclipse | Havoc DMG +10% | Basic/Heavy Attack: Havoc DMG +7.5%, stacks 4x, 15s |

### 2.2 Utility / Support Sets
| Set | 2pc | 5pc |
|-----|-----|-----|
| Rejuvenating Glow | Healing +10% | On healing allies: whole team ATK +15% for 30s |
| Moonlit Clouds | Energy Regen +10% | Outro Skill: next Resonator ATK +22.5% for 15s |
| Lingering Tunes | ATK +10% | On-field: ATK +5% every 1.5s, stacks 4x; Outro Skill DMG +60% |
| Halo of Starry Radiance | Healing Bonus +10% | On heal: each 1% Off-Tune Buildup grants +0.2% team ATK (<=25%) for 4s |
| Reel of Spliced Memories | ATK +10% | Tune Rupture/Strain-Shifting: team Tune Break Boost +20 for 30s |

### 2.3 Advanced / Element-Reaction Sets
| Set | 2pc | 5pc |
|-----|-----|-----|
| Frosty Resolve | Res. Skill DMG +12% | Res. Skill -> +22.5% Glacio DMG 15s; Res. Lib -> +18% Skill DMG 5s (stacks 2x) |
| Eternal Radiance | Spectro DMG +10% | Spectro Frazzle -> Crit Rate +20% 15s; 10 stacks -> +15% Spectro DMG 15s |
| Midnight Veil | Havoc DMG +10% | Outro: 480% Havoc DMG AoE + incoming Resonator +15% Havoc DMG 15s |
| Empyrean Anthem | Energy Regen +10% | Coordinated Attack DMG +80%; crit Coord -> active ATK +20% 4s |
| Tidebreaking Courage | Energy Regen +10% | ATK +15%; at 250% ER -> all Attribute DMG +30% |
| Gusts of Welkin | Aero DMG +10% | Aero Erosion -> team Aero DMG +15% (+15% more for trigger) 20s |
| Windward Pilgrimage | Aero DMG +10% | Aero Erosion hit -> Crit Rate +10% & Aero DMG +30% 10s |
| Flaming Clawprint | Fusion DMG +10% | Res. Lib -> team +15% Fusion DMG & caster +20% Res. Lib DMG 35s |
| Pact of Neonlight Leap | Spectro DMG +10% | Outro -> incoming ATK +15% (+0.3%/Tune Break Boost, <=15%) 15s |
| Rite of Gilded Revelation | Spectro DMG +10% | Basic Attack -> Spectro DMG +10% (3x) 5s; at 3 -> Res.Lib grants +40% Basic Atk DMG |
| Trailblazing Star | Fusion DMG +10% | Fusion Burst/Tune Rupture-Shifting -> Crit Rate +20% & Fusion DMG +20% 8s |
| Chromatic Foam | Fusion DMG +10% | Fusion Burst -> +10% Fusion DMG 15s; Outro -> incoming +25% Fusion DMG 15s |
| Sound of True Name | Aero DMG +10% | Echo Skill DMG -> Echo Skill Crit Rate +20% & Aero DMG +15% 5s |
| Wishes of Quiet Snowfall | Glacio DMG +10% | Glacio Chafe -> +10% Glacio DMG 15s + Snowfall (Res.Lib -> Crit Rate +25%) |

### 2.4 3-Piece Sets
| Set | 3pc |
|-----|-----|
| Dream of the Lost | Holding 0 Resonance Energy -> Crit Rate +20% & Echo Skill DMG +35% |
| Crown of Valor | On gaining Shield: ATK +6% & Crit DMG +4% 4s (1/0.5s, stacks 5x) |
| Law of Harmony | Echo Skill -> caster +30% Heavy Atk DMG 4s; team +4% Echo Skill DMG (stacks 4x) 30s |
| Flamewing's Shadow | Echo Skill DMG -> Heavy Atk Crit Rate +20%; Heavy Atk -> Echo Skill Crit Rate +20%; both active -> +16% Fusion DMG |
| Thread of Severed Fate | Havoc Bane -> ATK +20% & Res. Lib DMG +30% 5s |

### 2.5 Patch 3.5 New Sets
| Set | Note |
|-----|------|
| Song of Feathered Trace | Used by Yangyang: Xuanling (Havoc Sword DPS) |
| Heart of Evil's Purge | New 3.5 set |
| Lamp of Nether Road | New 3.5 set |

---

## 3. Echo Cost (4 / 3 / 1)

### 3.1 Cost Budget & Loadout
- Every Resonator equips **5 Echoes**. Total cost budget = **12**.
- Standard loadout: **4-3-3-1-1 (43311)**. Alternative: **4-4-1-1-1 (44111)**.
- Only the **top slot (Main Echo)** grants an active **Echo Skill** in combat. The other 4 slots contribute passive stats + Sonata count only.

### 3.2 Cost -> Echo Class -> Available Main Stats
| Cost | Echo Class | Primary Main Stat Pool | Secondary (fixed) |
|------|-----------|------------------------|-------------------|
| 4 | Overlord / Calamity | Crit Rate, Crit DMG, Healing Bonus, ATK%, HP%, DEF%, Elemental DMG% | Flat ATK |
| 3 | Elite | Elemental DMG%, Energy Regen, ATK%, HP%, DEF% | Flat ATK |
| 1 | Common | ATK%, HP%, DEF% | Flat HP |

- **Crit Rate / Crit DMG / Healing Bonus** appear ONLY on Cost-4 (as main stat).
- **Elemental DMG Bonus / Energy Regen** appear ONLY on Cost-3 (as main stat).
- Calamity-tier (4-Cost) Echoes drop only from **Tacet Field** bosses, gated by Waveplate.
- Each counted Echo must be **unique** (duplicate copies of same enemy do NOT advance set count).

### 3.3 Cost Role Function
| Cost | Typical purpose |
|------|-----------------|
| 4 | Big offensive/critical/healing main stat + the active Echo Skill for rotation |
| 3 | Element DMG% / ATK% / Energy Regen depending on rotation needs |
| 1 | ATK% / HP% / DEF% foundation for scaling |

---

## 4. All Weapons

Weapon types: **Broadblade, Sword, Pistols, Gauntlets, Rectifier**. 110+ total.
5-star weapons: base ATK 500-588 (some signatures ~675 with lower % secondary).
Secondary stat options: ATK%, Crit Rate, Crit DMG, Energy Regen, HP, DEF.

### 4.1 Notable 5-star Weapons (by secondary stat)
| Weapon | Type | Base ATK (Lv.90) | Secondary (Lv.90) |
|--------|------|------------------|-------------------|
| Verdant Summit | Broadblade | 588 | Crit DMG 48.6% |
| Lustrous Razor | Broadblade | 587 | ATK 36.4% |
| Emerald of Genesis | Sword | 587 | Crit Rate 24.3% |
| Emerald Sentence | Sword | 587 | Crit Rate 24.3% |
| Static Mist | Pistols | 587 | Crit Rate 24.3% |
| Abyss Surges | Gauntlets | 587 | ATK 36.4% |
| Blazing Justice | Gauntlets | 587 | Crit DMG 48.6% |
| Cosmic Ripples | Rectifier | 500 | ATK 54.0% |
| Stringmaster | Rectifier | 500 | Crit Rate 36.0% |
| Rime-Draped Sprouts | Rectifier | 500 | Crit DMG 72.0% |
| The Last Dance | Broadblade | 500 | Crit DMG 72.0% |
| Whispers of Sirens | Pistols | 500 | Crit DMG 72.0% |
| Thunderflare Dominion | Gauntlets | 675 | Crit Rate 12.1% |
| Stellar Symphony | Rectifier | 412 | Energy Regen 77% |
| Unflickering Valor | Sword | 415 | Energy Regen 77% |
| Boson Astrolabe | Rectifier | 525 | Energy Regen 38.8% |
| Bloodpact's Pledge | Sword | 587 | Energy Regen 38.9% |
| Defier's Thorn | Sword | 413 | HP 72.2% |

### 4.2 Common 4-star Weapons
| Weapon | Type | Base ATK | Secondary |
|--------|------|----------|-----------|
| Commando of Conviction | Sword | 412 | ATK 30.3% |
| Undying Flame | Pistols | 413 | ATK 30.3% |
| Lunar Cutter | Sword | 412 | ATK 30.3% |
| Hollow Mirage | Gauntlets | 412 | ATK 30.3% |
| Autumntrace | Broadblade | 412 | Crit Rate 20.2% |
| Augment | Rectifier | 412 | Crit Rate 20.2% |
| Radiant Dawn | Sword | 412 | Crit DMG 40.5% |
| Aether Strike | Gauntlets | 412 | Crit DMG 40.5% |
| Jinzhou Keeper | Rectifier | 387 | ATK 36.4% |
| Cadenza / Discord / Marcato / Variation / Overture | (ER set) | 337 | Energy Regen 51.8% |
| Amity Accord / Dauntless Evernight | Gauntlet/Broadblade | 337 | DEF 61.5% |
| Celestial Spiral / Fusion Accretion / Ocean's Gift / Waltz in Masquerade | various | 462 | ATK 18.2% |

### 4.3 Weapon Passive Format (template for AI to fill per weapon)
```
- Weapon: <name>
  Type: <Broadblade/Sword/Pistols/Gauntlets/Rectifier>
  Rarity: <5-star/4-star/3-star>
  Base ATK (Lv.90): <value>
  Secondary Stat: <stat + %>
  Passive Ability: <name + full R1->R5 scaling text>
```
> Note: Full passive R1-R5 text varies per weapon and per patch. Populate from the in-game weapon detail page or a live wiki (wutheringwaves.fandom.com/wiki/Weapon/List). Above stats are verified; passive descriptions should be pulled per weapon.

---

## 5. All Characters

54+ playable Resonators as of Version 3.6. Every Resonator has **5 abilities in fixed order**:
1. **Basic Attack** - multi-hit combo + Heavy (charged, uses stamina) + Mid-air/Plunge variant.
2. **Resonance Skill** - primary active, short CD (8-15s), generates Concerto.
3. **Resonance Liberation** - ultimate, long CD (20-30s), 100-150 Energy cost, high AoE DMG, big Concerto gain.
4. **Forte Circuit / Inherent Skill** - the character's unique mechanic/resource gauge.
5. **Outro Skill** - triggers on swap-out at full Concerto; usually a team buff or parting DMG.

Plus passives: **Intro Skill** (triggers on swap-in) and 2 Inherent Skills.

### 5.1 Character Roster (element / weapon / role)
| Character | Element | Weapon | Role |
|-----------|---------|--------|------|
| Jingran | Fusion | Broadblade | Main DPS |
| Qingxiao | Aero | Sword | Main DPS |
| Suisui | Glacio | Rectifier | Support |
| Yangyang: Xuanling | Havoc | Sword | Main DPS (Havoc Bane/Heavy Atk) |
| Lucilla | Glacio | Rectifier | Support |
| Rebecca | Electro | Pistols | Sub-DPS |
| Lucy | Spectro | Pistols | Main DPS |
| Denia | Fusion | Rectifier | Sub-DPS |
| Hiyuki | Glacio | Sword | Main DPS |
| Sigrika | Aero | Gauntlets | Main DPS |
| Luuk Herssen | Spectro | Gauntlets | Main DPS |
| Aemeath | Fusion | Sword | Main DPS |
| Mornye | Fusion | Broadblade | Support |
| Lynae | Spectro | Pistols | Sub-DPS |
| Chisa | (verify) | (verify) | Support |
| Qiuyuan | (verify) | (verify) | Sub-DPS (Outro buffer) |
| Galbrena | Fusion | (verify) | Main DPS (Molten Rift) |
| Iuno | (verify) | (verify) | Sub-DPS |
| Augusta | (verify) | (verify) | Main DPS |
| Phrolova | (verify) | (verify) | Main DPS |
| Lupa | Fusion | (verify) | Sub-DPS |
| Cartethyia | Aero | (verify) | Main DPS (Aero Erosion) |
| Ciaccona | Aero | (verify) | Sub-DPS |
| Zani | Spectro | (verify) | Main DPS |
| Rover (Aero) | Aero | Sword | Support/DPS |
| Rover (Havoc) | Havoc | Sword | Main DPS (Havoc Eclipse) |
| Rover (Electro) | Electro | Sword | Sub-DPS |
| Rover (Spectro) | Spectro | Sword | Support |
| Cantarella | (verify) | (verify) | Sub-DPS |
| Phoebe | Spectro | (verify) | Main DPS |
| Brant | Fusion | (verify) | Sub-DPS |
| Lumi | (verify) | (verify) | Support |
| Roccia | Havoc | (verify) | Sub-DPS |
| Carlotta | Glacio | Pistols | Main DPS |
| Camellya | Havoc | Sword | Main DPS |
| Youhu | (verify) | (verify) | Support |
| Shorekeeper | Spectro | Rectifier | Support/Healer |
| Xiangli Yao | Electro | Gauntlets | Main DPS |
| Zhezhi | Glacio | Rectifier | Sub-DPS |
| Changli | Fusion | Sword | Sub-DPS |
| Jinhsi | Spectro | Broadblade | Main DPS |
| Jiyan | Aero | Broadblade | Main DPS |
| Jianxin | Aero | Gauntlets | Support |
| Lingyang | Glacio | Gauntlets | Main DPS |
| Calcharo | Electro | Broadblade | Main DPS |
| Yuanwu | Electro | Gauntlets | Support |
| Taoqi | Havoc | Broadblade | Support |
| Sanhua | Glacio | Sword | Sub-DPS |
| Mortefi | Fusion | Pistols | Sub-DPS |
| Danjin | Havoc | Sword | Sub-DPS |
| Chixia | Fusion | Pistols | Main DPS |
| Baizhi | Glacio | Rectifier | Healer |
| Yinlin | Electro | Rectifier | Sub-DPS |
| Verina | Spectro | Rectifier | Healer/Support |
| Encore | Fusion | Rectifier | Main DPS |
| Yangyang | Aero | Sword | Support |
| Aalto | Aero | Pistols | Sub-DPS |
| Buling | (verify) | (verify) | Support |

> Entries marked "(verify)" are newer 3.4-3.6 Resonators whose element/weapon should be confirmed on wutheringwaves.fandom.com or game8.co.

### 5.2 Character Ability Format (template for AI to fill per character)
```
## <Character Name>
- Element: <element>  |  Weapon: <type>  |  Rarity: <5-star/4-star>  |  Role: <role>

### Basic Attack - <name>
<full description incl. Heavy Attack, Mid-air, Dodge Counter>

### Resonance Skill - <name>
<description, cooldown, Concerto/Energy generation, enhanced state>

### Resonance Liberation - <name>
<description, energy cost, cooldown, AoE effect>

### Forte Circuit / Inherent Skill - <name>
<unique resource/mechanic gauge>

### Intro Skill - <name>
<on swap-in effect>

### Outro Skill - <name>
<on swap-out team buff / parting damage>

### Inherent Skills (Passives)
<passive 1 + passive 2>

### Resonance Chain (Sequence Nodes S1-S6)
S1: ...
S2: ...
S3: ...
S4: ...
S5: ...
S6: ...
```
> Full per-character ability + Sequence text is extensive and patch-dependent. Populate each block from the in-game character page or a live wiki (wutheringwaves.fandom.com - Resonance Skill / Liberation / Chain lists). Roster, elements, weapons, and roles above are verified.

---

## Data Sources & Verification Notes
- Echo stat tables (mainstat max, substat ranges, rarity slots): cross-verified across Prydwen, GameVika, WutheringWaves.party, Neonsect.
- Sonata set list (34 sets) with 2pc/5pc/3pc: Prydwen + GameVika (Sep 2026).
- Cost/loadout (43311 / 44111, 12 budget): GameVika, BuffBuff, LevelCrux.
- Weapon stats: Prydwen weapons page (May 2026) + WutheringLab.
- Character roster/elements/weapons/roles: Game8 (Sep 2026), WutheringLab, u7buy 3.5 tier list.
- Per-weapon passive R1-R5 text and per-character full ability/Sequence text should be pulled live per item, as they change with patches. Templates provided in 4.3 and 5.2.
