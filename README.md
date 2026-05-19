# 🌌 Another Universe

🇹🇭 [ภาษาไทย](#-thai) · 🇬🇧 [English](#-english)

---

<a id="-thai"></a>

## 🇹🇭 Thai

*"ถ้าตัวละครสองคนได้พบกันในโลกที่แตกต่างออกไป เรื่องราวของพวกเขาจะยังเหมือนเดิมไหม?"*

**Another Universe** เป็น Extension สำหรับ [SillyTavern](https://github.com/SillyTavern/SillyTavern) ที่จะพาตัวละครของคุณกระโดดข้ามมิติไปยังโลกคู่ขนาน นำบุคลิก ความสัมพันธ์ และน้ำเสียงที่มีอยู่ มาตีความใหม่ผ่านสถานการณ์และอารมณ์ที่แตกต่างออกไปในทุกครั้งที่กด Generate

> 💡 **รองรับ 2 ภาษา (TH / EN):** ระบบจะตรวจภาษาของ SillyTavern อัตโนมัติ หรือเลือกเองได้จากการตั้งค่า Extension ในแถบ Extensions

---

### ✨ Features (จุดเด่น)

- **🎭 150,000+ ความเป็นไปได้:** ผสมผสาน 51 ธีมโลก × 53 เหตุการณ์การพบกัน × 54 โทนอารมณ์ หรือจะปล่อยให้ AI เลือกเองทั้งหมดก็ได้
- **🎨 Custom Theme / Encounter / Mood:** อยากได้โลกในแบบของคุณเองจริงๆ? เลือก `🎨 กำหนดเอง` ในแต่ละช่อง แล้วบรรยายโลก / รูปแบบการพบเจอ / โทนอารมณ์ลงไปได้ตรงๆ (สูงสุด 1,000 ตัวอักษรต่อช่อง) ระบบจะส่งคำบรรยายของคุณเข้า prompt แบบ priority block พร้อม anti-injection wrapper สลับใช้ระหว่าง preset กับ custom ได้อิสระทุกฟิลด์
- **🎴 Export Character Card:** เปลี่ยนเรื่องที่ generate ได้ให้กลายเป็นการ์ดตัวละครได้ทันที รองรับ 2 รูปแบบ:
  - **🎴 PNG Card** — Character Card V2 PNG (drag-drop เข้า SillyTavern ได้ทันที, ฝังด้วย tEXt chunk + base64)
  - **🗂️ JSON** — Character Card V2 JSON เปล่า (portable สำหรับ TavernAI / RisuAI / JanitorAI หรือเป็น fallback ถ้า PNG มีปัญหา)
  - เนื้อเรื่องที่ generate กลายเป็น `first_mes` อัตโนมัติ (พร้อมแทนชื่อเป็น `{{user}}` / `{{char}}` placeholder), `scenario` รวม theme + encounter + mood, ดึง avatar / description / personality / mes_example / creator จาก char ตัวเดิมไว้ครบ
- **🌐 Multilingual (TH / EN):** สลับภาษาทั้ง UI ได้ทุกจุด รวมถึง dropdown labels ทั้ง 158 รายการ ตั้ง Language เป็น Auto/TH/EN ได้ในแถบ Extensions
- **🤯 Wild Themes:** ครอบคลุมตั้งแต่ ละครไทย, ตำนานไทย, ครึ่งสัตว์, ยุคดึกดำบรรพ์, จีนกำลังภายใน, ซอมบี้, มาเฟีย, แวมไพร์, โลกในเกม, วนลูปเวลา, ตะวันตกเถื่อน, อวกาศโอเปร่า, นักสืบ, ซามูไร, คาสิโน, ประภาคาร และอีกมากมาย
- **🔥 Dark & Spicy:** มีตัวเลือกสายมืดและสายแซ่บ เช่น ยันเดเระ, เลือดสาด, สลับร่าง, แฟนกำมะลอ, คลุมถุงชน, คนกับผี, สัญญากับปีศาจ, ตัวประกัน, การประมูล, นักล่าเงินรางวัล
- **🎨 Period-Appropriate Language:** ระบบปรับภาษาและสรรพนามให้เหมาะกับยุคสมัย (เช่น ยุคกลางใช้ thee/thou, ไทยใช้ ข้าพเจ้า/ท่าน, ญี่ปุ่นใช้ honorifics)
- **⚡ Quick Settings:** ปุ่ม `🌌` ในเมนูแชท (เหนือ Author Note) เปิดหน้าตั้งค่าด่วน เลือกธีมแล้ว Generate ได้ทันที
- **📚 Universe Gallery:** ระบบจัดเก็บประวัติเรื่องราวอัตโนมัติ สูงสุด 50 รายการ พร้อมระบบติดดาว ⭐ Favorite และปุ่ม 🎴 / 🗂️ Export Card ในแต่ละรายการ
- **📸 Export to Image:** บันทึกเรื่องราวเป็นรูปภาพ 2 สไตล์ — **Long Card** (เต็มเรื่อง) และ **Short Card** (Cinematic โชว์โควทเด็ด) พร้อมแสดง attribution "[username] × [character] story"
- **📱 Universal UI:** รองรับมือถือ, แท็บเล็ต และคอมพิวเตอร์ครบ จัดกึ่งกลางหน้าจออัตโนมัติ พร้อม card design ที่สวยงามทุกแพลตฟอร์ม

---

### 🗃️ ระบบความทรงจำ (Gallery System)

ทุกครั้งที่ Generate เรื่องราวสำเร็จ ระบบจะบันทึกอัตโนมัติลงใน **Universe Gallery** โดยมีกลไกดังนี้:

| รายละเอียด               | ค่า                                                            |
| ----------------------- | ------------------------------------------------------------- |
| จำนวนสูงสุดที่เก็บได้          | **50 รายการ**                                                 |
| เมื่อเกินขีดจำกัด             | ลบรายการ **เก่าสุดที่ไม่ได้ติดดาว** ออก 1 รายการ                     |
| รายการที่ติดดาว ⭐ Favorite | **ไม่ถูกลบโดยอัตโนมัติเด็ดขาด** แม้จะเกิน 50 รายการ                   |
| การเก็บข้อมูล              | บันทึกใน SillyTavern Settings (ถาวรตราบที่ไม่ Clear หรือ Uninstall) |

**สรุปสั้นๆ:** ติดดาว ⭐ ไว้เรื่องไหนที่ชอบ มันจะไม่หายไปเอง มีแค่เรื่องที่ไม่ได้ติดดาวเท่านั้นที่จะถูกดันออกเมื่อมีเรื่องใหม่เข้ามา

---

### 🛠️ การติดตั้ง (Installation)

1. คัดลอกโฟลเดอร์ `another-universe`
2. นำไปวางในโฟลเดอร์ของ SillyTavern:

   ```
   SillyTavern/public/scripts/extensions/third-party/another-universe
   ```

3. รีสตาร์ทหรือรีเฟรชหน้าต่าง SillyTavern (F5)
4. เปิดแผง Extensions และติ๊กถูกที่ช่อง `Enabled` ข้าง **Another Universe**
5. (ออปชัน) เลือกภาษา UI: `Auto` / `🇹🇭 ไทย` / `🇬🇧 English`

---

### 💡 วิธีการใช้งาน (Usage)

1. กดปุ่ม **`🌌`** ในเมนูแชท (อยู่เหนือ Author Note) เพื่อเปิดหน้าตั้งค่าด่วน
2. เลือกรูปแบบตามต้องการ:
   - **Theme:** โลกแบบไหน (ไซเบอร์พังค์, แฟนตาซียุคกลาง, ฯลฯ)
   - **Encounter:** สถานการณ์การพบกัน (เจอกันครั้งแรก, ศัตรู, คู่แข่ง, สลับร่าง, ฯลฯ)
   - **Mood:** โทนอารมณ์ (โรแมนติก, ปวดตับ, เร่าร้อน, ยันเดเระ, ฯลฯ)
   - เลือก **"❌ ไม่ระบุ"** เพื่อปล่อยให้ AI สุ่มเอง หรือ **"🎨 กำหนดเอง"** เพื่อบรรยายในแบบของคุณเอง (มีกล่องข้อความให้กรอกท้ายตัวเลือก)
3. กดปุ่ม **✨ Generate** แล้วรอรับเรื่องราวในโลกคู่ขนาน
4. ในหน้าจอเรื่องราว จะมีปุ่มให้เลือก:
   - **📸 Long / Short Card** — บันทึกเรื่องเป็นรูปภาพ
   - **🎴 Export PNG Card** — Character Card V2 PNG พร้อมลากเข้า SillyTavern
   - **🗂️ Export JSON** — Character Card V2 JSON สำหรับ tool อื่นๆ หรือเป็น fallback
   - **✏️ Edit / 🔄 Generate** — แก้เนื้อเรื่องด้วยตัวเองหรือสุ่มใหม่
5. กดปุ่ม **📚 Gallery** เพื่อดูเรื่องราวเก่าทั้งหมด แต่ละรายการมีปุ่ม ⭐ / 🎴 / 🗂️ / 🗑️ ให้กดได้

---

### 🔧 ติดต่อสอบถาม

หากพบปัญหาในการใช้งาน หรืออยากเสนอธีมโลกใหม่ๆ สามารถติดต่อได้ที่:

**Discord: majesty.pop (POPKO)**

---

### 📜 License & Terms of Use

Extension นี้ใช้ **Custom License** ดูรายละเอียดเต็มที่ไฟล์ [LICENSE](./LICENSE)

> [!WARNING]
> **สำคัญมาก (CRITICAL):**
> โปรเจกต์นี้สร้างขึ้นเพื่อแบ่งปันให้คอมมูนิตี้ใช้งานฟรี
>
> 1. ✅ **อนุญาต:** Fork / ดัดแปลง / พัฒนาต่อ เพื่อแจกจ่ายคืนคอมมูนิตี้
> 2. ❌ **ห้าม:** นำไปใช้เชิงพาณิชย์หรือแสวงหากำไรทุกรูปแบบ
> 3. ❌ **ห้าม:** ปิดซอร์สโค้ด หรือดัดแปลงเพื่อจำหน่าย
> 4. ⚠️ **ต้อง:** ให้เครดิตว่ามาจาก Another Universe โดย POPUKO
>
> *หากพบเห็นผู้ใดฝ่าฝืน จะดำเนินการแจ้งกับทุกคอมมูนิตี้ที่เกี่ยวข้องทันที*

---

<a id="-english"></a>

## 🇬🇧 English

*"If two characters met in a different world, would their story still be the same?"*

**Another Universe** is an Extension for [SillyTavern](https://github.com/SillyTavern/SillyTavern) that takes your characters across dimensions into parallel worlds. It reinterprets the existing personalities, relationships, and tones through different scenarios and moods every time you press Generate.

> 💡 **Bilingual (TH / EN):** The extension auto-detects SillyTavern's language and switches the entire UI accordingly. You can also pick the language manually in the Extensions panel.

---

### ✨ Features

- **🎭 150,000+ possibilities:** Mix 51 world themes × 53 encounter types × 54 mood tones, or let the AI choose everything randomly.
- **🎨 Custom Theme / Encounter / Mood:** Want a world entirely your own? Pick `🎨 Custom` for any field and describe the world / encounter / mood directly (up to 1,000 characters per field). Your description is injected into the prompt as a high-priority block wrapped in an anti-injection delimiter. Mix and match preset and custom across all three fields freely.
- **🎴 Export Character Card:** Turn any generated story into a SillyTavern character card. Two formats:
  - **🎴 PNG Card** — Character Card V2 PNG (drag-drop into SillyTavern; embedded via tEXt chunk + base64).
  - **🗂️ JSON** — Plain Character Card V2 JSON (portable for TavernAI / RisuAI / JanitorAI, or as a fallback if the PNG path doesn't work for you).
  - The generated story becomes `first_mes` automatically (with auto `{{user}}` / `{{char}}` placeholder replacement). `scenario` combines theme + encounter + mood. avatar / description / personality / mes_example / creator are pulled from the source character.
- **🌐 Multilingual (TH / EN):** Every UI string switches with the locale, including all 158 dropdown labels. Language choice is `Auto` / `🇹🇭 ไทย` / `🇬🇧 English` in the Extensions panel.
- **🤯 Wild themes:** Thai Drama, Thai Mythology, Kemono, Prehistoric, Wuxia / Cultivation, Zombie, Mafia, Vampire, Virtual World, Time Loop, Wild West, Space Opera, Detective Noir, Samurai, Casino, Lighthouse, and many more.
- **🔥 Dark & Spicy:** Yandere, Gore, Body Swap, Fake Dating, Arranged Marriage, Ghost × Human, Demon Pact, Hostage, Auction, Bounty Hunter, etc.
- **🎨 Period-appropriate language:** The system adjusts language and pronouns to match the era (e.g. Medieval uses thee/thou, Thai uses respectful pronouns, Japanese uses honorifics).
- **⚡ Quick Settings:** Click the `🌌` button in the chat menu (above Author Note) to open quick settings — pick a theme and Generate instantly.
- **📚 Universe Gallery:** Auto-saves every generated story (up to 50). Pin favorites with ⭐ and export each entry as PNG / JSON.
- **📸 Export to Image:** Save stories as 2 styles of image — **Long Card** (full story) and **Short Card** (cinematic with featured quote). Includes "[username] × [character] story" attribution.
- **📱 Universal UI:** Works on mobile, tablet, and desktop. Auto-centered, beautiful card design on every platform.

---

### 🗃️ Gallery System

Every successful generation is automatically saved to the **Universe Gallery** with these rules:

| Detail              | Value                                                              |
| ------------------- | ------------------------------------------------------------------ |
| Max entries         | **50**                                                             |
| When over the limit | Removes the **oldest non-favorited** entry (1 at a time)           |
| ⭐ Favorited entries | **Never auto-deleted**, even past 50                               |
| Storage             | SillyTavern Settings (persistent until you Clear All or Uninstall) |

**TL;DR:** Star ⭐ the stories you love and they're safe forever. Only un-starred entries get pushed out as new ones come in.

---

### 🛠️ Installation

1. Copy the `another-universe` folder.
2. Place it inside your SillyTavern folder:

   ```
   SillyTavern/public/scripts/extensions/third-party/another-universe
   ```

3. Restart or refresh the SillyTavern window (F5).
4. Open the Extensions panel and tick the `Enabled` checkbox next to **Another Universe**.
5. (Optional) Pick the UI language: `Auto` / `🇹🇭 ไทย` / `🇬🇧 English`.

---

### 💡 Usage

1. Click the **`🌌`** button in the chat menu (above Author Note) to open quick settings.
2. Pick what you want:
   - **Theme:** What kind of world (Cyberpunk, Medieval Fantasy, etc.)
   - **Encounter:** How they meet (First Meeting, Rivals, Body Swap, etc.)
   - **Mood:** Emotional tone (Romantic, Angsty, Passionate, Yandere, etc.)
   - Pick **"❌ Unspecified"** to let the AI decide freely, or **"🎨 Custom"** to write your own description (a textarea appears below the dropdowns).
3. Click **✨ Generate** and wait for your parallel universe story.
4. On the story view you'll find:
   - **📸 Long / Short Card** — save the story as an image.
   - **🎴 Export PNG Card** — Character Card V2 PNG, drag straight into SillyTavern.
   - **🗂️ Export JSON** — Character Card V2 JSON, for other tools or as a fallback.
   - **✏️ Edit / 🔄 Generate** — manually edit the story or roll a new one.
5. Click **📚 Gallery** to browse past stories. Each item has ⭐ / 🎴 / 🗂️ / 🗑️ buttons.

---

### 🔧 Contact

For bugs, feature requests, or new theme suggestions:

**Discord: majesty.pop (POPKO)**

---

### 📜 License & Terms of Use

This Extension uses a **Custom License**. See the full terms in the [LICENSE](./LICENSE) file.

> [!WARNING]
> **CRITICAL:**
> This project was created to be shared freely with the community.
>
> 1. ✅ **Allowed:** Fork / modify / develop further to share back with the community
> 2. ❌ **Forbidden:** Any commercial or for-profit use
> 3. ❌ **Forbidden:** Closing the source or selling derivatives
> 4. ⚠️ **Required:** Credit Another Universe by POPUKO
>
> *Any violations will be reported to all relevant communities immediately.*

---

## 🌌 Inspiration

*"Do you think we're best friends in other universes too?"*

![Inspiration](./inspiration.jpg)

---
*Created with magic and curiosity. ✨*
