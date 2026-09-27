# Data Quality & Coverage

Snapshot: 2026-09-20. This is a secondary-source, source-linked research corpus, not an official Kuro game-data export and not a live in-game test.

## Coverage manifest

| Dataset | Included | Meaning |
|---|---:|---|
| Echo mainstats | 88 cost/rarity/stat rows | +0 and maximum values from two sources, with conflicts preserved |
| Echo substats | 13 types | Discrete rolls, not official drop probabilities |
| Sonata sets | 34 | All collected nonempty set-effect rows |
| Echo skills | 181 | 43 Cost 4; 53 Cost 3; 85 Cost 1 |
| Weapons | 122 | Named passive mechanics and R1–R5 parameters; two secondary-only refinements flagged |
| Character kits | 58 | Variants counted separately; 348 chain nodes |
| Supplementary Echo pages | 23 | Missing data checked against a second source |

Counts are generated from the included normalized records, not inferred from a site's headline count. The inventory follows the fetched [Echo list](https://game8.co/games/Wuthering-Waves/archives/452491), [weapon list](https://game8.co/games/Wuthering-Waves/archives/452490), [Sonata list](https://game8.co/games/Wuthering-Waves/archives/456215) and the per-character/per-item pages linked in the datasets.

## Inclusion and exclusion

- The source pages show a 3.6-era database with 3.7 previews; this pack does not certify every entry's exact live-release status on every region/server. See [Game8 version overview](https://game8.co/games/Wuthering-Waves/archives/559680).
- Five Echo rows with TBD identifiers/skills were excluded: Formrender, Skywatch Lancer, Soulfrayer, Bloomburst Puppet and Jade Nether Serpent. They are not silently treated as completed entries. ([Game8 Echo List](https://game8.co/games/Wuthering-Waves/archives/452491))
- The term “all” in filenames means all records in the researched inventory, not a guarantee of exhaustive future or hidden content. Character variants are separate kit records; aliases are not extra characters.
- Values are factual paraphrases of fetched pages. Full raw editorial articles, lore, images, builds and copyrighted page dumps are not bundled.

## Resolved or explicitly preserved conflicts

- **Mainstats:** 39 cost/rarity/stat rows have differing or missing endpoints between Game8 and Wiki. Both readings are included; `null` marks an unresolved numeric endpoint in JSON. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456278); [Wiki](https://wutheringwaves.fandom.com/wiki/Echo/Stats))
- **Reroll rule:** Older stats pages say substats cannot change; the current Transducer guide gives a reroll workflow. The pack follows the newer, specific Transducer guide rather than repeating the old absolute claim. ([Game8 Transducer](https://game8.co/games/Wuthering-Waves/archives/578127); [Wiki](https://wutheringwaves.fandom.com/wiki/Echo/Stats))
- **Tyro / Training:** Passive values were replaced with individually fetched Game8 R1–R5 tables. Tyro starts at 5% ATK; Training starts at 4%, not the lower values encountered elsewhere. ([Tyro Broadblade](https://game8.co/games/Wuthering-Waves/archives/455942); [Training Broadblade](https://game8.co/games/Wuthering-Waves/archives/455941))
- **Abyss Surges:** R1 Energy Regen is recorded as 12.8%, consistent between Game8 and Wuthering.gg; a conflicting WuWaBuild value is not used. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455915); [Wuthering.gg](https://wuthering.gg/weapons/abyss-surges))
- **Lumingloss / Thunderbolt:** Game8 lacks R2–R5. Theria Games supplies the progression, which is marked secondary-only and should be checked in game before precise optimization. ([Lumingloss](https://theriagames.com/guide/wuthering-waves-lumingloss/); [Thunderbolt](https://theriagames.com/guide/wuthering-waves-thunderbolt/))
- **Jiyan:** Prydwen corrects the Normal Attack trigger wording for Abyssal Slash / Banner of Triumph; numeric Lv.1 rows remain attributed to Game8. ([Prydwen](https://www.prydwen.gg/wuthering-waves/characters/jiyan))
- **Echo rank versus rarity:** Supplementary pages sometimes show inconsistent rank labels. Their coefficients are kept in a separate evidence block instead of being silently combined with the main rarity-5 block. ([Dreamless](https://wuthering.gg/echos/dreamless))

## Character limitations by record

These are source omissions or ambiguities, not necessarily missing gameplay mechanics. A mechanic having no duration in its source does not prove that it has no duration.

### Aalto

- The evidence does not provide Aalto's exact Mist Drop maximum, initial quantity, recovery cap, consumption timing, or complete Forte Circuit resource rules. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))
- The evidence does not specify the exact HP-scaling formula for Mist Avatar beyond stating that its level-1 HP value is 100% and that S2 grants 100% more inherited HP. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))
- The target, duration, stacking behavior, and exact qualifying projectile rules for the Gate of Quandary ATK increase are not fully specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))
- The source's Normal Attack text contains corrupted wording around Mist Shot and does not clearly distinguish it from the separately listed Mid-Air Attack beyond saying it consumes Stamina and fires mid-air shots. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))
- The source lists S4's “Vaporized Bullet” and “Mist Stealth state,” but neither term is defined in the supplied ability descriptions; the relationship to Mist Missile and Mistcloak Dash is therefore ambiguous. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))
- The source does not provide level-1 quantitative tables for Inherent Skills, Outro, Tune Break, or the individual Resonance Chain effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))
- The supplied page text includes attribute-bonus rows, but their exact unlock placement and whether repeated Aero DMG Bonus/ATK entries belong to separate skill nodes are not fully clear. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454214))

### Aemeath

- The fetched evidence does not provide a separate general Resonance Mode activation/switch mechanic. ([Game8](https://game8.co/games/Wuthering-Waves/archives/572587))
- The source's Normal Attack table lists Aemeath and Mech variants but does not provide a separate standalone Mech Normal Attack category outside Shared Voyage. ([Game8](https://game8.co/games/Wuthering-Waves/archives/572587))
- Exact scaling-stat labels are not supplied; listed percentages are reproduced without inferring whether they scale from ATK or another stat. ([Game8](https://game8.co/games/Wuthering-Waves/archives/572587))
- The S5 shield duration appears as 'for 5' in the source; it is interpreted only as 5 seconds because the surrounding text describes a duration, but the source formatting is broken. ([Game8](https://game8.co/games/Wuthering-Waves/archives/572587))
- No skill-level progression beyond the supplied Effect (Lvl 1) rows is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/572587))
- The source contains navigation/recommendation fragments, but they do not define additional ability mechanics and were excluded. ([Game8](https://game8.co/games/Wuthering-Waves/archives/572587))

### Augusta

- The fetched evidence does not provide explicit level-scaling formulas beyond the displayed skill Lv.1 tables; no Lv.10 values were inferred. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))
- The source gives no separate quantitative table for the Normal Attack attribute-node bonuses beyond listing Crit. Rate +1.20% and +2.80%; these values are retained in the mechanics. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))
- The source gives no separate quantitative table for the Resonance Skill and Liberation attribute-node bonuses beyond listing their ATK effects; these values are retained in the mechanics. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))
- The source does not state a numeric shield value, duration, trigger interval, or other details for any effects introduced by Sequence 5 beyond its 50% increase. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))
- The source's Sequence 6 wording names 'Heavy Attack - Thunder Rage' although the base ability section names Thunderoar attacks; the wording has been retained without resolving whether this is a separate or alternate name. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))
- The source does not provide a damage value or additional effect for Tune Break: Broadblade. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))
- The source does not state a numeric effect for Blazing Valor's Crown of Wills restoration beyond 'fully restore'. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524890))

### Baizhi

- The evidence does not explicitly identify whether every listed HP or Health scaling value uses current HP or Max HP; values are retained using the source wording. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454224))
- The Emergency Plan Forte Circuit table labels are ambiguous: “Heavy Attack with ‘Concentration’ Con. Energy Regen: 4,” “Resonance Skill with ‘Concentration’ Con.: 8,” and “Heavy Attack ‘Concentration’ Con.: 2.5” do not clearly state whether each is per consumed Concentration or a total. The mechanics text confirms that Heavy Attack restores Resonance and Concerto Energy, while Emergency Plan restores Concerto Energy. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454224))
- The source does not provide separate numerical tables for the inherent skills, Outro Skill, Tune Break, Euphonia, or most additional effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454224))
- The source states that Remnant Entities automatically consume stacks every 2.5 seconds but does not explicitly state a duration or whether the entities disappear when stacks reach zero. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454224))
- The source does not specify the exact target range for “nearby” beyond using that term. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454224))
- The source does not specify whether the team-wide healing wording includes Baizhi in every instance, although it states “entire team” or “all team members nearby.” ([Game8](https://game8.co/games/Wuthering-Waves/archives/454224))

### Brant

- The source does not state the numerical amount of Bravo gained from Normal Attacks, Intro Skill, or Resonance Skill hits; only the triggers and the 100 Bravo maximum are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))
- The Waves of Acclaims healing entry is malformed as “312+1.09\*per 1% Energy Regen”; its exact formula and missing operation are unsupported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))
- The Shield entry is malformed as “2500+9”; the scaling term and formula are unsupported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))
- The Resonance Liberation healing entry is given only as “500+1.75” without a stated scaling variable or operation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))
- The source labels some mid-air attacks as “Charged Attack” and contains apparent typographical errors such as “Mid-air Chargef Attack,” “Interlufe,” and “Basick Attack”; these have been normalized only where the intended mechanic is clear. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))
- The source does not provide separate numerical tables for Inherent Skills, Outro Skill, or Tune Break. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))
- The source does not explicitly state a numerical cooldown for Returned from Ashes or a duration for the Aflame state beyond the separate 12-second Aflame Duration entry. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486245))

### Buling

- The evidence does not provide a separate numeric table for Forte Circuit resource requirements, Minor Yin/Minor Yang capacity, or the exact duration of the Yin-Yang Balance state. ([Game8](https://game8.co/games/Wuthering-Waves/archives/557981))
- The evidence does not specify the numerical damage or duration of the target Vibration Strength reduction from Heavy Attack – Thunder Over Mountain. ([Game8](https://game8.co/games/Wuthering-Waves/archives/557981))
- The evidence does not provide a separate numeric table for Outro Skill healing or damage amplification beyond the stated percentages and durations. ([Game8](https://game8.co/games/Wuthering-Waves/archives/557981))
- The evidence identifies Flashing Thunder Spell: Harmony as replacing the normal Liberation during Yin-Yang Balance, but does not state whether the replacement shares the normal Liberation cooldown or Resonance Energy cost. ([Game8](https://game8.co/games/Wuthering-Waves/archives/557981))
- The source labels the S3 emergency restoration value as based on Buling’s ATK but does not provide a dedicated skill-level table; it is reported directly from the node description. ([Game8](https://game8.co/games/Wuthering-Waves/archives/557981))
- The source does not define the damage classification of the listed attacks beyond identifying their Electro DMG where stated, and does not provide switch-out behavior beyond the Intro and Outro descriptions. ([Game8](https://game8.co/games/Wuthering-Waves/archives/557981))

### Calcharo

- The evidence does not provide an explicit time limit for recasting Extermination Order before its switch-out/recast condition causes cooldown. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454217))
- The Forte Circuit table contains two separate Con. Energy Regen entries for Mercy and Death Messenger; the source does not identify whether the second pair represents a different energy type, so both rows are retained verbatim. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454217))
- The source's named Intro Skill is Wanted Outlaw, but S2 and S5 call the corresponding skill Wanted Criminal; the evidence does not resolve whether this is a naming inconsistency or a separate skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454217))
- The source does not provide a separate numerical multiplier for the increased Deathblade Gear Dodge Counter damage beyond the listed Heavy Attack/Dodge Counter table rows. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454217))
- The source does not specify the exact target-selection behavior or duration of the Shadowy Raid Phantom beyond attacking targets in front and supporting the on-field Resonator. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454217))

### Camellya

- The source's Ephemeral table displays “635.00%%,” which is malformed; its numerical value is recorded as n.a. rather than corrected. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source does not state the scaling stat for any damage value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source does not provide a numerical base value for Sweet Dream's DMG Multiplier, only its Crimson Bud increase and S6 modifications. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source repeats “Vining Waltz 1 STA Cost: 5” four times; the repeated rows are retained exactly, but their intended labels cannot be determined. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source does not provide separate quantitative tables for Inherent Skills, Tune Break, or the Resonance Chain effects; their numerical details are recorded only where the node descriptions explicitly state them. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The S5 description calls Everblooming an Outro Skill and Twining an Intro Skill, conflicting with the main listing, which identifies Everblooming as Intro and Twining as Outro. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source does not explicitly state whether the 100 Crimson Pistils restored by Intro Skill Everblooming and Ephemeral are subject to the 100-Pistil holding cap, beyond separately stating that the cap is 100. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source mentions targets for damage attacks but does not specify target counts, area size, or other targeting restrictions. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))
- The source provides no shield, healing, or defensive effect descriptions beyond interruption resistance and interruption immunity. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473332))

### Cantarella

- The evidence does not provide separate numerical damage or cost tables for Mirage entry, Trance, Shiver, Hazy Dream application, or the Coordinated Attacks beyond the listed rows. ([Game8](https://game8.co/games/Wuthering-Waves/archives/500493))
- The source states that some effects are classified as Basic Attack DMG or Echo Skills, but does not provide additional scaling formulas for those classifications. ([Game8](https://game8.co/games/Wuthering-Waves/archives/500493))
- The source does not provide a standalone numerical table for Tune Break beyond its full Off-Tune trigger condition. ([Game8](https://game8.co/games/Wuthering-Waves/archives/500493))
- The source's attribute-bonus rows are included with the associated skill, but their upgrade-level behavior is not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/500493))
- The source does not explicitly state whether the generic first damage instance that triggers Jolt must come from Cantarella; it only states that Cantarella triggers Jolt and that other Resonators remove Hazy Dream without triggering it. ([Game8](https://game8.co/games/Wuthering-Waves/archives/500493))

### Carlotta

- The evidence provides only skill Lv.1 values; no higher-level values are supported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486251))
- No numerical duration is provided for Moldable Crystal gain windows beyond the stated 10-second Moldable Crystal duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486251))
- The evidence describes Final Bow's switch-out and Twilight Tango ending conditions but does not provide a separate duration for the Final Bow state. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486251))
- The source navigation text is truncated, and some table labels are compressed, but the listed ability names and Lv.1 values are readable. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486251))
- The evidence mentions an Outro Skill named Kaleidoscope Sparks in S3 but does not provide a standalone base description for that skill; only its additional Closing Remark strike is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486251))

### Cartethyia

- The evidence does not provide a numerical Conviction gain per Fleurdelys hit or a stated Conviction cap beyond the 120-point activation threshold. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))
- The duration or timing window for casting May Tempest Break the Tides before the skill enters cooldown is not numerically specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))
- The source describes the Forte as Mid-air Attack Stage 2 in the Liberation text but the Forte skill table lists only Mid-air Attack Stages 1–3; the exact mapping of all transformed mid-air stages is ambiguous. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))
- The inherent-skill wording says targets with more than 3 Aero Erosion stacks receive an additional 10% per stack, up to 3 stacks; the exact interpretation of the total stack-based multiplier is not further clarified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))
- No numerical values are supplied for the Stagnate duration, interruption-resistance increase, force-field ranges, pull strength, water-walking Stamina drain, or Aero Erosion damage itself. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))
- The source labels the Tune Break trigger but supplies no damage, duration, cooldown, or other effect details. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))
- The source supplies attribute-bonus rows but does not explicitly assign them to individual upgrade nodes beyond the listed skill sections. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507777))

### Changli

- The fetched character-information table is visibly truncated, so fields such as How to Get and voice actor are unsupported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/452826))
- The source does not provide level-10 values; all quantitative values above are explicitly labeled skill Lv.1. ([Game8](https://game8.co/games/Wuthering-Waves/archives/452826))
- The source states that Basic Attack 4 and Mid-air Attack 4 enter True Sight for 12s, but does not provide a separate cooldown or attempt system for those entries. ([Game8](https://game8.co/games/Wuthering-Waves/archives/452826))
- The source does not specify the exact ATK scaling formula or target count beyond the stated nearby-target wording for Resonance Liberation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/452826))
- The source does not define the exact damage or resistance-to-interruption value for Sequence 1's resistance effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/452826))
- The source presents the True Sight - Capture, Conquest, and Charge entries under Resonance Skill, while Flaming Sacrifice is presented under Forte Circuit but classified as Resonance Skill DMG; their source categorization is retained as stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/452826))

### Chisa

- The source gives no character-level base statistics, upgrade-level values, exact durations for several input windows, exact Chainsaw Fever depletion rates, or exact Lifethread passive-generation rate. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524880))
- The source states that Death Snip and Moment of Nihility heal nearby team Resonators, but does not specify whether the listed healing values are single-target, total, or otherwise distributed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524880))
- The source labels Sawring - Eradication's Ring of Chainsaw bonus as a DMG multiplier but does not state the exact formula or whether the listed 1.30% is additive or multiplicative. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524880))
- The source contains navigation fragments and does not provide separate detailed skill tables for the attribute bonuses shown in the page text; those bonuses are therefore not treated as standalone abilities. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524880))

### Chixia

- The evidence does not provide an explicit numerical acquisition amount for Thermobaric Bullets from Normal Attack POW POW, Intro Skill Grand Entrance, or Resonance Skill Whizzing Fight Spirit. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))
- The rate or timing at which Thermobaric Bullets are consumed during DAKA DAKA! is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))
- The damage scaling for the regular DAKA DAKA! attacks and the exact damage formula for Boom Boom are not separately provided beyond the listed Forte table rows. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))
- The evidence gives a 60-round base Thermobaric Bullet cap and states that Scorching Magazine adds 10 rounds, but it does not explicitly state the resulting cap in a separate effect line. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))
- The Resonance Chain 5 description refers to an inherent skill named Numbingly Spicy!, while the listed Inherent Skill 2 is named Spicy and Numbing; the evidence does not resolve whether these are the same skill or a naming inconsistency. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))
- The source labels the numeric values as Skill Detail / Effect (Lvl 1), but does not provide level-scaling information beyond those Lv.1 values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))
- The source does not state switch-out behavior, shields, healing, or additional restrictions for these abilities. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454220))

### Ciaccona

- The evidence does not provide numerical damage values for the individual Green Tonic and Yellow Tonic effects beyond the shared Symphonic Poem: Tonic DMG row. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507924))
- The evidence does not define the amount of Concerto Energy restored by the normal Recital Tonic interaction; only Successful Interaction Concerto Regen: 10 is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507924))
- The evidence does not explain Off-Tune Level mechanics, its accumulation, or Tune Break's damage/effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507924))
- The evidence does not provide the number of charges or recharge behavior for Resonance Skill beyond Sequence 3 granting one additional charge. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507924))
- The source lists attribute bonuses but does not clearly identify whether their displayed values are separate node effects or cumulative values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/507924))

### Danjin

- The evidence does not provide the exact amount of Ruby Blossom gained per Resonance Skill use. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454227))
- The evidence describes a special condition when Ruby Blossom exceeds 120 and a 120-Ruby-Blossom consumption, but does not explicitly label 120 as the resource's maximum cap. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454227))
- The exact HP basis for Chaoscleave's 36% HP healing is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454227))
- The evidence does not provide the duration, stack behavior, or other limits for Incinerating Will beyond its 12-second duration and its 20% Danjin damage increase against marked targets. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454227))
- The evidence does not provide the exact timing or detailed hit behavior of the HP cost attached to Incinerating Will/Incinerating Will use beyond stating that each attack consumes 3% of maximum HP. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454227))
- No separate numerical effect table is supplied for the inherent skills, Outro, Tune Break, or Resonance Chain nodes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454227))

### Denia

- The evidence supports Fusion as the element, Rectifier as the weapon, and 5-star rarity, but does not provide complete Resonator information such as acquisition method or voice actor. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))
- The source does not explain how Denia enters, selects, or changes between Resonance Mode - Fusion Burst and Resonance Mode - Tune Strain. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))
- The source does not provide a separate numerical table for Tune Break, Outro, Inherent Skills, or most passive effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))
- The source states that Void Particle is consumed by Breakdown Form Normal Attacks but does not specify the exact amount consumed per hit. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))
- The source does not specify the exact Off-Tune Level, Tune Strain, or Fusion Burst stack durations except where explicitly stated, nor does it define the full behavior of Tune Strain - Interfered. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))
- The source gives S5 as Final Act - Stagecraft Form DMG increased by 100% and S6 as a 200% Fusion Burst DMG multiplier increase, but does not clarify whether these are additive damage increases or multiplier changes beyond the wording provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))
- The extracted page contains a broken navigation/stat table and does not provide complete base-stat or progression data. ([Game8](https://game8.co/games/Wuthering-Waves/archives/585681))

### Encore

- The fetched evidence does not provide Encore's acquisition method or English voice actor. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454221))
- The source presents attribute-bonus entries for several abilities, but does not clearly associate every entry with a named node or provide a complete skill-tree mapping; those bonuses are not treated as separate abilities. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454221))
- The source's Forte text uses both 'Dissonance state' and 'Cosmos' Dissonance state'; no separate duration is provided for either state beyond the stated trigger and ending conditions. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454221))
- The source does not provide level-scaling tables beyond the listed skill Lv.1 values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454221))

### Galbrena

- The evidence does not provide Galbrena's acquisition method, voice actor, or other character-information fields. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))
- The exact Sinflame recovery amount per qualifying attack is not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))
- The evidence does not state Galbrena's maximum STA, Purging Flame generation amount beyond the one-to-one Sinflame conversion, or whether any resources persist when switching out. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))
- The source gives no separate numerical Skill Detail table for Ashen Pursuit, Tune Break, Inherent Skills, or the sequence effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))
- The source labels Ashen Pursuit as an Outro Skill but provides only its ATK scaling expression and no duration, cooldown, target restrictions, or switch-out behavior. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))
- The wording for S6 says Eternal Hypostasis lasts but does not provide a separate duration; the base Demon Hypostasis limit of more than 50 seconds is the only stated duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))
- No additional shields, heals, crowd-control effects, or switch-out rules are supported by the evidence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524888))

### Hiyuki

- The evidence does not specify the scaling stat or full damage formulas for the listed attacks. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- Several effects refer to an unspecified range, duration window, valid-target condition, or exact timing window; those values are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- The exact DMG multiplier for Glacio Bite's stack-based instance is not provided; only its dependence on the target's current Glacio Bite stack limit is stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- The exact Frostbind and Stagnate durations/effects are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- The evidence does not provide a separate numerical Skill Detail table for Forte resource restoration beyond the explicitly stated values, or for Inherent Skills, Outro Skill, or Tune Break. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- The source uses both 'Glacio Chafe' and 'Glacio Bite' conversion wording; the reference preserves the stated rule that Glacio Bite counts as Glacio Chafe and Glacio Bite DMG counts as Glacio Chafe DMG. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- The source does not provide the exact DMG increase formula for Foreclaiming: Blade Liberation beyond the listed base and per-Snowforged-Blade values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))
- The phrase '2 charges of Frostblight: Jade Cleave' in S2 is reproduced as stated, although the base skill table lists Jade Cleave/Petalfall as sharing a single 12-second cooldown. ([Game8](https://game8.co/games/Wuthering-Waves/archives/586421))

### Iuno

- The evidence does not provide the exact Sentience restored by Moonring Basic Attack, Moonring Dodge Counter, or Mid-air Attack while in Lunar Cycle. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524889))
- The evidence does not provide the exact Sentience costs for Moonbow Basic Attack, Moonbow Dodge Counter, or Arc Beyond the Edge in New Moon. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524889))
- The evidence does not specify the exact ATK-scaling notation for Moonbow Basic Attack 2 Healing; the source table states only 13.03%. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524889))
- The evidence does not provide the duration of the S3 window during which Arc Beyond the Edge does not reset the Moonbow Basic Attack cycle. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524889))
- The source includes navigation labels and an incomplete general information table, but no additional ability mechanics are supplied there. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524889))
- The source does not provide separate numerical tables for the Tune Break effect, Outro amplification duration beyond the stated prose, or the Inherent Skill 2 stack duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524889))

### Jianxin

- The fetched evidence does not state the exact numerical Chi gain from any listed source or the Chi consumption rate during Zhoutian Progress. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))
- The fetched evidence does not specify Jianxin's base statistics, scaling-stat labels for the percentage damage values, or the exact shield scaling interpretation beyond the displayed formulas. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))
- The Normal Attack, Resonance Skill, Forte Circuit, Resonance Liberation, and Intro tables provide Level 1 values only; no higher-level values are supported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))
- Some attribute-bonus entries identify bonuses but not the node or unlock condition associated with each bonus. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))
- The Forte Circuit description mentions Chi Strike but provides no separate Chi Strike damage row in the supplied table. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))
- The source uses both “Primordial Chi Spiral” and the S6 text's “Primordial Qi Spiral”; this reference treats them as the same named Forte Circuit attack based on context. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))
- The source's extracted contents table is malformed, but the supplied ability sections identify the listed abilities and their mechanics. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454213))

### Jingran

- The source does not provide a numerical value for the Fire of Life-based DMG multiplier increase on Soul Raid and Stardome Meander. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605307))
- The source gives no separate skill-detail table for Forte Circuit attacks Soul Raid or Stardome Meander. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605307))
- The source does not state a numeric damage value for the summoned Chimei Wangliang attacks beyond the Resonance Liberation table value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605307))
- The source's broadblade Tune Break entry provides no damage or other numeric values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605307))
- The source includes attribute-bonus rows under Edge of Life and Death and Malevolent Encounter, but does not provide separate level-scaling context; values are retained exactly as shown and labeled skill Lv.1. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605307))
- The source does not explicitly provide a separate numeric damage table for Shadow Step beyond the listed '30+25' value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605307))

### Jinhsi

- The fetched evidence does not provide a separate scaling-stat description for the abilities. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- The Heavy Attack DMG value in the Normal Attack table is malformed and cannot be reliably reconstructed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- The Overflowing Radiance DMG value is malformed and cannot be reliably reconstructed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- The Incarnation - Basic Attack 2 DMG value contains a malformed percentage (13.0.8%) and cannot be reliably reconstructed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- No separate numerical damage or effect table is provided for Crescent Divinity beyond its Spectro DMG, 10s cooldown, and 8 Concerto Regen. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- No separate quantitative table is provided for Inherent Skills, Temporal Bender, Tune Break, Eras in Unity, Incarnation, or Unison beyond values stated in their mechanics. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- The evidence does not state how Incarnation is entered except that Overflowing Radiance sends Jinhsi into it, nor does it state whether Incarnation can be manually ended by any other means. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))
- The evidence does not provide shield, healing, or damage-scaling-stat mechanics; none are claimed here. ([Game8](https://game8.co/games/Wuthering-Waves/archives/455405))

### Jiyan

- The fetched evidence does not provide exact Resolve gains from Lone Lance or Tactical Strike. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- The rate and timing details of gradual Resolve loss after 15 seconds without a hit are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- The source mentions aerial variants named Mid-Air Strike and Wind Sweep in the Banner of Triumph condition, but does not provide separate descriptions or damage-table rows for those named variants. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- No separate damage value is provided for Emerald Storm: Prelude itself; the available table only gives Emerald Storm: Finale damage. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- The source does not provide a standalone Resonance Liberation table for Prelude distinct from the Qingloong Mode table. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- The evidence does not specify whether the listed percentages use a particular level-scaling convention beyond the source's Skill Lv.1 labels. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- No shield, healing, switch-out, or explicit off-field restriction mechanics are stated in the fetched evidence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))
- Game8's Normal Attack prose mislabeled Abyssal Slash / Banner of Triumph; corrected trigger wording uses Prydwen. Numeric Lv.1 rows remain from Game8. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454216))

### Lingyang

- The fetched evidence does not provide a separate damage table for Radiant Plunge, despite stating that it becomes available after Stormy Kicks. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))
- The fetched evidence names Swift Punches but does not provide a separate Swift Punches damage or effect table; the listed table is labeled Furious Punches. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))
- The Resonance Liberation prose contains the malformed duration “50%s,” conflicting with the Skill Detail table's 14-second Lion's Vigor duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))
- The exact numeric Lion's Spirit restoration amounts from Furious Punches, Lion Awakens, and Strive: Lion's Vigor are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))
- The exact Lion's Spirit consumption rate is not provided; only the 50% reduction during Lion's Vigor and the resulting duration limits are stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))
- The target count, range, and detailed hit behavior for several attacks are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))
- The source lists attribute-bonus rows without clearly mapping each duplicated row to a specific node or skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454223))

### Lucilla

- The fetched evidence does not explicitly state the scaling stat for any damage percentage. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))
- The source states that Clear As Day holds up to 0 Resonance Energy; this may be a source or formatting error, but no alternative value is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))
- The source provides no separate quantitative table for Inherent Skill 1, Inherent Skill 2, Forte Circuit sub-effects, Outro Skill, Tune Break, or Resonance Chain nodes; listed values for those entries are taken directly from their prose where available. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))
- The exact target range for Focus Ring, Spotlight's Glacio RES reduction, Montage, and other area effects is not quantified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))
- The source does not define the duration or exact removal conditions for Reminiscence beyond Letting It Go ending it and the stated mode-specific effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))
- The source does not provide separate damage values for Compensate, Spotlight, Oblivion, or the Reminiscence replacement attacks beyond the tables reproduced above; Oblivion has no damage row in the supplied evidence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))
- The source does not explain how Resonance Mode is entered or switched, only the effects associated with Glacio Chafe and Echo modes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568207))

### Lucy

- The fetched evidence does not provide skill-level scaling beyond the displayed Skill Detail/Efffect (Lvl 1) values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598702))
- The source contains inconsistent Spoofing Program naming: Cyberwave Malfunction in Resonance Liberation versus Cyberware Malfunction in S1/S2, and Cyberpsychosis versus Psychosis in S2. The reference preserves both forms where relevant. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598702))
- The source states SQL increases Multi-threading's DMG Multiplier by 270% but does not specify whether this is additive, multiplicative, or a final multiplier treatment. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598702))
- No separate skill-detail tables are supplied for Inherent Skills, Outro Skill, or Tune Break itself; their unsupported numeric fields are therefore omitted or marked n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598702))
- The source does not provide a numeric damage value for the automatic Override activation condition beyond the listed Override rows. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598702))
- The source's introductory claim supplies Lucy's Spectro element, Pistol weapon type, and 5-star rarity; no further equipment or build information is supported here. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598702))

### Lumi

- The fetched evidence does not provide the numerical amount of Resonance Skill DMG amplification for the Outro Skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473488))
- The fetched evidence does not specify the increased DMG multipliers or extra Spark amounts for Red Spotlight Mode and Yellow Spotlight Mode. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473488))
- The fetched evidence does not specify the exact target behavior or damage classification beyond the stated Basic Attack classifications for Laser, Glitter, Energized Pounce, Energized Rebound, and Red Light Heavy Attack. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473488))
- The source labels the Normal Attack section as Navigation Support; this reference treats it as Lumi's Normal Attack because the Forte text explicitly refers to Normal Attack Navigation Support. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473488))
- No quantitative table is supplied for Inherent Skills, Outro Skill, or Tune Break; unsupported numerical fields are marked n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/473488))

### Lupa

- The fetched evidence does not provide Lupa's acquisition method or voice actor. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))
- Exact Wolflame restoration from ordinary Normal Attacks, Resonance Skills, and Resonance Liberation is not specified; only the explicitly listed restorations are quantified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))
- The exact duration of the Shewolf's Hunt-to-Feral Fang availability window is not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))
- The evidence states that Dance With the Wolf: Climax removes Burning Matchpoint when it ends, but does not specify whether any other Burning Matchpoint effects are altered before that point. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))
- The source presents attribute bonuses within skill sections, but does not clearly identify their unlock conditions or whether the listed percentages are part of the corresponding skill's damage table. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))
- Tune Break has no damage or effect values in the fetched evidence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))
- The source contains a likely typo, 'Pack Hurt,' in Sequence 3; it is interpreted as Pack Hunt because that is the named effect used elsewhere in the supplied text. ([Game8](https://game8.co/games/Wuthering-Waves/archives/520661))

### Luuk Herssen

- No separate numerical Skill Detail table is supplied for Normal Attack's whirling blade, Scythe: Dissection's or Resection's Tune Strain effect beyond the stated duration, or the fixed Ichor Blade's complete damage behavior beyond its per-0.15s value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568210))
- The source identifies the character as a 5-star Spectro Gauntlet Resonator, but the provided Resonator Information table is structurally broken; no additional weapon or base-stat information is available. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568210))
- The source does not provide numerical values for the Tune Break Boost stat itself, Tune Strain stack caps except where explicitly stated, or the exact duration/amount of the 15% Scythe: Resection damage reduction beyond 1s. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568210))
- The phrase 'the next Normal Attack triggers Basic Attack - Golden Impale' does not specify a separate input time limit; only the listed airborne Dodge Counter and switch-out cancellation conditions are supported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568210))

### Lynae

- The fetched evidence does not provide a separate numerical table for every individual sub-action or for the exact Overflow recovery amounts from normal attacks, Lynae-Style Palettes, Mid-air Attack, Dodge Counter, and Intro Skill; only the explicitly tabulated values are reported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- Several timing windows are described as 'within a certain time' without a numeric duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source states that Basic Attack - Visual Impact grants 40 Tune Break Boost for 30s, but does not provide a separate skill-detail table row for this effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source's Tune Strain wording is ambiguous about whether the 0.12% increase is applied per stack, per Tune Break Boost point, or both; it is preserved as written. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source lists an Intro Skill named Time to Show Some Colors!, while Inherent Skill 2 refers to Taste My Colors!; the evidence does not clarify whether these are alternate names or a source inconsistency. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source does not provide cooldown or energy values for the Intro, Outro, or Tune Break abilities beyond the explicitly listed values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source does not provide a separate exact damage table for the 100% Spectro damage of Let's Hit the Road!. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source does not state the scaling stat for the listed damage values; Tune Rupture Response is explicitly expressed as Tune AMP. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))
- The source contains no separate weapon, acquisition, or voice-actor details beyond the stated Pistol weapon and 5-star Spectro classification. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568211))

### Mornye

- The fetched evidence does not provide explicit level-scaling formulas for many effects beyond the listed Skill Detail tables. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The source contains no separate quantitative table for Tune Break's Tune Strain stacking effect beyond the stated 0.12% per Tune Break Boost point. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The exact duration or numerical damage-reduction value for the Parry state is not stated beyond 100% damage reduction; its duration is therefore n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The target-count, duration, and exact effect details of Optimal Solution's Stagnation are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The source labels Wide Field Observation Mode movement as continuously consuming Stamina and provides a per-second cost, but does not state total Stamina or exact flight speed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The source does not provide a separate Skill Detail table for Proof of Boundedness, Visual Field, Observation Marker, or Interfered Marker; values are reported only where stated in the text. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The phrase 'their DMG' for Interfered Marker is not explicitly scoped beyond nearby team Resonators in the source. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The S1 source contains the apparent typo 'pr' in the condition; it is interpreted as 'or' without changing the stated effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))
- The source does not explicitly identify a separate standalone skill for Syntony Field or High Syntony Field; they are included as additional abilities because their mechanics are present. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568193))

### Mortefi

- The evidence does not state Mortefi's ATK or another scaling stat for the listed damage values; percentages are therefore reproduced without assigning a scaling stat. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454222))
- Exact Annoyance restoration amounts from Impromptu Show, Dissonance, and the post-Passionate Variation Basic Attack effect are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454222))
- The duration of Burning Rhapsody is given as 10 in the Liberation table, but its unit is not explicitly labeled there; the text refers to it as a duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454222))
- The evidence does not specify the exact effect of Tune Break beyond its availability when the target's Off-Tune Level is full. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454222))
- The evidence does not provide a separate skill-detail table for the Inherent Skills, Outro, Tune Break, or most Resonance Chain effects; unsupported level-specific values are not inferred. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454222))
- The source contains the Fury Fugue damage and Energy Regen rows both under the Resonance Skill section and the Forte Circuit section; they are retained in both relevant ability entries rather than treated as separate unsupported values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454222))

### Phoebe

- The source gives no separate detailed skill entry for Basic Attack: Chamuel's Star beyond the Resonance Skill description and its stage multipliers. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source's Forte Circuit table contains malformed percentage values for Absolute Litany DMG and Utter Confession DMG; their exact numerical values are reported as n.a. rather than corrected by inference. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The Resonance Liberation Skill DMG value is likewise malformed as 202.00%% and is reported as n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source uses both 'Absolution Litany' in the mechanics text and 'Absolute Litany' in the table label; the intended naming is ambiguous. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source does not specify the durations of Absolution status, Confession status, Spectro Frazzle, Divine Voice, or Prayer-related states except where durations are explicitly listed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source does not specify the exact trigger timing or duration of the 'shortly after' Resonance Skill teleport window. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source does not define whether the 256% Absolution DMG Amplification applies to the entire skill or a particular hit beyond stating that the skill gains the amplification. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source does not provide an explicit damage formula for most entries beyond the listed multipliers and the Outro's ATK scaling. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))
- The source does not provide a separate cooldown or resource cost for Tune Break. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486244))

### Phrolova

- The fetched evidence gives no explicit numeric values for Reincarnate duration, Resolving Chord duration, Compose cooldown beyond the stated 25s entry interval, Volatile Note ordering behavior beyond the listed rules, or the exact maximum Aftersound value referred to as 'max'. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524877))
- The source does not provide a separate Resonance Liberation cooldown or a conventional Resonance Energy cost; it explicitly states maximum Resonance Energy is 0 and the Liberation consumes no Resonance Energy. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524877))
- The source mentions Hazy Dream but does not define how that state is applied or removed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524877))
- The source labels several tables as Effect (Lvl 1), but some non-damage passive values are stated in prose rather than in a formal table; they are retained as provided and not converted to higher-level values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524877))
- The evidence does not provide a separate standalone damage table for Apparition of Beyond - Hecate beyond its S6 scaling of 216.42% of Phrolova's ATK. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524877))
- The fetched page identifies Phrolova as playable, 5-star, Havoc, and Rectifier, but provides no acquisition details or voice-actor information. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524877))

### Qingxiao

- The evidence does not provide exact damage values for many effects beyond the listed Skill Detail tables, nor exact durations for Ephemeral Transcendence, Heaven's Clarity, Sword Flight, Resonant Chime, Mindlock, or Swordlight Ward beyond the stated 1-second damage-reduction duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605308))
- The evidence mentions Flight Qi but provides no maximum, regeneration, or numeric consumption rate; only S5's 30% reduction is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605308))
- The evidence names Sword Dodge as a Sword Flight entry skill but does not provide a separate Sword Dodge ability description or damage/table row. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605308))
- The exact meaning of 'additional Off-Tune Level' and the amount built by the enhanced Heavy Attack - Heaven's Reckoning are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605308))
- The source labels Resonance Chain effects as S1-S6 and supplies their names/effects, but does not provide separate numerical damage tables for Juque Perdition or World in Chorus. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605308))
- No separate standalone numeric table is supplied for Tune Break, Inherent Skills, Outro Skill, or the extra movement/state mechanics; unsupported values are therefore omitted. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605308))

### Qiuyuan

- The source does not provide the exact Stamina cost for Resonance Skill or Undaunted Wayfarer beyond stating that Stamina is consumed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The source does not provide level-scaling tables beyond the displayed skill Lv.1 values; no Lv.10 values are supported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The exact duration or timing window for the Normal Attack follow-up after Inkwash and Intro Skill is not stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The amount of Swordster's Soliloquy consumed by To Teach, To Save, and To Sacrifice is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The source does not state whether the 30% Bamboo's Shade Echo Skill DMG Bonus is additive or multiplicative with other bonuses. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The source describes S3's 500% and 600% effects as DMG multiplier increases but does not clarify their precise additive or multiplicative calculation method. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The source does not provide a separate skill-detail table for Tune Break. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The source does not state the exact target count or area for several nearby-target effects beyond the wording supplied. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))
- The fetched text contains navigation/table fragments and does not provide additional Resonator information such as acquisition method, base statistics, or voice actor. ([Game8](https://game8.co/games/Wuthering-Waves/archives/524882))

### Rebecca

- No explicit acquisition method, voice actor, or complete character-information table values are provided in the fetched evidence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598700))
- The Heavy Attack - Guts quantitative row is labeled 'Heavy Attack - Guts DMG' but has value 20, conflicting with the earlier 102.00% damage row; both source rows are retained without interpretation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598700))
- The source's Preem Choom entry is under Outro but refers to Lucy and includes Lucy-specific wording; its attribution to Rebecca is unsupported and therefore marked ambiguous. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598700))
- The source does not provide complete level-scaling tables beyond the listed skill Lv.1 values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598700))
- The duration wording for Inherent Skill 1 says '10% for 12' and is interpreted only as the explicitly stated 12-second duration; the unit omitted in the source is not supplied. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598700))
- The source contains a typo 'Havy Attack' in Inherent Skill 1; the corresponding named skill is retained as Heavy Attack - Bang-bang-bang!: Guts. ([Game8](https://game8.co/games/Wuthering-Waves/archives/598700))

### Roccia

- The fetched evidence does not provide Roccia's method of acquisition, voice actor, or a complete resonator-information table beyond rarity, attribute, and weapon. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- No separate numerical table is supplied for Inherent Skills, Outro, Tune Break, or the Resonance Chain effects; their listed quantities are taken directly from the prose. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- The source uses both '10 Concerto Energy' in S1 and 'Concerto Regen' in ability tables; these terms are preserved according to the source and are not reconciled. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- The Normal Attack text states that charging restores Imagination and that Normal Attacks restore Imagination, but gives no exact amount. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- The exact target behavior and damage formula for Magic Box are not specified beyond nearby-target pulling and 100 points of Havoc DMG. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- The exact damage value or formula for Tune Break is not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- The source does not provide a separate full damage table for Basic Attack:Reality Recreation; only its 100% relation to Real Fantasy Stage 3 DMG is given. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))
- The source's formatting does not explicitly label which numeric entries are standard skill-level rows versus attribute-node values; all supplied table values are marked skill Lv.1 without extrapolation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486246))

### Rover Aero

- The fetched evidence identifies Rover Aero as free after completing the Main Quest “The Maiden,” but the quest text is truncated and does not provide further unlock details. ([Game8](https://game8.co/games/Wuthering-Waves/archives/505267))
- No numerical Skill Detail table is provided for the Outro, Tune Break, Inherent Skills, or Resonance Chains; no values were inferred. ([Game8](https://game8.co/games/Wuthering-Waves/archives/505267))
- The source uses percentage expressions such as “27.69%+1.00%\*25” and “11.76%\*3+52.89%” without explaining their component meanings; they are retained verbatim. ([Game8](https://game8.co/games/Wuthering-Waves/archives/505267))
- The source does not explicitly provide cooldown, cost, or resource requirements for Normal Attack variants, Cloudburst Dance, or Unbound Flow beyond the listed Windstrings costs and gains. ([Game8](https://game8.co/games/Wuthering-Waves/archives/505267))
- The source states that Cloudburst Dance heals nearby team Resonators but does not specify whether its healing occurs once per cast or per stage beyond the single table value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/505267))
- The source does not define Aero Erosion's duration, damage, or normal stack limit; it only states the stack-removal/infection interaction and the Aeolian Realm maximum-stack increase. ([Game8](https://game8.co/games/Wuthering-Waves/archives/505267))

### Rover Electro

- The fetched evidence does not provide an explicit damage type or scaling-stat statement for every individual attack; listed damage types and the one explicit healing formula are retained as written. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The Forte Circuit section describes Spectro, Havoc, and Aero Thrum of All Sounds attacks despite the character being identified as Electro; the source does not explain this apparent cross-element behavior, so it is reported without correction. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The exact timing window for the attack that triggers Riposte Strike's neutralization and Stagnation effect is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The source does not define the duration or detailed behavior of Stagnate or Electro Flare. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The source says Electric Surge is restored when listed skills deal damage but does not provide the amount restored. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The source does not specify how much Thunder Rage each damaging Thrum of All Sounds hit restores, beyond stating that it is restored when the skill deals damage. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The source does not specify the exact Basic Attack-stage mapping for Apex Resonance's chained Thrum of All Sounds skills. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- No level-10 values are provided; all quantitative values are skill Lv.1 values from the fetched tables. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The source does not provide quantitative details for the Parry Stance's interruption resistance beyond immunity, its 60% damage reduction, or the successful-Dodge timing of Dodge: Flicker. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))
- The source does not provide a separate skill-detail table for the Outro Skill, Tune Break, Inherent Skills, or Resonance Chain nodes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/606967))

### Rover Havoc

- The evidence states that Havoc Rover is free and unlocked after completing the Main Quest “Grand Warst…” but the quest title is truncated, so the complete unlock requirement cannot be confirmed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))
- No explicit Dark Surge duration or condition for leaving the state is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))
- No explicit switch-out behavior, shield effects, or additional healing beyond Sequence Node 3 is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))
- The evidence does not specify whether the listed attribute bonuses are unlocked at particular Forte levels or nodes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))
- The exact target range and field size for Outro Soundweaver are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))
- Tune Break has no damage, duration, cost, cooldown, or additional effect stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))
- The source labels the Forte entries as Umbra: Basic Attack, Heavy Attack, Plunging Attack, and Dodge Counter but does not separately state every input restriction beyond the listed Dark Surge conversions. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456120))

### Rover Spectro

- The evidence does not state the exact amount of Diminutive Sound gained per Normal Attack hit, Heavy Attack Aftertune hit, or Waveshock cast beyond confirming that each grants it. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The source states that post-2.0 Resonating Spin applies two Spectro Frazzle stacks along with Shimmer, but does not provide Spectro Frazzle's effect or duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The source lists Resonating Whirl damage in the Forte table without explaining its trigger or mechanics. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The precise duration or behavior of Resonating Spin itself is not provided; only that Resonating Echoes can be used after it ends. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The target-area size and exact detonation interval for Echoing Orchestra are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The Outro's stasis effect is described without its gameplay effect beyond the 3s area and its association with the next or nearby Outro-triggering character. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The evidence uses the name Echoing Resonance in Sequence 4, while the listed Resonance Liberation is named Echoing Orchestra; the relationship between these names is not explained. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))
- The source's navigation labels are fragmented, but the listed ability descriptions provide the identifiable Normal Attack, Resonance Skill, Forte Circuit, Inherent Skills, Resonance Liberation, Intro, Outro, and Tune Break entries. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454228))

### Sanhua

- The evidence does not provide the exact Forte Gauge cursor timing, Frostbite-area dimensions, or the number of hits represented by the Forte Circuit Burst Damage row beyond the notation 93.70%\*2. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454225))
- The source labels several Energy-related rows as 'Con.' or 'Con. Damage Regen'; their exact in-game terminology is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454225))
- The source provides no numerical tables for the Inherent Skills, Outro, Tune Break, or Resonance Chain effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454225))
- The source does not provide the exact trigger or duration rules for the S5 automatic explosions beyond stating that the creations explode even when not detonated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454225))
- The source's navigation and table text is partially truncated or malformed, but the listed ability names and effects are retained where readable. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454225))

### Shorekeeper

- The fetched evidence does not provide separate cooldown, duration, or resource-cost values for most Normal Attack and Forte Circuit sub-actions beyond the listed Stamina costs and Concerto regeneration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- The exact duration of Unbound Form and the amount or timing of Deductive Data generated per second are not numerically specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- The source states that Collapsed Cores transform into Flare Star Butterflies but does not provide a maximum number of simultaneously existing Flare Star Butterflies or a full duration for the butterflies. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- The source's Discernment DMG row is presented as '9.88%\*3 HP'; this has been retained verbatim because the scaling notation is ambiguous. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- The source does not provide a numeric healing amount for the Outer Stellarealm's repeated healing separately from the Resonance Liberation healing table row. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- The evidence does not specify whether the 15% DMG amplification from Binary Butterfly applies to all damage types or provide a separate cooldown. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- The sequence effects are duplicated in the source's extra-ability section; they are represented once as the six Resonance Chain nodes and again as named extra-ability entries only to preserve the supplied ability information. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))
- No additional mechanics are provided for Tune Break beyond the full Off-Tune Level requirement. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463667))

### Sigrika

- The evidence provides only skill Lv.1 numerical values; no higher-level values are supported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))
- The source does not specify the exact damage or duration behavior of Stagnate, the exact Rune-slot ordering beyond leftmost removal, or whether all listed damage-multiplier increases are additive or multiplicative. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))
- The source uses the label “Innate Gift?” including a question mark; this has been retained rather than normalized. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))
- The source says Sigrika gains 50 Full Stop after Heavy Attack - Schemata of Runes, but does not state whether this gain is affected by any additional conditions. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))
- The source does not provide separate quantitative tables for Inherent Skills, Outro Skill, Tune Break, or the extra Rune/state rules. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))
- The source does not specify a numerical value for the normal Forte Circuit activation's Full Stop consumption beyond stating that it consumes all Full Stop. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))
- The source does not specify whether the 50% Schemata-of-Runes DMG-multiplier increase and the Soliskin Vitality-based DMG Amplification apply to every component of the resulting Runic effect beyond the listed wording. ([Game8](https://game8.co/games/Wuthering-Waves/archives/568208))

### Suisui

- The evidence does not provide an explicit numerical healing value for Plume Step itself beyond the separate 'Healing per Plume Step' table row. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605302))
- The evidence does not state the exact duration or timing window for performing each Plume Step, Dodge follow-up, or Drizzle Stance Basic Attack cycle preservation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605302))
- The exact scaling/stat classification for most listed DMG percentages is not specified; only Awakening Spring, Enrichment Healing, Spring's Birth healing, Plume Step healing, and the stated HP/energy-based effects identify HP or Energy Regen scaling. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605302))
- The source does not provide a separate numerical table for Inherent Skill 1 or Inherent Skill 2. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605302))
- The attribute-bonus rows are presented under individual source sections, but their exact upgrade-node placement is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605302))
- The phrase 'all nearby Resonators' does not provide an exact range. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605302))

### Taoqi

- The evidence does not provide the exact DEF or HP scaling formulas behind the Fortified Defense HP recovery, Rocksteady Shields, Timed Counter shields, or Unmovable beyond the listed Level 1 table values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454226))
- The evidence does not specify the exact duration or stacking/refresh behavior of Rocksteady Defense. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454226))
- The evidence does not clarify whether Rocksteady Shield's damage reduction applies to Taoqi only or to any on-field character beyond its wording that the character is attacked. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454226))
- The evidence does not provide a separate numerical table for Strategic Parry triggered by Resonance Skill casting versus Heavy Attack. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454226))
- The Tune Break entry gives no damage, duration, cost, cooldown, or additional effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454226))
- The source includes a recommended-sequence section listing S1-S6 but does not provide recommendation rationale; only the separate node descriptions were used here. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454226))

### Verina

- The fetched text does not state the maximum number of Photosynthesis Energy stacks or how those stacks are normally generated, apart from the S2 additional grant. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))
- The scaling-stat basis for percentage portions of the listed healing formulas is not explicitly labeled in the tables; ATK is stated explicitly for several other effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))
- The source gives no separate quantitative table for Inherent Skills, Outro Skill, Tune Break, or the sequence nodes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))
- The numeric unit for Photosynthesis Mark Duration, cooldown, and energy values is presented without an explicit unit in the source; the duration is treated as seconds only where the prose explicitly says seconds. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))
- The source mentions Trees Growth in S4 but provides no definition or standalone ability entry for it. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))
- The Dodge Counter description duplicates the mid-air plunging-attack wording and does not clarify whether it has any additional dodge-counter-specific behavior. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))
- The fetched content truncates the general Resonator Information table, so acquisition method and voice actor are unsupported. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454229))

### Xiangli Yao

- The fetched evidence does not provide explicit ATK/HP/DEF scaling-stat labels for most attacks; only Chain Rule explicitly states scaling from Xiangli Yao's ATK. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461501))
- The exact numerical amount of the interruption-resistance enhancement from Inherent Skill 2 is not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461501))
- The exact mechanics of the Basic Attack Pivot - Impale replacement beyond its three stages are not separately specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461501))
- The source repeats Cogitation Model information under Forte Circuit and Resonance Liberation; it does not clearly separate whether all listed quantitative rows belong exclusively to one section. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461501))
- The source's Resonance Information table is truncated, although the prose identifies Xiangli Yao as a 5-star Electro Gauntlet character. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461501))
- No separate quantitative table is supplied for Inherent Skills, Tune Break, or most Resonance Chain effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461501))

### Yangyang

- The evidence does not state the scaling stat or damage formula for any attack. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The exact target-count, crowd-control duration, and vortex duration for Zephyr Domain and Wind Spirals are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The evidence does not specify how Melody gain behaves when the 3-Melody cap is already reached. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The evidence does not specify whether every listed hit of Zephyr Song or Zephyr Domain can grant Melody independently beyond the wording 'on hit.' ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The exact activation input, timing window, and hit details for Stormy Strike and Feather Release are not fully described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- No cooldown or other restriction is given for Stormy Strike or Feather Release. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The evidence does not specify the duration, stacking behavior, or recipient rules for Whispering Breeze beyond its 5-second recovery period. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The Tune Break effect is only described as being cast when the target's Off-Tune Level is full; its damage, cost, cooldown, and other mechanics are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- The source formatting contains broken or ambiguous navigation/table labels, but the listed ability names and Lv.1 rows have been retained as presented. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))
- No additional quantitative tables are supplied for the Inherent Skills, Outro Skill, Tune Break, or Resonance Chain effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454215))

### Yangyang: Xuanling

- The source does not provide the fixed damage values for the Wraith of Sound attacks. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605297))
- Basic Attack - Havoc in Bloom Stage 3 DMG is blank in the source table and is recorded as n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605297))
- The Forte text says Streaming Storm lasts 15s but later refers to Drifting Mist in the once-per-25s sentence; the intended name of that cooldown-limited effect is ambiguous. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605297))
- The source does not specify the exact fixed damage or duration of the Wraith of Sound, Feather Release: Xuanling, or some Shadow of Xuanling variants beyond the values explicitly listed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605297))
- The source does not provide numeric Skill Detail tables for the Inherent Skills, Outro, Tune Break, or Resonance Chain effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/605297))

### Yinlin

- The evidence does not provide numerical Judgment Point gains from Normal Attack, Magnetic Roar, or Electromagnetic Blast; it only states that these actions restore Judgment Points. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454218))
- The duration or timing window for activating Lightning Execution after Magnetic Roar is not numerically specified; the evidence only states that it enters cooldown if not activated in time or if Yinlin is switched out. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454218))
- The source states that Sinner's Mark is removed when Yinlin exits, but does not explicitly clarify whether this refers to exiting the field or another form of exit. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454218))
- The source includes attribute-bonus rows but does not identify their exact unlock nodes or progression requirements. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454218))
- The evidence does not provide numerical scaling for the Resonance Skill, Forte Circuit, or other effects beyond the listed skill Lv.1 tables. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454218))

### Youhu

- All listed damage, healing, and Antique Appraisal multipliers are missing from the fetched evidence and are reported as n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))
- The Normal Attack table contains blank Lv.1 values for all listed damage rows. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))
- The Resonance Skill table is structurally broken in the fetched evidence; the individual Concerto Regen rows are reconstructed from the visible labels, while their displayed values are treated as 10 based on the adjacent source entries. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))
- The source does not specify the numerical amount or regeneration rate of Frost, the Fortune Rolling duration or behavior beyond restoring Frost over time, the specified response time for Fortune’s Favor, or the exact Vibration Strength, stance-break, pull, and healing magnitudes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))
- The source does not provide a separate numerical table for Lucky Draw or Antique Appraisal beyond the incomplete Resonance Skill table. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))
- The source states that Poetic Essence restores HP but does not provide its healing amount; Double Pun Bonus Healing is also numerically unavailable. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))
- The source does not specify whether the listed attribute bonuses belong to particular advancement nodes beyond their placement in the respective skill sections. ([Game8](https://game8.co/games/Wuthering-Waves/archives/463668))

### Yuanwu

- The evidence does not provide exact base durations or trigger details for the Basic Attack, Heavy Attack, Mid-air Attack, or Dodge Counter beyond the listed descriptions and table values. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454219))
- The evidence states that Lightning Infused greatly increases anti-interruption but does not provide a numerical value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454219))
- The evidence does not provide a numerical value for the Thunder Uprising Vibration Strength-depletion enhancement from Inherent Skill 1. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454219))
- The evidence does not provide a numerical shield value beyond the S4 formula of 200% of Yuanwu's DEF. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454219))
- The source's character-information table is truncated, but the fetched text explicitly identifies Yuanwu as Electro, Gauntlets, and 4-star. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454219))

### Zani

- The evidence does not provide exact Redundant Energy gained from Normal Attack hits or the listed skill casts, nor the exact Blaze recovered by the final stage of Targeted Action or Forcible Riposte. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- The source uses both “Heavy Slash - Lightsmash” and the apparent typo “Heavy Slash - Lighstmash”; they are treated as the same named attack. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- The detailed formulas for several attacks are presented as additive percentage strings without explaining hit segmentation or multiplier interpretation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- The source does not specify a numerical Redundant Energy cost for Crisis Response Protocol beyond consuming all available energy. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- The source does not specify the exact duration of Standard Defense Protocol, Crisis Response Protocol, or Scorching Light Ready Stances. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- No healing or shield effect is stated in the supplied evidence; the defensive effects are damage reduction, damage negation for the triggering hit, interruption immunity, and Stagnation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- The source mentions Inferno Mode increasing the Basic Attack DMG multiplier and lists a 25% increase, but does not clarify whether the value applies to every Basic Attack variant. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- The target scope of some Stagnation and Vibration Strength effects is described as the target or nearby targets, but the evidence does not provide ranges or durations for those effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))
- No separate skill-detail table is supplied for Tune Break. ([Game8](https://game8.co/games/Wuthering-Waves/archives/486248))

### Zhezhi

- The fetched evidence does not provide the exact amount of Afflatus gained by Normal Attacks or the Intro Skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461497))
- The evidence states that Creation's Zenith deals greater Glacio DMG than Stroke of Genius but does not provide a separate comparative base value beyond its listed 60.00%\*3 Lv.1 table entry. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461497))
- The evidence does not provide a numerical damage value for the 18% Basic Attack DMG Bonus beyond the stated percentage and duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461497))
- Tune Break has no damage, cost, cooldown, or regeneration values in the fetched evidence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461497))
- No separate skill table is supplied for Calligrapher's Touch, Flourish, or Carve and Draw; their listed numerical values are taken directly from the effect text where available. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461497))
- The source's Resonance Chain heading includes a recommendation section, but only the six explicit S1-S6 node descriptions were used. ([Game8](https://game8.co/games/Wuthering-Waves/archives/461497))

## Echo evidence still requiring care

### Abyssal Gladius

- No exact duration is given for the held Echo form. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492503))
- No hit counts or movement details are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492503))
- No separate main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492503))
### Abyssal Mercator

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492504))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492504))
- Additional scaling types or triggers: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492504))
### Abyssal Patricius

- No holding behavior, hit count, or additional scaling details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492502))
### Aero Drake

- No hit count, movement behavior, holding behavior, or damage-scaling stat is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506678))
- No main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506678))
### Aero Predator

- Skill duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454291))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454291))
- Additional trigger details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454291))
### Aero Prism

- The source does not specify hit count, movement behavior, holding behavior, or whether the effect is an active skill versus a main-slot passive. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499524))
### Aureate Picket

- No additional skill levels or rarity values are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607288))
- No trigger details beyond Echo Skill activation, no hit count, no duration, no movement details, and no holding behavior are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607288))
### Autopuppet Scout

- No skill duration, hit count, movement behavior, or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454278))
- No main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454278))
### Baby Viridblaze Saurian

- HP restoration amount/scaling is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454293))
- Transformation duration is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454293))
- Damage coefficients, damage type, and hit count are not applicable or not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454293))
- No active-versus-main-slot passive distinction is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454293))
### Bell-Borne Geochelone

- No movement behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454269))
- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454269))
- No separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454269))
### Calamity Effigy

- No movement behavior or hold-input behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/616376))
- No hit count is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/616376))
- No additional damage-scaling details are provided beyond the 405.00% Aero DMG coefficient. ([Game8](https://game8.co/games/Wuthering-Waves/archives/616376))
### Calcified Junrock

- The source does not specify the interval or trigger condition for the up-to-5 healing instances. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499525))
- No damage, movement, holding, or main-slot passive details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499525))
### Capitaneus

- No holding behavior is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506667))
- No additional movement behavior is described beyond the jump-up attack. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506667))
- No separate scaling stat is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506667))
### Carapace

- No movement details provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454279))
- No holding behavior provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454279))
- No passive effect provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454279))
- No additional scaling details provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454279))
### Chasm Guardian

- The HP-recovery tick interval and exact number of ticks are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454280))
- No additional movement details beyond the leap strike are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454280))
- No holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454280))
### Chest Mimic

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492519))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492519))
- Additional triggers, duration, scaling details, and passive effects: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492519))
### Chirpuff

- No holding behavior or alternate input details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454294))
- No separate main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454294))
### Chop Chop

- No movement behavior or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492506))
- No main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492506))
- No additional scaling type beyond the listed Fusion DMG coefficients is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492506))
### Chop Chop: Headless

- No separate passive/main-slot effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492511))
- No movement or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492511))
- No hit count or additional scaling details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492511))
### Chop Chop: Leftless

- No additional skill details, scaling information, hit count, duration, movement behavior, or holding behavior are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492512))
### Chop Chop: Rightless

- No movement behavior, hold behavior, hit count, duration, or main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492513))
### Clang Bang

- No detailed timing or duration for the summoned Clang Bang is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459485))
- No explicit scaling-stat description beyond Glacio DMG and the listed 32.00% + 64 value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459485))
- No hit count, holding behavior, or separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459485))
### Corrosaurus

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/corrosaurus))
- No hold mechanic or additional passive requirement is stated. ([Wuthering.gg](https://wuthering.gg/echos/corrosaurus))
### Crownless

- No movement behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454270))
- No holding or charge behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454270))
- No additional scaling details are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454270))
- The page does not explicitly label the post-transformation bonuses as a main-slot passive, though they apply to the current character after transformation. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454270))
### Cruisewing

- No additional damage, trigger, duration, movement, holding, or main-slot passive details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454295))
### Cuddle Wuddle

- No movement behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492507))
- No holding or charge behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492507))
- No separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492507))
### Cyan-Feathered Heron

- Hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454281))
- Skill duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454281))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454281))
- Additional movement details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454281))
### Devotee's Flesh

- No movement or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526506))
- No separate main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526506))
- No additional damage-scaling type beyond Aero DMG is stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526506))
### Diamondclaw

- Hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454296))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454296))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454296))
- Parry State duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454296))
### Diggy Duggy

- No detailed scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492518))
- No hit count, hold behavior, or separate passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492518))
### Diurnus Knight

- Scaling stat/type beyond the stated 268.20% Spectro DMG is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492500))
- Hit count, holding behavior, transformation duration, and duration of the Spectro Frazzle damage increase are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492500))
### Dragon of Dirge

- No movement, holding, interruption, or additional scaling details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492490))
- The periodic hit interval and total number of hits are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492490))
### Dreamless

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/dreamless))
- No hold mechanic is specified. ([Wuthering.gg](https://wuthering.gg/echos/dreamless))
- No additional passive requirement is specified beyond the stated Resonance Liberation trigger. ([Wuthering.gg](https://wuthering.gg/echos/dreamless))
### Dwarf Cassowary

- No additional triggers or durations are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459486))
- No detailed movement behavior beyond tracking the enemy is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459486))
### Electro Drake

- No movement or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506676))
- No main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506676))
### Electro Predator

- No movement or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454297))
- No main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454297))
### Excarat

- No damage coefficients, damage/scaling types, hit count, duration, or holding mechanics are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454298))
- No separate passive effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454298))
### Fae Ignis

- No additional skill scaling, hit count, movement behavior, holding behavior, or main-slot passive details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492514))
### Fallacy of No Return

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/fallacy-of-no-return))
- No separate passive requirement is stated. ([Wuthering.gg](https://wuthering.gg/echos/fallacy-of-no-return))
- The duration of the 10% Energy Regen bonus is not separately specified; the text gives 20s after both buffs are described. ([Wuthering.gg](https://wuthering.gg/echos/fallacy-of-no-return))
- No rarity value is provided beyond the explicit Overlord class and Rank 5. ([Wuthering.gg](https://wuthering.gg/echos/fallacy-of-no-return))
### Feilian Beringal

- Movement behavior and holding behavior are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454266))
- No additional skill scaling or damage details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454266))
### Fission Junrock

- No damage, damage type, or scaling information is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454299))
- No hit count, effect duration, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454299))
- The source does not specify the exact trigger or interval represented by “each time” for the healing effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454299))
### Flautist

- No movement or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454282))
- No separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454282))
### Flora Drone

- No detailed hit count, movement behavior, holding behavior, skill duration, or main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571392))
### Flora Reindeer

- No detailed movement, holding, hit-count, scaling, or main-slot passive information is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571376))
### Fog Lionarch

- No additional scaling stat or formula is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607313))
- No duration, trigger condition, movement behavior, or hold behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607313))
- No separate passive effect is listed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607313))
### Fog Lionarch: Body

- No detailed information on hit count, summon duration, holding behavior, or main-slot passive effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607300))
### Fog Lionarch: Head

- No additional damage or scaling type is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607301))
- No hit count, duration, holding behavior, or main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607301))
### Forbidden Bastion

- No holding behavior or alternate held effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607314))
- No hit count, movement details, or additional active-skill triggers are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607314))
- No scaling details beyond 237.60% Glacio DMG are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607314))
### Frostbite Coleoid

- No movement or holding behavior is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571370))
- No hit count is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571370))
- No damage scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571370))
- No separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571370))
### Frostscourge Stalker

- No separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492510))
- No additional triggers, duration, scaling details, hit count, movement behavior, or holding behavior are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492510))
### Fusion Drake

- The overview labels the damage as Fusion DMG, while the detailed skill text specifies Havoc DMG; the page does not resolve this discrepancy. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526505))
- No separate passive, movement, or holding mechanics are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526505))
### Fusion Dreadmane

- The source does not specify a trigger beyond activation of the Echo skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454300))
- No movement, holding, duration, or detailed hit-count behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454300))
### Fusion Prism

- No movement or holding behavior is stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454301))
- No summon or effect duration is stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454301))
- No additional hit count, trigger condition beyond summoning, or scaling-stat details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454301))
### Fusion Warrior

- No damage numbers or scaling attributes are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454302))
- No hit count, duration, movement details, or holding behavior are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454302))
- No distinct active/main-slot passive breakdown is provided beyond the active counterattack effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454302))
### Galescourge Stalker

- No active duration is specified for the summon or healing effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492508))
- No damage or damage-scaling information is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492508))
- No movement or holding behavior is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492508))
- No separate main-slot passive is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492508))
### Geospider S4

- No movement behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571390))
- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571390))
- No skill duration beyond the two listed hits is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571390))
- No separate passive, trigger condition, or scaling details are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571390))
### Glacio Drake

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506675))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506675))
- Additional scaling details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506675))
### Glacio Dreadmane

- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459483))
- Exact number of consecutive attacks/hits: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459483))
- Additional movement behavior beyond mid-air casting and landing: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459483))
### Glacio Predator

- Skill activation trigger is not explicitly detailed beyond the summon action. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454303))
- Charging duration, movement behavior during charging, and total skill duration are n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454303))
- No separate passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454303))
### Glacio Prism

- Summon duration is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454304))
- Movement and holding behavior are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454304))
- No separate main-slot passive effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454304))
### Glommoth

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/glommoth))
- Rarity: n.a. ([Wuthering.gg](https://wuthering.gg/echos/glommoth))
### Golden Junrock

- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499526))
- Separate main-slot passive effect: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499526))
- Additional triggers, durations, scaling details, and hit-count information: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499526))
### Gulpuff

- No additional damage-scaling details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454305))
- No movement or holding behavior is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454305))
- No separate passive or main-slot effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454305))
### Havoc Drake

- Skill duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526504))
- Additional trigger conditions, scaling details, and other effects: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526504))
### Havoc Dreadmane

- Skill duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454283))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454283))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454283))
### Havoc Prism

- No duration, movement, holding, or main-slot passive details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454306))
### Havoc Warrior

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454307))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454307))
- Additional trigger conditions: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454307))
- Separate passive effects: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454307))
### Hecate

- Summon duration is not numerically stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492488))
- No movement behavior or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492488))
- No separate hit count for the Servants’ attacks is given. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492488))
- No damage-scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492488))
### Hoartoise

- HP restoration amount and scaling type are not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454308))
- Transformation duration is not provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454308))
- No damage coefficients or damage types are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454308))
- No hit count, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454308))
- No separate main-slot passive effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454308))
### Hocus Pocus

- No movement or repositioning behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492516))
- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492516))
- No main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492516))
### Hoochief

- No detailed hit count, movement behavior, holding behavior, scaling attribute, or main-slot passive is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454284))
### Hooscamp

- No explicit hit count. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454309))
- No additional scaling-stat description. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454309))
- No holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454309))
- No separate passive or main-slot effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454309))
### Hurriclaw

- No separate main-slot passive, scaling details beyond the listed Aero DMG coefficients, or additional timing values are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499523))
### Hyvatia

- No damage-scaling stat or formula is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571354))
- No movement, targeting, or hold behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571354))
- No separate main-slot passive is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571354))
### Iceglint Dancer

- No damage-scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578129))
- No duration, hit count, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578129))
- No separate main-slot passive effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578129))
### Impermanence Heron

- Continuous flame attack duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454271))
- Continuous flame attack hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454271))
- Initial slam hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454271))
### Inferno Rider

- Riding Mode duration and detailed movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454272))
- Exact trigger/control for exiting Riding Mode: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454272))
- Separate main-slot passive restriction: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454272))
### Ironhoof

- No holding behavior or hold-duration details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571374))
- No separate main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571374))
- No additional damage-scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571374))
### Jué

- No holding behavior or hold-specific mechanics are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/458463))
- No separate main-slot passive effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/458463))
### Kerasaur

- No hold-input behavior or hold duration is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526507))
- No separate active-effect duration is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526507))
### Kernel Puppet: Anger

- No damage scaling stat is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607295))
- No hit count, duration, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607295))
- No passive or main-slot effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607295))
### Kernel Puppet: Fright

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607299))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607299))
- Duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607299))
- Additional hit-count or scaling details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607299))
### Kernel Puppet: Grief

- No duration specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607298))
- No hit count specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607298))
- No movement or holding behavior specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607298))
- No main-slot passive effect specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607298))
- No additional scaling type specified beyond Spectro DMG. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607298))
### Kernel Puppet: Joy

- No detailed attack sequence, hit count, movement behavior, holding behavior, or scaling information is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607294))
### Kernel Puppet: Reflection

- No additional scaling type, hit count, duration, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607297))
### Kernel Puppet: Worry

- No additional scaling type, attack duration, hit count, movement behavior, holding behavior, or main-slot passive is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607296))
### Kronablight

- No detailed information is provided for hit count, scaling stat, transformation duration, hold input, or passive effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578131))
### La Guardia

- The duration of the held transformation is not numerically specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506679))
- No additional movement details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506679))
### Lady of the Sea

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/lady-of-the-sea))
- Trigger condition, hold behavior, and passive requirements are n.a. ([Wuthering.gg](https://wuthering.gg/echos/lady-of-the-sea))
### Lampylumen Myriad

- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454273))
- No additional movement behavior is specified beyond consecutive forward strikes. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454273))
- The source does not separately label the Glacio DMG/Resonance Skill DMG increase as an active or main-slot passive effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454273))
### Lava Larva

- The activation trigger is not separately detailed beyond summoning the Lava Larva. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459487))
- No total duration, attack interval, range, hit count, or additional movement/holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459487))
### Lightcrusher

- No duration is provided for the Lightcrusher form or Ablucence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459484))
- No exact distance, travel time, or momentum duration is provided for the held movement. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459484))
- No additional hit-count details are provided beyond generating 6 Ablucence and each Ablucence explosion dealing damage. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459484))
- No main-slot passive effect is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459484))
### Lioness of Glory

- No exact duration is given for the active animation or its short delay. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526509))
- No holding behavior, charge mechanic, or additional movement details are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526509))
- No separate duration is given for the main-slot passive bonuses. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526509))
### Lorelei

- The source does not specify hit count, movement behavior, holding behavior, or active transformation duration. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492491))
### Lottie Lost

- No additional scaling type, hit-count details, movement behavior, holding behavior, or main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492517))
### Lumiscale Construct

- Parry Stance duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459482))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459482))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459482))
- Hit count: n.a.; the page describes a slash or counterattack but does not state a numerical hit count. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459482))
- Damage scaling basis beyond Glacio DMG: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459482))
- Separate active versus main-slot passive details: no passive is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/459482))
### Mech Abomination

- Exact Mech Waste explosion timing: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454274))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454274))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454274))
- Detailed hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454274))
### Mining Drone

- No separate active/main-slot passive breakdown is provided beyond the transformation attack. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571391))
- No trigger, movement, holding, or duration details are stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571391))
### Mining Reindeer

- No detailed information on movement, holding, targeting behavior, hit count, or passive effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571375))
### Mourning Aix

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454275))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454275))
- Scaling/stat basis beyond the listed damage types and percentages: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454275))
- The source overview mentions continuous attacks, but the detailed skill specifies 2 consecutive claw attacks. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454275))
### Myriad Snare: Rustfire Chassis

- Active-effect duration: n.a.; the source refers to “during this duration” but gives no duration value. ([Game8](https://game8.co/games/Wuthering-Waves/archives/610348))
- Holding behavior: n.a.; no hold input or alternate behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/610348))
- No additional damage type, trigger condition, or scaling information is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/610348))
### Nameless Explorer

- No damage-scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578133))
- No hit count, holding behavior, or additional movement behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578133))
### Nightmare: Aero Predator

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-aero-predator))
### Nightmare: Baby Roseshroom

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-baby-roseshroom))
- No hold mechanic or passive requirement is stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-baby-roseshroom))
### Nightmare: Baby Viridblaze Saurian

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-baby-viridblaze-saurian))
- Healing amount/rate and restoration duration are not specified. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-baby-viridblaze-saurian))
- No hold mechanic, additional trigger, or passive requirement is specified. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-baby-viridblaze-saurian))
### Nightmare: Chirpuff

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-chirpuff))
- Hold mechanic: n.a. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-chirpuff))
- Additional passive requirements: n.a. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-chirpuff))
### Nightmare: Crownless

- The source does not provide hit-count, movement, or holding/hold-input details. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492496))
### Nightmare: Cyan-Feathered Heron

- Supplementary cooldown: n.a. (not stated) ([Wuthering.gg](https://wuthering.gg/echos/nightmare-cyan-feathered-heron))
- No cooldown stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-cyan-feathered-heron))
- No duration, hold requirement, or additional passive requirement stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-cyan-feathered-heron))
### Nightmare: Dwarf Cassowary

- No scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564921))
- No separate main-slot passive is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564921))
- No hold behavior or effect duration is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564921))
### Nightmare: Electro Predator

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-electro-predator))
- No hold mechanic or passive activation requirement is stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-electro-predator))
### Nightmare: Feilian Beringal

- No movement behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492492))
- No holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492492))
- No explicit scaling stat is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492492))
- No exact duration is provided for the Whirlwind Beam. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492492))
### Nightmare: Glacio Predator

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-glacio-predator))
### Nightmare: Gulpuff

- Supplementary cooldown: 8s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-gulpuff))
- No additional trigger, hold behavior, or passive requirement is stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-gulpuff))
### Nightmare: Havoc Warrior

- Supplementary cooldown: 15s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-havoc-warrior))
- No explicit activation trigger beyond using the Echo skill. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-havoc-warrior))
- No duration is specified for the transformation. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-havoc-warrior))
- No additional passive requirement, hold condition, or buff is specified. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-havoc-warrior))
### Nightmare: Hecate

- Supplementary cooldown: 25s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-hecate))
- Duration of the granted buffs: n.a. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-hecate))
### Nightmare: Impermanence Heron

- No movement or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492493))
- No active transformation duration is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492493))
### Nightmare: Inferno Rider

- No duration is specified for Riding Mode or the main-slot bonuses. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492497))
- No detailed movement behavior during Riding Mode is specified beyond entering riding mode by holding Echo Skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492497))
- No hit count or additional scaling-stat information is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492497))
### Nightmare: Kelpie

- No movement or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526510))
- No hit count or effect duration is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526510))
### Nightmare: Lampylumen Myriad

- No hit count is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506683))
- No movement behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506683))
- No holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506683))
- No transformation or passive duration is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506683))
- No damage-scaling stat is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506683))
### Nightmare: Mourning Aix

- Active-skill duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492498))
- Hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492498))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492498))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492498))
### Nightmare: Roseshroom

- Damage scaling stat: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564919))
- Activation trigger details: n.a.; the source only states that the Echo summons Roseshroom. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564919))
- Duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564919))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564919))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564919))
- Whether the laser can hit exactly three times or how hits are timed: only “up to 3 times” is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/564919))
### Nightmare: Tambourinist

- Supplementary cooldown: 15s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-tambourinist))
- No rank-scaling values are provided beyond the displayed Rank 5 coefficient. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-tambourinist))
- No additional passive requirement or summon duration is stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-tambourinist))
### Nightmare: Tempest Mephis

- No additional skill details, such as scaling beyond the listed percentage, hit count, movement behavior, or hold behavior, are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492495))
### Nightmare: Thundering Mephis

- No additional skill details, including hit count, movement behavior, or holding behavior, are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492494))
### Nightmare: Tick Tack

- No holding behavior is specified. ([Game8](https://game8.co/games/1300/archives/564920))
- No explicit movement details beyond charging toward the enemy are provided. ([Game8](https://game8.co/games/1300/archives/564920))
- No ATK-scaling formula or other scaling details are provided. ([Game8](https://game8.co/games/1300/archives/564920))
- No separate main-slot passive effect is provided. ([Game8](https://game8.co/games/1300/archives/564920))
### Nightmare: Violet-Feathered Heron

- Supplementary cooldown: 15s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-violet-feathered-heron))
- Parry Stance duration is not specified. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-violet-feathered-heron))
- No hold input or other passive requirements are specified. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-violet-feathered-heron))
### Nightmare: Viridblaze Saurian

- Supplementary cooldown: 15s ([Wuthering.gg](https://wuthering.gg/echos/nightmare-viridblaze-saurian))
- No hold mechanic, passive requirement, summon duration, damage interval, or additional trigger is stated. ([Wuthering.gg](https://wuthering.gg/echos/nightmare-viridblaze-saurian))
### Nimbus Wraith

- No detailed trigger conditions, movement behavior, holding behavior, or main-slot passive effect are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492515))
### Nocturnus Knight

- Hit count, movement distance, holding behavior, and additional scaling details are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492501))
### Pilgrim's Shell

- No movement or holding behavior is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526508))
- No hit count or attack sequence details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526508))
- No separate main-slot passive effect is listed. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526508))
### Porcelain Picket

- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607304))
- No skill duration, additional movement details, or scaling attribute beyond the listed Aero DMG coefficients is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607304))
### Questless Knight

- No additional skill details, hit count, movement behavior, or holding behavior are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492499))
### Rage Against the Statue

- No hit count, effect duration, or main-slot passive details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/499522))
### Reactor Husk

- No holding behavior or alternate input is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571363))
- No explicit hit count, duration beyond the listed cooldown, or additional scaling details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571363))
### Reminiscence - Kronaclaw

- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578132))
- Activation trigger details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578132))
- Main-slot passive details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578132))
### Reminiscence: Denia

- Scaling type beyond the stated Fusion DMG percentage: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597652))
- Hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597652))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597652))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597652))
- Separate main-slot passive designation: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597652))
### Reminiscence: Fenrico

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/reminiscence-fenrico))
- No additional trigger, duration, or hold condition is stated for the Echo's buffs. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence-fenrico))
### Reminiscence: Fleurdelys

- The source does not provide movement or holding behavior details. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506685))
### Reminiscence: Nightmare Adam Smasher

- Supplementary cooldown: 20s explicitly stated for the Echo Skill; no separate cooldown is given for Lucy's special variants. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence---nightmare-adam-smasher))
- The duration and magnitude of Lucy's movement-speed increase and nearby-enemy slow are not provided. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence---nightmare-adam-smasher))
- No separate cooldown is specified for Lucy's tap or hold variants. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence---nightmare-adam-smasher))
- The exact trigger scope of the 20s cooldown is not further clarified in the source. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence---nightmare-adam-smasher))
### Reminiscence: Threnodian - Leviathan

- Supplementary cooldown: No explicit cooldown stated; Core of Collapse can trigger once every 0.5s while active. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence-threnodian---leviathan))
- The maximum number of Core of Collapse triggers is not provided; the text ends at “up to”. ([Wuthering.gg](https://wuthering.gg/echos/reminiscence-threnodian---leviathan))
### Reminiscence: Threnodian - Voidborne Construct

- No movement or holding behavior is described. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597651))
- No active-effect duration is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597651))
- No activation trigger beyond summoning the Creation is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597651))
- No damage scaling stat is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597651))
### Rocksteady Guardian

- Parry State duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454267))
- Exact activation behavior beyond transformation: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454267))
- Additional movement or hold controls: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454267))
### Roseshroom

- The source does not specify movement behavior, holding behavior, or a main-slot passive effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454285))
### Sabercat Prowler

- The page's overview says Fusion DMG and mentions a Sabercat Reaver, while the detailed skill section states Havoc DMG and a Sabercat Prowler; the detailed skill entry is used here. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571371))
- No additional trigger conditions, duration, hit count, movement behavior, or hold behavior are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571371))
### Sabercat Reaver

- The fetched page does not provide detailed information on hit count, movement, holding behavior, scaling beyond the 192.6% Fusion DMG coefficient, or active-versus-main-slot passive distinctions. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571372))
### Sabyr Boar

- The source does not specify hit count, movement behavior, holding behavior, or any main-slot passive effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454310))
### Sacerdos

- Activation trigger details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506680))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506680))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506680))
- Additional scaling details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506680))
### Sagittario

- No holding behavior or hold duration is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506682))
- The exact movement distance is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506682))
- No additional active duration is specified beyond the movement/action description. ([Game8](https://game8.co/games/Wuthering-Waves/archives/506682))
### Sentry Construct

- The source does not specify the Strike Capacitor’s maximum charge count or charging increments. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492489))
- No hit count, scaling-stat information, holding behavior, transformation duration, or freeze duration is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492489))
### Shadow Stepper

- No skill duration is stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578128))
- No hit count, movement behavior, or holding behavior is stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578128))
- No damage-scaling stat or active-versus-main-slot passive details are stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578128))
### Sigillum

- No trigger conditions beyond summoning are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578106))
- No duration, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578106))
- Scaling details beyond the listed Fusion DMG percentages are not stated. ([Game8](https://game8.co/games/Wuthering-Waves/archives/578106))
### Smiter

- No movement or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607303))
- No main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607303))
- No additional scaling information beyond Spectro DMG coefficients is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607303))
### Smolder

- The source does not specify the number of fireballs or hits. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607302))
- The source does not provide a separate damage-scaling stat, effect duration, movement behavior, or holding behavior. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607302))
### Snip Snap

- No skill duration is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454311))
- No exact fireball or hit count is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454311))
- No movement or holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454311))
- No separate main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454311))
### Spacetrek Explorer

- No damage coefficients or damage/scaling types are provided because the described effect deals no stated damage. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571373))
- No hit count, movement behavior, holding behavior, or active-versus-main-slot passive classification is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571373))
### Spearback

- No additional trigger conditions, scaling details, movement behavior, holding behavior, or passive effects are specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454286))
### Spectro Drake

- The overview describes Spectro DMG, while the detailed skill text specifies Havoc DMG; no resolution is provided by the source. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526503))
- No movement behavior, holding behavior, or main-slot passive effect is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/526503))
### Spectro Prism

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454312))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454312))
- Additional scaling details: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454312))
### Stone Picket

- No detailed information is provided for hit count, duration, movement, holding behavior, or main-slot passive effects. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607305))
- Damage scaling details beyond the Aero DMG coefficient are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/607305))
### Stonewall Bracer

- The source does not specify an exact charge distance, movement speed, or whether the charge can be redirected. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454287))
- The source does not provide a separate trigger condition beyond the skill activation and hit sequence. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454287))
- The source does not state a shield duration or absorption limit. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454287))
- No separate active-versus-main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454287))
### Tambourinist

- Effect duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454288))
- Periodic emission interval: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454288))
- Damage scaling basis: n.a.; only the 14.40% additional Havoc DMG value is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454288))
- Separate active versus main-slot passive details: n.a. beyond the summon-based Echo skill. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454288))
- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454288))
- Hold behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454288))
### Tempest Mephis

- Movement behavior and holding behavior are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454276))
- Exact tail-swing hit count and transformation duration are not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454276))
### The False Sovereign

- Supplementary cooldown: 8s; starts with 2 charges and gains 1 charge every 8s, up to 2 charges. ([Wuthering.gg](https://wuthering.gg/echos/the-false-sovereign))
- No separate duration is specified for the transformation or the main-slot damage bonuses. ([Wuthering.gg](https://wuthering.gg/echos/the-false-sovereign))
- No additional hold requirement or duration is stated. ([Wuthering.gg](https://wuthering.gg/echos/the-false-sovereign))
### Thousand-Puppet Pavilion

- Supplementary cooldown: 20s ([Wuthering.gg](https://wuthering.gg/echos/thousand-puppet-pavilion))
- No hold mechanic or hold-specific value is stated; n.a. ([Wuthering.gg](https://wuthering.gg/echos/thousand-puppet-pavilion))
### Thundering Mephis

- The source does not specify movement behavior beyond the rapid assault. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454277))
- The source does not specify any holding behavior. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454277))
### Tick Tack

- No additional passive, scaling, or hold/alternate behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454313))
### Traffic Illuminator

- No damage coefficients or scaling types provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454314))
- No hit-count, movement, or holding details provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454314))
### Tremor Warrior

- The fetched page states that the details are incomplete and based on pre-release information. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571388))
- No damage scaling/stat basis beyond the listed Electro DMG coefficient is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571388))
- No hit count, duration, movement details, holding behavior, or main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571388))
### Twin Nova - Collapsar Blade

- No movement behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571368))
- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571368))
- The total number of rapid-fire attacks/hits is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571368))
### Twin Nova - Nebulous Cannon

- No movement behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571366))
- No holding behavior is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571366))
- No separate damage coefficient is provided for the paired Twin Nova - Collapsar Blade effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571366))
### Vanguard Junrock

- No hit count specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454315))
- No holding behavior specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454315))
- No duration or stat-scaling attribute beyond the listed damage coefficient and flat value specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454315))
### Violet-Feathered Heron

- No exact Parry Stance duration is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454289))
- No movement or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454289))
- No hit count or separate main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454289))
### Viridblaze Saurian

- The source does not specify an active duration, hit interval, movement behavior, holding behavior, or main-slot passive effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454290))
### Vitreum Dancer

- Hit count: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492505))
- Damage scaling stat: n.a.; only the Electro DMG type and coefficient are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492505))
- Active effect duration: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492505))
- Movement/holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492505))
### Voidwing Moth

- No additional movement details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597653))
- No other scaling basis, such as ATK or HP scaling, is specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/597653))
### Voltscourge Stalker

- Movement behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492509))
- Holding behavior: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492509))
- Additional triggers, durations, scaling details, and passive effects: n.a. ([Game8](https://game8.co/games/Wuthering-Waves/archives/492509))
### Whiff Whaff

- No main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454316))
- No movement or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454316))
### Windlash Coleoid

- The source does not provide hit count, movement details, holding behavior, or a main-slot passive effect. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571369))
### Young Roseshroom

- No skill duration, hit count, movement behavior, or holding behavior is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454292))
- No separate main-slot passive effect is provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454292))
### Zig Zag

- Scaling basis beyond the stated 48.00% + 96 is not specified. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454021))
- The source does not state hit count, movement behavior, or holding behavior. ([Game8](https://game8.co/games/Wuthering-Waves/archives/454021))
### Zip Zap

- No skill duration, movement behavior, holding behavior, or main-slot passive details are provided. ([Game8](https://game8.co/games/Wuthering-Waves/archives/571389))
