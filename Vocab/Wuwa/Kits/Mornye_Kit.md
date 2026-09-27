# Mornye — Kit Summary

> ปรับโครงจาก `WAF_HSR_Kit_Summary_Guide.md` มาใช้กับ Wuthering Waves
> (Path/Element → Element/Weapon, Trace A2/A4/A6 → Inherent Skill 1/2, Eidolon E1–E6 → Resonance Chain S1–S6)

| หัวข้อ | ข้อมูล |
|---|---|
| Element | Fusion |
| Weapon | Broadblade |
| Rarity | 5★ |
| Version | ไม่มีข้อมูล |
| Role | Healer / Support + Tune Break enabler (สเกลด้วย DEF และ Energy Regen) |
| Signature Weapon | ไม่มีข้อมูล |
| Core Resource | Rest Mass Energy → Relative Momentum |
| สภาวะหลัก | Wide Field Observation Mode + Syntony Field |

## TL;DR
- ตัวซัพพอร์ต Fusion ที่ฮีลด้วย **DEF** และปั๊มดาเมจให้ทั้งทีมผ่านระบบ **Marker + Tune Break**
- กินอาหารเป็น **Energy Regen** — ทุก 1% ที่เกิน 100% แปลงเป็น Crit Rate / Crit DMG ของตัวเอง และแปลงเป็น DMG Bonus ที่ทีมได้จาก Interfered Marker (เพดาน 40%)
- ลูปหลัก: สะสม Rest Mass Energy 100 → Heavy Attack กระโดดเข้า **Wide Field Observation Mode** → ตี Basic ในโหมดจน Relative Momentum เต็ม → **Heavy Attack - Inversion** ติด Observation Marker
- แพ้ทางคือโหมดหลักเปราะมาก: Dodge, Jump, สลับตัว, แตะสิ่งแวดล้อม หรือแตะพื้น = โหมดจบทันที และเดินในโหมดกิน Stamina ตลอดโดยไม่ฟื้น
- ทีมต้องมีคนที่ทำ **Tune Break DMG** ได้ ไม่งั้น Marker แทบไม่มีค่า

---

## ทรัพยากรและสภาวะพิเศษ

| ชื่อ | ได้มาจาก | เพดาน/ระยะเวลา | ใช้ทำอะไร |
|---|---|---|---|
| Rest Mass Energy | Baseline Mode: Basic ATK / Heavy ATK / Dodge Counter / Optimal Solution เข้าเป้า | สูงสุด 100 | ครบ 100 เปลี่ยน Heavy Attack เป็น Geopotential Shift (เข้าโหมด) |
| Relative Momentum | เฉพาะใน Wide Field Observation Mode: Basic ATK โหมด / Dodge Counter โหมด / Distributed Array เข้าเป้า (ห้ามได้ระหว่าง Inversion) | สูงสุด 100 | ครบ 100 เปลี่ยน Heavy Attack เป็น Inversion |
| Wide Field Observation Mode | Heavy Attack - Geopotential Shift หรือ Intro Skill | 30s | โหมดลอยกลางอากาศ เปลี่ยนชุดสกิล + สร้าง Syntony Field |
| Syntony Field | สร้างตอนเข้า Wide Field Observation Mode | 25s | ดาเมจตอนเกิด (นับเป็น Resonance Liberation DMG), ฮีลทุก 3s, +50% Off-Tune Buildup Rate, +ต้านการชะงัก |
| High Syntony Field | กด Critical Protocol ขณะมี Syntony Field อยู่ (แทนที่ของเดิม) | 25s | สืบทอดของเดิมทั้งหมด + DEF ทีม 20% + Healing Multiplier +40% |
| Parry | Resonance Skill - Expectation Error | ระยะเวลา ไม่มีข้อมูล | ลดดาเมจรับ 100% / โดนตี = จบ Parry แล้วออก Optimal Solution / สลับตัว = จบทันที |
| Observation Marker | Heavy Attack - Inversion (หรือระหว่าง Visual Field) | 30s | เพื่อนในทีมทำ Tune Break DMG ใส่เป้าที่มาร์ก → ติด Interfered Marker |
| Interfered Marker | เป้าที่มี Observation Marker โดน Tune Break DMG | 8s | เป้าที่ติด Tune Rupture/Strain - Interfered รับดาเมจจากทั้งทีมเพิ่ม (ER เกิน 100% ทุก 1% = +0.25%, cap 40%) |
| Visual Field | เพื่อนในทีมฆ่าเป้าที่มี Observation/Interfered Marker | 3s | ระหว่างนี้ เพื่อนตีอะไรก็ตาม Mornye จะติด Observation Marker ให้เป้านั้น |
| Proof of Boundedness | กด Expectation Error หรือ Distributed Array (IS2) | 60s / ได้ใหม่ทุก 5 นาที | กันดาเมจหนักและกันตาย (ดูหัวข้อ Inherent Skill 2) |
| Stagnation | Optimal Solution | ไม่มีข้อมูล (จำนวนเป้า/ระยะเวลาไม่ระบุ) | ตรึงศัตรูรอบตัว / สลับตัว = จบก่อนกำหนด |

---

## สกิลรายตัว

### Mechanic พิเศษเฉพาะตัว — Forte Circuit: Mass-Energy Equivalence
แกนของตัวละคร: สะสมพลังงาน 2 ชั้นเพื่อเข้าโหมดลอยตัวแล้วติด Marker ให้ทีมรุมขยี้

- **Baseline Mode** (โหมดปกติ) คือช่วงที่สะสม Rest Mass Energy
- **Heavy Attack - Geopotential Shift** (Rest Mass Energy 100): ดาเมจ Fusion นับเป็น Heavy Attack DMG → 22.20% + 49.81% (Lv.1) แล้วดีดตัวขึ้นอากาศ กินพลังงานทั้งหมด เข้า Wide Field Observation Mode
- **Wide Field Observation Mode** อยู่ได้ 30s: ค้างปุ่ม Normal Attack จะยิง Basic Stage 1→3 ต่อเนื่อง ถ้า Relative Momentum เต็มระหว่างทางจะกลายเป็น Heavy Attack - Inversion แทน
- ในโหมด: เคลื่อนที่กิน Stamina 5/วินาที และ **Stamina ไม่ฟื้น**; Dodge แบบมีทิศทาง = บินเร็วได้สูงสุด 10s
- ในโหมด: โดนตีหรือถูกดีดลอย กด Dodge ฟื้นตัวทันทีและนับเป็น Dodge สำเร็จ — ได้ 3 ครั้ง รีเซ็ตเมื่อออกจากโหมด
- กด Jump = ร่อนลงช้าๆ ระหว่างร่อนใช้ Basic โหมด / Distributed Array / Inversion ไม่ได้ ถ้ากด Jump ตอน Stamina หมด = ออกจากโหมด
- โหมดจบเมื่อ: Dodge, Jump, Mid-air Attack, โต้ตอบสิ่งแวดล้อม, ใช้ Utility, สลับตัว, หรือไม่ได้ลอยอยู่แล้ว
- **Heavy Attack - Inversion** (Relative Momentum 100): กินโมเมนตัมทั้งหมด ดาเมจ 130.00% (Lv.1) นับเป็น Heavy Attack DMG ใช้กลางอากาศได้ และติด **Observation Marker** 30s
- **Syntony Field** (เกิดพร้อมโหมด) 25s: ดาเมจตอนเกิด 20.00%×5 นับเป็น Resonance Liberation DMG, ฮีล 40 + 9.63% DEF ทุก 3s, +50% Off-Tune Buildup Rate, เพิ่มต้านชะงัก
- **Interfered Marker**: ทุก 1% ของ Energy Regen ที่เกิน 100% → ทีมตีเป้านั้นแรงขึ้น 0.25% เพดาน 40%
- **Tune Rupture Response - Particle Jet**: ดาเมจ Fusion 1 ครั้งใส่เป้าที่อยู่ในสถานะ Tune Rupture - Interfered — 150.00% Tune AMP (Lv.1) นับเป็น Tune Rupture DMG
- (IS1) Energy Regen ของ Mornye +10%
- (IS1) กด Intro Skill คืน Concerto Energy 20 (ทุก 20s) และ Basic โหมด Stage 3 คืนอีก 20 (ทุก 20s)

### Basic ATK — Ground State Calibration
ชุดตีปกติ 4 สเต็ป และมีชุดแยกเฉพาะตอนอยู่ในโหมด

- Basic Attack: ตีต่อเนื่องสูงสุด 4 สเต็ป ดาเมจ Fusion
  - Stage 1: 11.20% + 8.40%×2 | Stage 2: 12.00% + 12.00% + 9.00%×4 | Stage 3: 20.80% + 5.20%×6 | Stage 4: 68.00% (ทั้งหมด Lv.1)
- Heavy Attack: กิน Stamina 25 — 5.58% + 5.58% + 7.44% (Lv.1)
- Mid-air Attack: กิน Stamina 30 — 49.60% (Lv.1) กด Normal ต่อในเวลาที่กำหนด = ออก Basic Stage 3
- Dodge Counter: 81.60% (Lv.1) กด Normal ต่อ = ออก Basic Stage 2

#### Wide Field Observation Mode (ร่างเสริม)
- Basic ATK โหมด: ตีต่อเนื่อง 3 สเต็ป — Stage 1: 7.00%×4 | Stage 2: 13.00%×4 | Stage 3: 4.68%×4 + 16.64%×2 (Lv.1)
- Dodge Counter โหมด: 13.00%×4 (Lv.1) กด Normal ต่อ = ออก Basic โหมด Stage 3

### Resonance Skill — Resolution
สกิลฮีล + ตั้งการ์ดสวน และเปลี่ยนเป็นสกิลฮีลระยะไกลเมื่ออยู่ในโหมด

- **Expectation Error**: ฮีลทีมรอบตัว 49 + 11.88% DEF (Lv.1) แล้วเข้า Parry ลดดาเมจรับ 100% | CD 5s
  - โดนตีระหว่าง Parry → จบ Parry แล้วออก **Optimal Solution** ทันที
  - ไม่โดนตี → กด Normal Attack เพื่อจบ Parry แล้วออก Basic Stage 2
- **Optimal Solution**: ตรึงเป้ารอบตัว (Stagnation) ดาเมจ 90.40% (Lv.1) และลด CD ของ Expectation Error ลง 2 วินาที
- **Distributed Array** (แทนที่ Resonance Skill ในโหมด): ฮีล 225 + 54.00% DEF (Lv.1) + เรียก Hover Cannons ตีเป้า 20.00%×4 | CD 16s | Concerto +10
- (IS2) การกด Expectation Error หรือ Distributed Array จะแจก **Proof of Boundedness** ให้ทั้งทีม (ดูหัวข้ออื่นๆ)

### Resonance Liberation — Critical Protocol (Energy 175)
ท่าไม้ตายที่สเกลจาก DEF และแปลง Energy Regen ส่วนเกินเป็นคริต

- ดาเมจ 262.75% ของ **DEF** (Lv.1) ใส่เป้าในระยะ | CD 25s | Concerto +20 | ใช้กลางอากาศได้
- ทุก 1% ของ Energy Regen ที่เกิน 100%: Crit Rate +0.5% (cap 80%) และ Crit DMG +1% (cap 160%)
- ถ้ามี Syntony Field อยู่ จะถูกแทนที่ด้วย **High Syntony Field** 25s: DEF ทีม +20%, Healing Multiplier +40%, สืบทอดฮีล/ต้านชะงัก/Off-Tune Buildup Rate ของสนามเดิม

### Intro / Outro
- **Intro Skill — Convergence**: ดาเมจ 102.00% (Lv.1) แล้วดีดตัวขึ้นอากาศ ล้าง Rest Mass Energy ทั้งหมด และเข้า Wide Field Observation Mode ทันที | Concerto +10
- **Outro Skill — Recursion**: ทั้งทีมได้ All DMG Amplification 25% นาน 30s

### Tune Break — Decoupling
ระบบเสริมกับกลไก Off-Tune ของทีม

- ตอบสนองต่อสถานะ Tune Rupture - Interfered และ Tune Strain - Interfered ได้
- เพื่อนทำ Tune Break DMG แล้วติด Tune Rupture - Interfered → Mornye ยิง Particle Jet อัตโนมัติ (เป้าละครั้งทุก 8s)
- Tune Strain - Interfered แต่ละสแต็กเพิ่ม Total DMG ของ Mornye ต่อเป้านั้น — ทุก 1 แต้ม Tune Break Boost = +0.12%
- มี Mornye ในทีม เพดานสแต็ก Tune Strain - Interfered ของเป้า +1
- Mornye ทำ Tune Break ใส่เป้าที่ Off-Tune Level เต็มได้

### อื่นๆ
- **(IS2) Proof of Boundedness** — อยู่ 60s, ได้ใหม่ทุก 5 นาที
  - ตัวที่กำลังเล่นจะโดนดาเมจเกิน 30% Max HP ไม่ได้ (แปลงเหลือ 30% Max HP) ใช้ได้ 3 ครั้งแล้วหมดสภาวะ
  - ดาเมจที่ควรทำให้ล้ม จะรอดแทน 1 ครั้ง แล้วหมดสภาวะ
  - ตอน Proof หมด ตัวที่เล่นอยู่ฟื้น HP เท่ากับ 150% DEF ของ Mornye

### สรุป Flow การเล่น
1. สลับเข้ามาด้วย **Intro Skill — Convergence** ถ้าทำได้ = เข้าโหมดฟรีทันทีโดยไม่ต้องสะสม
2. ถ้าเข้าเองแบบไม่มี Intro: อยู่ Baseline Mode เก็บ Rest Mass Energy ด้วย Basic / Heavy / Dodge Counter / Optimal Solution
3. ระหว่างนั้นกด **Expectation Error** เพื่อฮีล ตั้ง Parry และแจก Proof of Boundedness (โดนตี = ออก Optimal Solution ฟรี + ลด CD 2s)
4. Rest Mass Energy ครบ 100 → **Heavy Attack - Geopotential Shift** เข้า Wide Field Observation Mode พร้อม Syntony Field
5. ในโหมด: ค้าง Normal Attack ไล่ Basic Stage 1→3 และกด **Distributed Array** เพื่อฮีล + เก็บ Relative Momentum
6. Relative Momentum ครบ 100 → **Heavy Attack - Inversion** ติด Observation Marker 30s
7. กด **Critical Protocol** (ถ้าพลังงานพอ) เพื่ออัปสนามเป็น High Syntony Field
8. สลับออกด้วย **Outro — Recursion** ให้ทีม +25% All DMG Amp แล้วให้เพื่อนทำ Tune Break ใส่เป้าที่มาร์ก → Interfered Marker → Particle Jet ยิงเองอัตโนมัติ
9. เป้าตายระหว่างมีมาร์ก → ได้ Visual Field 3s → มาร์กตัวถัดไปฟรี แล้ววนกลับข้อ 2

---

## Resonance Chain (S1–S6)

| ลำดับ | ชื่อ | ผลของมัน | ความสำคัญ |
|---|---|---|---|
| S1 | The Silent Observer | Basic โหมดไม่โดนชะงัก, Interfered Marker อยู่นานขึ้น 150%, ให้ DMG Bonus แม้เป้าไม่ติด Tune Rupture/Strain - Interfered, ติด Observation Marker = ติด Interfered Marker ด้วย | จุดเปลี่ยนเกม |
| S2 | Morning Star of Entropy | ทีมได้ Crit DMG ใส่เป้าที่มี Interfered Marker (ER เกิน 100% ทุก 1% = +0.2%, cap 32%); Syntony/High Syntony Field เพิ่ม Off-Tune Buildup Rate ทั้งทีมอีก 20% | คุ้มค่า |
| S3 | Blueprint of Recursion | Distributed Array คืน Concerto 25 และ Relative Momentum 100 (ทุก 25s) | คุ้มค่า (ลดรอบสะสม) |
| S4 | Latent Variables of the Cosmos | High Syntony Field ฮีลเพิ่ม 30% | เสริมเล็กน้อย |
| S5 | Time Dilation Effect | Critical Protocol +40% DMG Multiplier, Particle Jet +160% DMG Multiplier | คุ้มค่า |
| S6 | To the Far Shores of the Stars | Critical Protocol ดาเมจเพิ่ม 400%; ออกจากไฟต์เกิน 4s ฟื้น Resonance Energy 10% ของ Max ทุก 0.2s | จุดเปลี่ยนเกม |

---

## ข้อควรระวัง & เงื่อนไขทีม
- **ต้องมีคนทำ Tune Break DMG ในทีม** ไม่งั้น Observation Marker ไม่แปลงเป็น Interfered Marker และ Particle Jet ไม่ยิง
- ปั้น **Energy Regen เกิน 100% ให้มากที่สุด** — เป็นทั้งคริตของตัวเอง (cap ที่ +160% ER) และ DMG Bonus ของทีม (cap ที่ +160% ER)
- ฮีลและดาเมจอัลติสเกลจาก **DEF** ไม่ใช่ ATK — ของขึ้น ATK แทบไม่มีประโยชน์
- Wide Field Observation Mode หลุดง่ายมาก: Dodge / Jump / Mid-air Attack / สลับตัว / แตะพื้น / ใช้ Utility = จบทันที
- ในโหมดกิน Stamina 5/วินาทีและไม่ฟื้น — ถ้าเดินเยอะจะไม่พอไล่ Relative Momentum ให้เต็ม
- Parry ของ Expectation Error หายทันทีที่สลับตัว ใช้เป็นการ์ดตอนจะสลับไม่ได้
- Proof of Boundedness ได้ใหม่ทุก **5 นาที** เท่านั้น ถือเป็นของสำรองชีวิต ไม่ใช่ของประจำรอบ
- Resonance Energy 175 ถือว่าสูง ต้องได้ ER จากของสวมอยู่แล้ว (ซึ่งตรงกับที่ต้องปั้นอยู่แล้ว)

---

## Build / Weapon / Echo / ทีม
- ไม่มีข้อมูล (แหล่งที่ใช้ให้เฉพาะรายละเอียดสกิล ไม่มีคำแนะนำ Echo / Sonata / อาวุธ / ทีมสำหรับ Mornye)
- ทิศทางที่อนุมานได้จากตัวเลขในสกิลเท่านั้น: เน้น Energy Regen + DEF% + Healing Bonus ❓

---

## หมายเหตุความครบถ้วนของข้อมูล (จากแหล่งเดิม)
- ไม่มีสูตร level scaling ของเอฟเฟกต์ส่วนใหญ่ — ตัวเลขทั้งไฟล์เป็นค่าที่ **skill Lv.1**
- ระยะเวลาของ Parry ไม่ระบุ (บอกแค่ลดดาเมจ 100%)
- จำนวนเป้า/ระยะเวลา/รายละเอียดของ Stagnation จาก Optimal Solution ไม่ระบุ
- Stamina รวมและความเร็วบินในโหมด ไม่ระบุ
- ไม่มีตารางตัวเลขแยกสำหรับ Proof of Boundedness / Visual Field / Observation Marker / Interfered Marker
- ขอบเขตคำว่า "their DMG" ของ Interfered Marker ระบุแค่ "ทีมที่อยู่ใกล้"
- ข้อความ S1 ในแหล่งข้อมูลมี typo "pr" ตีความเป็น "or"
- Syntony Field / High Syntony Field ไม่ได้เป็นสกิลแยกในแหล่งข้อมูล แต่ยกมาเป็นหัวข้อเพราะมีกลไกจริง

---

## แหล่งอ้างอิง
- ข้อมูลดิบในเครื่อง: `Vocab/Wuwa/All Character Abilities  Researched Inventory.md` (หัวข้อ Mornye)
- ต้นทาง: [Game8 — Mornye](https://game8.co/games/Wuthering-Waves/archives/568193) ❓ (เว็บสรุป ไม่ใช่ text ในเกมโดยตรง)
- อ้างอิงเวอร์ชันเกม: ไม่มีข้อมูล (ไฟล์ reference ในเครื่องระบุ 3.5–3.6)
- วันที่เรียบเรียง: 2026-09-20
