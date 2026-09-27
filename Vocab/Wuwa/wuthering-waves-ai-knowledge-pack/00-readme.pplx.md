# Wuthering Waves: AI Knowledge Pack

ชุดไฟล์ Markdown สำหรับให้ AI ค้นข้อมูลและอ้างอิงต่อ ครบ 5 หมวดตามโจทย์ โดยใส่รายละเอียดสกิลจริงที่ค้นได้แทน template ว่าง. วันที่รวบรวมคือ 20 กันยายน 2026; เนื้อหาความสามารถใช้ภาษาอังกฤษเพื่อรักษาชื่อสกิลและคำทางระบบ ส่วนคำแนะนำการใช้งานเป็นภาษาไทย.

## ไฟล์หลัก

| ไฟล์ | เนื้อหา |
|---|---|
| `01-echo-mainstats-substats.md` | Mainstats แยก Cost 1/3/4 และ rarity 2–5; substats 13 ชนิด; ระบบ Modifier/Transducer |
| `02-echo-set-bonuses.md` | 34 Sonata sets พร้อมเงื่อนไข จำนวนชิ้น ระยะเวลา และ stack |
| `03-echo-skills-cost-4-3-1.md` | 181 Echo: Cost 4 = 43, Cost 3 = 53, Cost 1 = 85 พร้อม skill และ main-slot passive ที่แหล่งข้อมูลระบุ |
| `04-all-weapon-abilities.md` | 122 อาวุธ: passive, trigger, R1 และ progression R1–R5 พร้อมธงข้อมูลรอง |
| `05-all-character-abilities.md` | 58 kits แยก variants พร้อม Basic/Skill/Forte/Liberation/Intro/Outro/Inherent และ S1–S6 |
| `06-data-quality-and-coverage.md` | ช่องว่าง ข้อขัดแย้ง และการตัดสินใจเรื่องแหล่งข้อมูล |
| `character-chunks/` | แบ่งตัวละครเป็น 6 ไฟล์ย่อยสำหรับ AI ที่รับไฟล์ใหญ่ไม่สะดวก |
| `data/` | JSON ที่จัดโครงสร้างแล้ว มี URL ต้นทาง เหมาะกับการค้นและแปลงไฟล์ต่อ |

จำนวนข้างต้นนับจากระเบียนที่รวบรวมในชุดไฟล์ ไม่ใช่การรับรองจำนวนคอนเทนต์ทั้งหมดในเกม ณ ทุกเซิร์ฟเวอร์. รายการอ้างอิงหลักคือ [Game8 Echo List](https://game8.co/games/Wuthering-Waves/archives/452491), [Weapon List](https://game8.co/games/Wuthering-Waves/archives/452490) และ [Sonata Effects](https://game8.co/games/Wuthering-Waves/archives/456215); หน้ารายตัวแนบอยู่ในไฟล์แต่ละหมวด.

## อ่านก่อนใช้คำนวณ

- **ไม่ใช่ official game-data export:** ชุดนี้สรุปจากเว็บข้อมูลชุมชนและคู่มือ พร้อมลิงก์ต้นทาง ไม่ได้ดึงข้อมูลจาก client เกมหรือทดสอบทุกสกิลในเกม.
- **ขอบเขตเวอร์ชัน:** ใช้ snapshot ของหน้าที่ตรวจอ่าน ไม่รวมรายการ Echo ที่ยังเป็น TBD และไม่อ้างว่าครบคอนเทนต์ในอนาคต; หน้าอ้างอิงแสดงข้อมูลยุค 3.6 และ preview 3.7. ([Game8](https://game8.co/games/Wuthering-Waves/archives/559680))
- **ระดับสกิล:** ตัวเลขตัวละครส่วนใหญ่เป็น Lv.1 ตามตารางต้นทาง ไม่ใช่ Lv.10; เอฟเฟกต์คงที่และ attribute node ต้องอ่านแยกจากการเพิ่มระดับสกิล.
- **ข้อมูลขัดกัน:** Mainstats บางค่าไม่ตรงกันระหว่างเว็บ จึงเก็บทั้งสองค่า; JSON ใช้ `null` สำหรับ endpoint ที่ยังตัดสินไม่ได้. ([Game8](https://game8.co/games/Wuthering-Waves/archives/456278); [Wiki](https://wutheringwaves.fandom.com/wiki/Echo/Stats))
- **อาวุธที่ใช้แหล่งรอง:** R2–R5 ของ Lumingloss และ Thunderbolt ได้จาก Theria Games เพราะตาราง Game8 ไม่ครบ จึงควรตรวจในเกมก่อนคำนวณละเอียด. ([Lumingloss](https://theriagames.com/guide/wuthering-waves-lumingloss/); [Thunderbolt](https://theriagames.com/guide/wuthering-waves-thunderbolt/))

## วิธีส่งให้ AI

เริ่มจากไฟล์นี้และ `06-data-quality-and-coverage.md` แล้วแนบเฉพาะหมวดที่ต้องใช้. ถ้าต้องการให้ AI อ่านทั้งหมด ใช้ไฟล์รวมที่ส่งแยก หรือแตก ZIP แล้วอัปโหลดไฟล์ Markdown ตามความจุของระบบ; ไม่จำเป็นต้องอัปโหลดทั้งไฟล์ตัวละครรวมและ chunks ซ้ำกัน.

### Prompt พร้อมใช้

```text
ใช้ชุด Wuthering Waves AI Knowledge Pack ที่แนบเป็นฐานความรู้
1. อ่าน README และ data-quality ก่อน แล้วค้นในหมวดที่เกี่ยวข้อง
2. รักษาชื่อสกิล ตัวเลข หน่วย trigger stack duration cooldown และผู้รับบัฟ
3. ห้ามเติมข้อมูลจากความจำโดยไม่ระบุแหล่งอ้างอิงเพิ่มเติม
4. n.a. / null = ยังไม่ทราบ ไม่ใช่ 0 และไม่ใช่ไม่มีเอฟเฟกต์
5. หากแหล่งข้อมูลขัดกัน ให้รายงานสองค่าและขอค่าจากเกม ไม่เลือกเอง
6. แยก Cost, rarity, Echo Skill rank, weapon R1–R5 และ character S1–S6
7. ห้ามอ้างตัวเลข Skill Lv.1 เป็น Lv.10 หรือประมาณค่าระดับอื่นเอง
8. แยก DMG Bonus, Amplification, DEF ignore และ RES reduction
9. แยก Echo active, main-slot passive และ Sonata set bonus
10. คง URL อ้างอิงไว้ติดกับข้อมูลใน Markdown ที่สร้างต่อ
11. ถ้าคำถามเกินขอบเขตหรือ snapshot ของไฟล์ ให้ค้นเพิ่มและแจ้งส่วนที่อัปเดต
```

## สิ่งที่ชุดนี้ไม่ได้รับรอง

ไม่ได้ให้ damage simulator, rotation ที่ทดสอบจริง, tier list หรือ multiplier ทุกระดับ 1–10 ของทุกตัวละคร. ช่องว่างรายตัวอยู่ท้ายแต่ละระเบียนและใน audit file เพื่อให้ AI ไม่เข้าใจว่าแค่มีหัวข้อครบแล้วหมายถึงข้อมูลทุกฟิลด์ได้รับการยืนยัน.
