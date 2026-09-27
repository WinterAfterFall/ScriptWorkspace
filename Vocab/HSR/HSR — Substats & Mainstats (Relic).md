# Honkai: Star Rail — Relic Substats & Mainstats

> อ้างอิงหลัก: [Honkai: Star Rail Fandom Wiki — Relic/Stats](https://honkai-star-rail.fandom.com/wiki/Relic/Stats)
> ข้อมูล ณ เวอร์ชัน 3.7–3.8 (กันยายน 2026)

---

## 1. สรุปโครงสร้าง Relic

Relic แต่ละชิ้นมี:
- **Main Stat** 1 ค่า (สุ่มตาม slot และมี weight ต่างกัน)
- **Sub Stat** 1–4 ค่า (เริ่มต้นตามความหายาก และเพิ่ม/อัปเกรดทุก 3 level)

Relic แบ่งเป็น 2 ประเภท:
- **Cavern Relic** (4 ชิ้น 1 set): Head, Hands, Body, Feet
- **Planar Ornament** (2 ชิ้น 1 set): Planar Sphere, Link Rope

---

## 2. Main Stat ตามช่อง (Slot)

### ตารางความเป็นไปได้ของ Main Stat

| Main Stat | Head | Hands | Body | Feet | Planar Sphere | Link Rope |
|---|:---:|:---:|:---:|:---:|:---:|:---:|
| HP (flat) | ✓ | — | — | — | — | — |
| ATK (flat) | — | ✓ | — | — | — | — |
| HP% | — | — | ✓ | ✓ | ✓ | ✓ |
| ATK% | — | — | ✓ | ✓ | ✓ | ✓ |
| DEF% | — | — | ✓ | ✓ | ✓ | ✓ |
| Effect Hit Rate | — | — | ✓ | — | — | — |
| Outgoing Healing Boost | — | — | ✓ | — | — | — |
| CRIT Rate | — | — | ✓ | — | — | — |
| CRIT DMG | — | — | ✓ | — | — | — |
| SPD | — | — | — | ✓ | — | — |
| Physical DMG Boost | — | — | — | — | ✓ | — |
| Fire DMG Boost | — | — | — | — | ✓ | — |
| Ice DMG Boost | — | — | — | — | ✓ | — |
| Wind DMG Boost | — | — | — | — | ✓ | — |
| Lightning DMG Boost | — | — | — | — | ✓ | — |
| Quantum DMG Boost | — | — | — | — | ✓ | — |
| Imaginary DMG Boost | — | — | — | — | ✓ | — |
| Break Effect | — | — | — | — | — | ✓ |
| Energy Regeneration Rate | — | — | — | — | — | ✓ |

**หมายเหตุ:** Head จะได้ HP (flat) เสมอ 100%, Hands ได้ ATK (flat) เสมอ 100%

### ความน่าจะเป็นของ Main Stat แต่ละช่อง

| Main Stat | Body | Feet | Planar Sphere | Link Rope |
|---|:---:|:---:|:---:|:---:|
| HP% | 20% | 28% | 12% | 26% |
| ATK% | 20% | 30% | 13% | 27% |
| DEF% | 20% | 30% | 12% | 24% |
| Effect Hit Rate | 10% | — | — | — |
| Outgoing Healing Boost | 10% | — | — | — |
| CRIT Rate | 10% | — | — | — |
| CRIT DMG | 10% | — | — | — |
| SPD | — | 12% | — | — |
| Physical / Fire / Ice / Wind / Lightning / Quantum / Imaginary DMG Boost (แต่ละธาตุ) | — | — | 9% | — |
| Break Effect | — | — | — | 16% |
| Energy Regeneration Rate | — | — | — | 5% |

---

## 3. ค่า Main Stat ตามความหายาก

**สูตร:** `Max = Base + Per Level × 15 (5★) / 12 (4★) / 9 (3★) / 6 (2★)`

### 5-Star Relics

| Stat | Base | Per Lv. | Max |
|---|---:|---:|---:|
| SPD | 4.032 | 1.4 | 25.032 |
| HP (flat) | 112.896 | 39.5136 | 705.6 |
| ATK (flat) | 56.448 | 19.7568 | 352.8 |
| HP% | 6.912% | 2.4192% | 43.20% |
| ATK% | 6.912% | 2.4192% | 43.20% |
| DEF% | 8.640% | 3.024% | 54.00% |
| Break Effect | 10.368% | 3.6288% | 64.80% |
| Effect Hit Rate | 6.912% | 2.4192% | 43.20% |
| Energy Regeneration Rate | 3.1104% | 1.0886% | 19.4394% |
| Outgoing Healing Boost | 5.5296% | 1.9354% | 34.5606% |
| Elemental DMG Boost (Phys/Fire/Ice/Wind/Ltng/Qnt/Img) | 6.2208% | 2.1773% | 38.8803% |
| CRIT Rate | 5.184% | 1.8144% | 32.40% |
| CRIT DMG | 10.368% | 3.6288% | 64.80% |

### 4-Star Relics

| Stat | Base | Per Lv. | Max |
|---|---:|---:|---:|
| SPD | 3.2256 | 1.1 | 16.4256 |
| HP (flat) | 90.3168 | 31.61088 | 469.6474 |
| ATK (flat) | 45.1584 | 15.80544 | 234.8237 |
| HP% | 5.5296% | 1.9354% | 28.7544% |
| ATK% | 5.5296% | 1.9354% | 28.7544% |
| DEF% | 6.912% | 2.4192% | 35.9424% |
| Break Effect | 8.2944% | 2.9030% | 43.1304% |
| Effect Hit Rate | 5.5296% | 1.9354% | 28.7544% |
| Energy Regeneration Rate | 2.4883% | 0.8709% | 12.9391% |
| Outgoing Healing Boost | 4.4237% | 1.5483% | 23.0033% |
| Elemental DMG Boost | 4.9766% | 1.7418% | 25.8782% |
| CRIT Rate | 4.1472% | 1.4515% | 21.5652% |
| CRIT DMG | 8.2944% | 2.9030% | 43.1304% |

### 3-Star Relics

| Stat | Base | Per Lv. | Max |
|---|---:|---:|---:|
| SPD | 2.4192 | 1.0 | 11.4192 |
| HP (flat) | 67.7376 | 23.70816 | 281.111 |
| ATK (flat) | 33.8688 | 11.85408 | 140.5555 |
| HP% | 4.1472% | 1.4515% | 17.2107% |
| ATK% | 4.1472% | 1.4515% | 17.2107% |
| DEF% | 5.184% | 1.8144% | 21.5136% |
| Break Effect | 6.2208% | 2.1773% | 25.8165% |
| Effect Hit Rate | 4.1472% | 1.4515% | 17.2107% |
| Energy Regeneration Rate | 1.8662% | 0.6532% | 7.745% |
| Outgoing Healing Boost | 3.3178% | 1.1612% | 13.7686% |
| Elemental DMG Boost | 3.7325% | 1.3064% | 15.4901% |
| CRIT Rate | 3.1104% | 1.0886% | 12.9078% |
| CRIT DMG | 6.2208% | 2.1773% | 25.8165% |

### 2-Star Relics

| Stat | Base | Per Lv. | Max |
|---|---:|---:|---:|
| SPD | 1.6128 | 1.0 | 7.6128 |
| HP (flat) | 45.1584 | 15.80544 | 139.991 |
| ATK (flat) | 22.5792 | 7.90272 | 69.9955 |
| HP% | 2.7648% | 0.9677% | 8.5710% |
| ATK% | 2.7648% | 0.9677% | 8.5710% |
| DEF% | 3.456% | 1.2096% | 10.7136% |
| Break Effect | 4.1472% | 1.4515% | 12.8562% |
| Effect Hit Rate | 2.7648% | 0.9677% | 8.5710% |
| Energy Regeneration Rate | 1.2442% | 0.4355% | 3.8572% |
| Outgoing Healing Boost | 2.2118% | 0.7741% | 6.8564% |
| Elemental DMG Boost | 2.4883% | 0.8709% | 7.7137% |
| CRIT Rate | 2.0736% | 0.7258% | 6.4284% |
| CRIT DMG | 4.1472% | 1.4515% | 12.8562% |

---

## 4. Sub Stat Pool และ Weight

Sub Stat ถูกสุ่มจาก pool 12 ชนิดด้วยระบบ weight (คล้าย Genshin Impact) โดย pool รวม weight เริ่มต้น = 100

| Sub Stat | Weight | สัดส่วนเริ่มต้น |
|---|---:|---:|
| HP (flat) | 10 | 10% |
| ATK (flat) | 10 | 10% |
| DEF (flat) | 10 | 10% |
| HP% | 10 | 10% |
| ATK% | 10 | 10% |
| DEF% | 10 | 10% |
| SPD | 4 | 4% |
| CRIT Rate | 6 | 6% |
| CRIT DMG | 6 | 6% |
| Effect Hit Rate | 8 | 8% |
| Effect RES | 8 | 8% |
| Break Effect | 8 | 8% |

**หมายเหตุ:** เมื่อมี substat ถูกเลือกไปแล้ว หรือ Main Stat เป็นตัวเดียวกัน weight ของ substat นั้นจะถูกลบออกจาก pool

---

## 5. ค่า Sub Stat ต่อ 1 Roll ตามความหายาก

Sub Stat แต่ละครั้งจะสุ่มค่าจาก 3 tier: Low / Med / High

### 5-Star Relic Roll

| Sub Stat | Low | Med | High |
|---|---:|---:|---:|
| SPD | 2.0 | 2.3 | 2.6 |
| HP (flat) | 33.87 | 38.10 | 42.34 |
| ATK (flat) | 16.935 | 19.052 | 21.169 |
| DEF (flat) | 16.935 | 19.052 | 21.169 |
| HP% | 3.456% | 3.888% | 4.320% |
| ATK% | 3.456% | 3.888% | 4.320% |
| DEF% | 4.320% | 4.860% | 5.400% |
| Break Effect | 5.184% | 5.832% | 6.480% |
| Effect Hit Rate | 3.456% | 3.888% | 4.320% |
| Effect RES | 3.456% | 3.888% | 4.320% |
| CRIT Rate | 2.592% | 2.916% | 3.240% |
| CRIT DMG | 5.184% | 5.832% | 6.480% |

### 4-Star Relic Roll

| Sub Stat | Low | Med | High |
|---|---:|---:|---:|
| SPD | 1.6 | 1.8 | 2.0 |
| HP (flat) | 27.096 | 30.483 | 33.87 |
| ATK (flat) | 13.548 | 15.242 | 16.935 |
| DEF (flat) | 13.548 | 15.242 | 16.935 |
| HP% | 2.7648% | 3.1104% | 3.456% |
| ATK% | 2.7648% | 3.1104% | 3.456% |
| DEF% | 3.456% | 3.888% | 4.320% |
| Break Effect | 4.1472% | 4.6656% | 5.184% |
| Effect Hit Rate | 2.7648% | 3.1104% | 3.456% |
| Effect RES | 2.7648% | 3.1104% | 3.456% |
| CRIT Rate | 2.0736% | 2.3328% | 2.592% |
| CRIT DMG | 4.1472% | 4.6656% | 5.184% |

### 3-Star Relic Roll

| Sub Stat | Low | Med | High |
|---|---:|---:|---:|
| SPD | 1.2 | 1.3 | 1.4 |
| HP (flat) | 20.322 | 22.862 | 25.403 |
| ATK (flat) | 10.161 | 11.431 | 12.701 |
| DEF (flat) | 10.161 | 11.431 | 12.701 |
| HP% | 2.0736% | 2.3328% | 2.592% |
| ATK% | 2.0736% | 2.3328% | 2.592% |
| DEF% | 2.592% | 2.916% | 3.240% |
| Break Effect | 3.1104% | 3.4992% | 3.888% |
| Effect Hit Rate | 2.0736% | 2.3328% | 2.592% |
| Effect RES | 2.0736% | 2.3328% | 2.592% |
| CRIT Rate | 1.5552% | 1.7496% | 1.944% |
| CRIT DMG | 3.1104% | 3.4992% | 3.888% |

### 2-Star Relic Roll

| Sub Stat | Low | Med | High |
|---|---:|---:|---:|
| SPD | 1.0 | 1.1 | 1.2 |
| HP (flat) | 13.548 | 15.242 | 16.935 |
| ATK (flat) | 6.774 | 7.621 | 8.468 |
| DEF (flat) | 6.774 | 7.621 | 8.468 |
| HP% | 1.3824% | 1.5552% | 1.728% |
| ATK% | 1.3824% | 1.5552% | 1.728% |
| DEF% | 1.728% | 1.944% | 2.160% |
| Break Effect | 2.0736% | 2.3328% | 2.592% |
| Effect Hit Rate | 1.3824% | 1.5552% | 1.728% |
| Effect RES | 1.3824% | 1.5552% | 1.728% |
| CRIT Rate | 1.0368% | 1.1664% | 1.296% |
| CRIT DMG | 2.0736% | 2.3328% | 2.592% |

---

## 6. กฎการเพิ่ม/อัปเกรด Sub Stat

| ความหายาก | Max Level | จำนวน Sub Stat เริ่มต้น | จำนวนครั้งเพิ่ม/อัปเกรด |
|---|:---:|:---:|:---:|
| 5-Star | +15 | 3 หรือ 4 | 5 ครั้ง (ทุก 3 level) |
| 4-Star | +12 | 2 หรือ 3 | 4 ครั้ง |
| 3-Star | +9 | 1 หรือ 2 | 3 ครั้ง |
| 2-Star | +6 | 0 | 2 ครั้ง |

### กฎการทำงาน

1. **ทุก 3 level** relic จะเพิ่ม sub stat ใหม่ (ถ้ายังไม่ครบ 4) หรือ **อัปเกรด** sub stat ที่มีอยู่แล้ว
2. หลังจากมี sub stat ครบ 4 แล้ว การ enhance ทุก 3 level จะสุ่มอัปเกรด 1 ใน 4 ตัวที่มีอยู่
3. Relic 5★ ที่เริ่มด้วย 4 sub stat จะสามารถ enhance sub stat ได้ **สูงสุด 5 ครั้ง** (level +15)
4. Relic 3★ ที่เริ่มด้วย 1 sub stat ไม่สามารถ enhance sub stat ได้เลย (level +9 = เพิ่ม 3 ครั้ง จะครบ 4 ตัวพอดี)

### ข้อจำกัด

- **ห้าม** สุ่ม sub stat ซ้ำกัน
- **ห้าม** สุ่ม sub stat ที่เป็นชนิดเดียวกับ main stat
- Head relic (main = HP flat) จะได้ HP% เป็น sub stat ได้ แต่ห้ามได้ HP flat
- Relic **ไม่สามารถ** มี HP% เป็น sub stat 2 ตัว
- Relic **สามารถ** มี ATK flat และ ATK% เป็น sub stat พร้อมกันได้ (คนละชนิด)

---

## 7. Priority Guide (สรุปแบบ meta)

### Main Stat ที่นิยม (โดยทั่วไป)

| Slot | DPS ทั่วไป | Break Effect DPS | Support/Healer | Sub-DPS/Follow-up |
|---|---|---|---|---|
| **Body** | CRIT Rate / CRIT DMG | ATK% / Break Effect | Outgoing Healing / EHR | CRIT Rate/DMG |
| **Feet** | SPD หรือ ATK% | SPD | SPD | SPD |
| **Planar Sphere** | Elemental DMG Boost (ตาม element) | ATK% / HP% | HP% / DEF% | Elemental DMG Boost |
| **Link Rope** | ATK% / Energy Regen | Break Effect | Energy Regen | ATK% / Energy Regen |

### Sub Stat Priority (โดยทั่วไป)

1. **CRIT Rate / CRIT DMG** (ตัว DPS หลัก) — เป้าอัตราส่วน 1:2
2. **SPD** — สำคัญมากสำหรับทุกตัว โดยเฉพาะ support
3. **ATK%** — สำหรับ scaling ATK
4. **Break Effect** — สำหรับ Break DPS
5. **Effect Hit Rate** — สำหรับ DoT / Debuffer
6. **Effect RES / HP%** — สำหรับ tank/sustain

---

## แหล่งอ้างอิง

- [Honkai: Star Rail Fandom Wiki — Relic/Stats](https://honkai-star-rail.fandom.com/wiki/Relic/Stats)
- [Honkai: Star Rail Fandom Wiki — Relic](https://honkai-star-rail.fandom.com/wiki/Relic)
- [Prydwen — Relic Stats Guide](https://www.prydwen.gg/star-rail/guides/relic-stats)
- [Gacha Data — Relic Substats](https://gacha-data.com/honkai-star-rail/relic-substats/)
