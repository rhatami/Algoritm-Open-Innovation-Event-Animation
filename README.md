<a id="fa"></a>

<div dir="rtl">

# انیمیشن هوش مصنوعی — Algoritm Open Innovation

[🇮🇷 نسخه‌ی فارسی ↑](#fa)

> یک انیمیشن موزیکال که از ابتدا تا انتها با کمک هوش مصنوعی برای رویداد **Algoritm Open Innovation** ساخته شد؛ رویدادی برای جذب ایده‌های نوآورانه در حوزه‌ی فین‌تک.
> این مخزن کل مسیر ساخت را مستند می‌کند: پرامپت‌ها، آزمون‌وخطاها و خروجی‌های نهایی؛ تا دیگران هم بتوانند از آن یاد بگیرند و آن را بازتولید کنند.

## 🎬 انیمیشن نهایی

▶️ **[مشاهده‌ی ویدیوی نهایی](06-final-assets/04-edit/Final-Video.mp4)**

🎵 [موسیقی نهایی (MP3)](06-final-assets/01-music/Final-Music.mp3)

همه‌ی خروجی‌های نهایی در پوشه‌ی [`06-final-assets/`](06-final-assets/) قرار دارند.

**داستان:** پسربچه‌ای که آرزوی سفر به ماه دارد، یک بذر جادویی می‌کارد، درباره‌ی رشد آن مطالعه می‌کند، در آکادمی بانکداری هوشمند آموزش می‌بیند و از درخت مراقبت می‌کند تا درخت به ماه برسد. درخت استعاره‌ای از یک **ایده** است که رشد می‌کند و به محصول و استارتاپ تبدیل می‌شود.

---

## 📌 خلاصه‌ی پروژه

| | |
|---|---|
| پروژه | انیمیشن هوش مصنوعی Algoritm Open Innovation |
| زمینه | فین‌تک / نوآوری باز |
| تجربه | اولین پروژه‌ی جدی انیمیشن با هوش مصنوعی |
| مدت انیمیشن | حدود ۲ دقیقه (۱۶ صحنه) |
| زمان تولید | حدود ۵ ساعت |
| بازه‌ی تولید | ۲۱:۳۰ تا ۰۲:۳۰ |
| هزینه‌ی کل | حدود ۱۷ دلار |
| دسترسی به مدل‌ها | Matis |
| تدوین | Shotcut |

---

## 🧠 روند کار

```text
Event Brief
    ↓
ChatGPT + Claude
    ↓
Lyrics & Creative Direction
    ↓
Human Refinement
    ↓
Pronunciation tuning (diacritics)
    ↓
Suno 4.5  →  Final Music
    ↓
Storyboard + Timing
    ↓
GPT Image 2  →  Keyframes / Scene Images
    ↓
Kling 2.5 Turbo Pro  →  Video Clips
    ↓
Shotcut  →  Final Animation
```

## 🛠️ ابزارها

| مرحله | ابزار | کاربرد |
|---|---|---|
| ایده‌پردازی / نوشتن | ChatGPT | ایده، شعر، طراحی استوری‌بورد و پرامپت |
| ایده‌پردازی / نوشتن | Claude | اصلاح شعر، رفع مشکل تلفظ، پرامپت استایل Suno |
| موسیقی | Suno V4.5 (‏Custom Mode، ‏105 BPM) | تولید موسیقی |
| تولید تصویر | GPT Image 2 | تولید تصویر هر صحنه (Keyframe) |
| تصویر به ویدیو | Kling AI 2.5 Turbo Pro | ساخت انیمیشن |
| تدوین | Shotcut | تدوین نهایی |
| دسترسی به مدل‌ها | Matis | دسترسی یکپارچه به چند مدل |

---

## 📁 ساختار مخزن

```text
01-lyrics/             Lyrics: from event brief to final diacritized version
02-music-generation/   Suno prompt, style prompt and settings
03-storyboard/         Scene-breakdown prompt and audio/scene timing
04-image-generation/   16 image prompts (GPT Image 2)
05-video-generation/   16 image-to-video prompts (Kling 2.5 Turbo Pro)
06-final-assets/       Final outputs
  ├── 01- music/       Final music (MP3)
  ├── 02- images/      Selected scene images
  ├── 03- videos/      Generated video clips
  └── 04- edit/        Shotcut project + Final Video.mp4
```

---

## 🪜 مراحل ساخت

### ۱. شعر — [`01-lyrics/`](01-lyrics/00-README.md)

توضیحات رویداد به یک ترانه‌ی انگیزشی تبدیل شد که بشود آن را به صحنه‌های انیمیشن نگاشت کرد. مسیر کار: پیش‌نویس با ChatGPT ← کوتاه‌سازی برای حدود یک دقیقه شعر ← بازنویسی انسانی ← اعراب‌گذاری برای رفع مشکل تلفظ Suno ← نسخه‌ی نهایی.

| فایل | توضیح |
|---|---|
| [`01-original-lyric.md`](01-lyrics/01-original-lyric.md) | توضیحات رویداد، پرامپت اولیه و اولین شعر تولیدشده |
| [`02-enhance-lyric.md`](01-lyrics/02-enhance-lyric.md) | کوتاه‌سازی شعر برای ویدیوی حدود یک دقیقه‌ای |
| [`03-final-lyric.md`](01-lyrics/03-final-lyric.md) | نسخه‌ی نهایی شعر که با دست ویرایش شد |
| [`04-lyrics-diacritics.md`](01-lyrics/04-lyrics-diacritics.md) | اولین دور اعراب‌گذاری کامل برای Suno 4.5 |
| [`05-enhance-lyric-diacritics.md`](01-lyrics/05-enhance-lyric-diacritics.md) | عیب‌یابی تلفظ با ChatGPT و Claude |
| [`06-final-lyrics-diacritics.md`](01-lyrics/06-final-lyrics-diacritics.md) | شعر نهایی اعراب‌گذاری‌شده |

### ۲. تولید موسیقی — [`02-music-generation/`](02-music-generation/README.md)

| فایل | توضیح |
|---|---|
| [`style-prompt.md`](02-music-generation/01-claude-prompt.md) | گفت‌وگو با Claude برای پیشنهاد Style Prompt |
| [`suno-prompt.md`](02-music-generation/02-suno-prompt.md) | شعر نهایی و Style Prompt واردشده در Suno |

تنظیمات: **Suno V4.5 ‏· Custom Mode ‏· 105 BPM**. موسیقی نهایی در [`06-final-assets/01- music/`](06-final-assets/01-music/) قرار دارد.

### ۳. استوری‌بورد و زمان‌بندی — [`03-storyboard/`](03-storyboard/)

| فایل | توضیح |
|---|---|
| [`01-scene-breakdown-prompt.md`](03-storyboard/01-scene-breakdown-prompt.md) | پرامپت ChatGPT: شعر + زمان‌ها + ایده‌ی داستان ← ۱۶ صحنه |
| [`02-timing.md`](03-storyboard/02-timing.md) | زمان‌بندی نهایی صحنه‌ها بر اساس آهنگ ساخته‌شده (۰۲:۰۲) |

### ۴. تولید تصویر — [`04-image-generation/`](04-image-generation/)

برای هر صحنه یک پرامپت برای **GPT Image 2** نوشته شد. در همه‌ی پرامپت‌ها توضیح شخصیت، مکان و سبک تکرار شده تا پسر، خانه و درخت در ۱۶ تصویر یکدست بمانند. در صحنه‌های ۷ و ۸ لوگوی آکادمی بانکداری هوشمند هم به‌عنوان تصویر مرجع به مدل داده شد.

### ۵. تولید ویدیو — [`05-video-generation/`](05-video-generation/)

برای هر صحنه یک پرامپت برای **Kling AI 2.5 Turbo Pro** نوشته شد که تصویر همان صحنه را به‌عنوان تصویر مرجع می‌گیرد. هر پرامپت حرکت ظریف شخصیت و دوربین را توصیف می‌کند و با فهرست محدودیت‌هایی مثل «بدون مورف، بدون شخصیت جدید، بدون متن» تمام می‌شود.

### ۶. خروجی‌های نهایی — [`06-final-assets/`](06-final-assets/)

موسیقی، تصاویر منتخب، کلیپ‌های ویدیویی و تدوین نهایی (در **Shotcut** و بر اساس موسیقی).

---

## 🎞️ نقشه‌ی صحنه‌ها

| # | زمان | اتفاق صحنه | پرامپت تصویر | پرامپت ویدیو |
|--:|---|---|---|---|
| 01 | 0:00–0:07 | پسر به ماه خیره می‌شود | [تصویر](04-image-generation/scene-01.md) | [ویدیو](05-video-generation/scene-01.md) |
| 02 | 0:07–0:13 | مطالعه و طراحی؛ جست‌وجوی راهی برای رسیدن به ماه | [تصویر](04-image-generation/scene-02.md) | [ویدیو](05-video-generation/scene-02.md) |
| 03 | 0:13–0:25 | جرقه‌ی ایده ← پیدا کردن بذر | [تصویر](04-image-generation/scene-03.md) | [ویدیو](05-video-generation/scene-03.md) |
| 04 | 0:25–0:32 | کاشتن بذر | [تصویر](04-image-generation/scene-04.md) | [ویدیو](05-video-generation/scene-04.md) |
| 05 | 0:32–0:40 | اولین جوانه | [تصویر](04-image-generation/scene-05.md) | [ویدیو](05-video-generation/scene-05.md) |
| 06 | 0:40–0:46 | مطالعه درباره‌ی رشد درخت | [تصویر](04-image-generation/scene-06.md) | [ویدیو](05-video-generation/scene-06.md) |
| 07 | 0:46–0:51 | ورود به آکادمی بانکداری هوشمند | [تصویر](04-image-generation/scene-07.md) | [ویدیو](05-video-generation/scene-07.md) |
| 08 | 0:51–0:57 | یادگیری در آکادمی | [تصویر](04-image-generation/scene-08.md) | [ویدیو](05-video-generation/scene-08.md) |
| 09 | 0:57–1:05 | بازگشت به خانه و مراقبت از درخت | [تصویر](04-image-generation/scene-09.md) | [ویدیو](05-video-generation/scene-09.md) |
| 10 | 1:05–1:15 | رشد محسوس درخت | [تصویر](04-image-generation/scene-10.md) | [ویدیو](05-video-generation/scene-10.md) |
| 11 | 1:15–1:25 | تماشای درخت در حال رشد از پشت پنجره | [تصویر](04-image-generation/scene-11.md) | [ویدیو](05-video-generation/scene-11.md) |
| 12 | 1:25–1:35 | پنجره‌ی خالی در شب؛ گذر زمان | [تصویر](04-image-generation/scene-12.md) | [ویدیو](05-video-generation/scene-12.md) |
| 13 | 1:35–1:45 | درخت از خانه بلندتر می‌شود | [تصویر](04-image-generation/scene-13.md) | [ویدیو](05-video-generation/scene-13.md) |
| 14 | 1:45–1:53 | درخت به ستاره‌ها می‌رسد | [تصویر](04-image-generation/scene-14.md) | [ویدیو](05-video-generation/scene-14.md) |
| 15 | 1:53–1:57 | درخت به ماه می‌رسد | [تصویر](04-image-generation/scene-15.md) | [ویدیو](05-video-generation/scene-15.md) |
| 16 | 1:57–2:00 | پسر شروع به بالا رفتن به سمت ماه می‌کند | [تصویر](04-image-generation/scene-16.md) | [ویدیو](05-video-generation/scene-16.md) |

---

## 🔁 اصل اصلی: تکرار و اصلاح

این پروژه فقط «پرامپت ← تولید ← تمام» نبود. روند واقعی بیشتر این‌طور بود:

`تولید ← ارزیابی ← اصلاح ← تولید دوباره ← انتخاب`

نمونه‌ها:

- در اولین تولید موسیقی، تلفظ فارسی مشکل داشت؛ پس شعر اصلاح و اعراب‌گذاری شد (فایل‌های `01-lyrics/04` تا `06`).
- بعضی تصویرها رد و دوباره تولید شدند.
- بعضی کلیپ‌های ویدیویی در تدوین نهایی استفاده نشدند.
- انتخاب نهایی صحنه‌ها بر اساس موسیقی و ریتم کلی انجام شد.

---

## 📊 آمار پروژه

- زمان تولید: حدود ۵ ساعت
- هزینه‌ی کل: حدود ۱۷ دلار
- تعداد صحنه‌های نهایی: ۱۶
- موسیقی نهایی: ۱ قطعه (۲:۰۲)

---

## 🚀 اگر می‌خواهی چیزی شبیه این بسازی

1. با یک بریف خلاقانه‌ی روشن شروع کن.
2. قبل از تولید دارایی‌ها، داستان و زبان بصری را مشخص کن.
3. موسیقی را **قبل از** قفل‌کردن زمان‌بندی صحنه‌ها بساز و اصلاح کن.
4. استوری‌بورد را بر اساس خط زمانی واقعی آهنگ بنویس.
5. قواعد یکدستی شخصیت و سبک را در هر پرامپت تصویر تکرار کن.
6. در صورت نیاز از هر صحنه چند کاندید تصویر بساز.
7. تصاویر منتخب را به کلیپ‌های کوتاه ویدیویی تبدیل کن.
8. بر اساس موسیقی تدوین کن؛ همه‌ی کلیپ‌های تولیدشده لزوماً به تدوین نهایی نمی‌رسند.
9. تلاش‌های ناموفق را نگه دار؛ برای یادگرفتن مفیدند.

---

<a id="en"></a>

[🇬🇧 English version ↓](#en)

# AI Animation — Algoritm Open Innovation


> An end-to-end, AI-assisted animated music video created for **Algoritm Open Innovation**, an event focused on attracting innovative ideas in fintech.
> This repository documents the whole process — prompts, iterations and final assets — so others can learn from it and reproduce it.

## 🎬 Final Animation

▶️ **[Watch the final video](06-final-assets/04-edit/Final-Video.mp4)**

🎵 [Final music (MP3)](06-final-assets/01-music/Final-Music.mp3)

All final outputs live in [`06-final-assets/`](06-final-assets/).

**The story:** a boy who dreams of traveling to the moon plants a magical seed, studies how to make it grow, learns at the Smart Banking Academy and cares for the tree until it reaches the moon. The tree is a metaphor for an **idea** that grows into a product and a startup.

---

## 📌 Project Snapshot

| | |
|---|---|
| Project | Algoritm Open Innovation AI Animation |
| Context | Fintech / Open Innovation |
| Experience | First serious AI animation project |
| Length | ~2 minutes (16 scenes) |
| Production time | ~5 hours |
| Production window | 21:30 – 02:30 |
| Total cost | ~$17 |
| Model access | Matis |
| Editing | Shotcut |

---

## 🧠 The Workflow

```text
Event Brief
    ↓
ChatGPT + Claude
    ↓
Lyrics & Creative Direction
    ↓
Human Refinement
    ↓
Pronunciation tuning (diacritics)
    ↓
Suno 4.5  →  Final Music
    ↓
Storyboard + Timing
    ↓
GPT Image 2  →  Keyframes / Scene Images
    ↓
Kling 2.5 Turbo Pro  →  Video Clips
    ↓
Shotcut  →  Final Animation
```

## 🛠️ Tools

| Stage | Tool | Purpose |
|---|---|---|
| Ideation / writing | ChatGPT | Ideas, lyrics, storyboard and prompt design |
| Ideation / writing | Claude | Lyrics refinement, pronunciation tuning, Suno style prompt |
| Music | Suno V4.5 (Custom Mode, 105 BPM) | Music generation |
| Image generation | GPT Image 2 | Scene / keyframe generation |
| Image-to-video | Kling AI 2.5 Turbo Pro | Animation |
| Editing | Shotcut | Final edit |
| Model access | Matis | Unified access to multiple models |

---

## 📁 Repository Structure

```text
01-lyrics/             Lyrics: from event brief to final diacritized version
02-music-generation/   Suno prompt, style prompt and settings
03-storyboard/         Scene-breakdown prompt and audio/scene timing
04-image-generation/   16 image prompts (GPT Image 2)
05-video-generation/   16 image-to-video prompts (Kling 2.5 Turbo Pro)
06-final-assets/       Final outputs
  ├── 01- music/       Final music (MP3)
  ├── 02- images/      Selected scene images
  ├── 03- videos/      Generated video clips
  └── 04- edit/        Shotcut project + Final Video.mp4
```

---

## 🪜 Step-by-Step

### 1. Lyrics — [`01-lyrics/`](01-lyrics/00-README.md)

The event description was turned into a motivational song that can be mapped to animation scenes. Process: draft with ChatGPT → shorten to ~1 minute of lyrics → human rewrite → add Persian diacritics to fix Suno's pronunciation problems → final version.

| File | What it is |
|---|---|
| [`01-original-lyric.md`](01-lyrics/01-original-lyric.md) | Event description, first prompt and first generated lyrics |
| [`02-enhance-lyric.md`](01-lyrics/02-enhance-lyric.md) | Shortening the lyrics for a ~1-minute video |
| [`03-final-lyric.md`](01-lyrics/03-final-lyric.md) | Hand-edited final lyrics |
| [`04-lyrics-diacritics.md`](01-lyrics/04-lyrics-diacritics.md) | First full diacritization pass for Suno 4.5 |
| [`05-enhance-lyric-diacritics.md`](01-lyrics/05-enhance-lyric-diacritics.md) | Pronunciation debugging with ChatGPT and Claude |
| [`06-final-lyrics-diacritics.md`](01-lyrics/06-final-lyrics-diacritics.md) | Final diacritized lyrics |

### 2. Music Generation — [`02-music-generation/`](02-music-generation/README.md)

| File | What it is |
|---|---|
| [`style-prompt.md`](02-music-generation/01-claude-prompt.md) | Asking Claude for a Suno style prompt |
| [`suno-prompt.md`](02-music-generation/02-suno-prompt.md) | Final lyrics + style prompt entered into Suno |

Settings: **Suno V4.5 · Custom Mode · 105 BPM**. The final track is in [`06-final-assets/01- music/`](06-final-assets/01-music/).

### 3. Storyboard & Timing — [`03-storyboard/`](03-storyboard/)

| File | What it is |
|---|---|
| [`01-scene-breakdown-prompt.md`](03-storyboard/01-scene-breakdown-prompt.md) | The ChatGPT prompt: lyrics + timestamps + story idea → 16 scenes |
| [`02-timing.md`](03-storyboard/02-timing.md) | Final scene timing, aligned to the finished song (02:02) |

### 4. Image Generation — [`04-image-generation/`](04-image-generation/)

One prompt per scene for **GPT Image 2**. Every prompt repeats the same character, location and style description to keep the boy, the house and the tree consistent across all 16 images. Scenes 07 and 08 also use the supplied Smart Banking Academy logo as a reference image.

### 5. Video Generation — [`05-video-generation/`](05-video-generation/)

One prompt per scene for **Kling AI 2.5 Turbo Pro**, using the matching scene image as the reference image. Each prompt describes subtle motion plus camera movement, and ends with a strict "no morphing / no new characters / no text" list.

### 6. Final Assets — [`06-final-assets/`](06-final-assets/)

Music, selected images, generated clips and the final edit (assembled in **Shotcut** against the music).

---

## 🎞️ Scene Map

| # | Time | What happens | Image prompt | Video prompt |
|--:|---|---|---|---|
| 01 | 0:00–0:07 | Boy looks at the moon | [Image](04-image-generation/scene-01.md) | [Video](05-video-generation/scene-01.md) |
| 02 | 0:07–0:13 | He studies and draws, searching for a way | [Image](04-image-generation/scene-02.md) | [Video](05-video-generation/scene-02.md) |
| 03 | 0:13–0:25 | Idea spark → discovers the seed | [Image](04-image-generation/scene-03.md) | [Video](05-video-generation/scene-03.md) |
| 04 | 0:25–0:32 | Plants the seed | [Image](04-image-generation/scene-04.md) | [Video](05-video-generation/scene-04.md) |
| 05 | 0:32–0:40 | First sprout appears | [Image](04-image-generation/scene-05.md) | [Video](05-video-generation/scene-05.md) |
| 06 | 0:40–0:46 | Studies how to grow it | [Image](04-image-generation/scene-06.md) | [Video](05-video-generation/scene-06.md) |
| 07 | 0:46–0:51 | Enters the Smart Banking Academy | [Image](04-image-generation/scene-07.md) | [Video](05-video-generation/scene-07.md) |
| 08 | 0:51–0:57 | Learns from the academy | [Image](04-image-generation/scene-08.md) | [Video](05-video-generation/scene-08.md) |
| 09 | 0:57–1:05 | Returns home and cares for the tree | [Image](04-image-generation/scene-09.md) | [Video](05-video-generation/scene-09.md) |
| 10 | 1:05–1:15 | Tree grows noticeably | [Image](04-image-generation/scene-10.md) | [Video](05-video-generation/scene-10.md) |
| 11 | 1:15–1:25 | Boy watches the growing tree | [Image](04-image-generation/scene-11.md) | [Video](05-video-generation/scene-11.md) |
| 12 | 1:25–1:35 | Empty window / night / time passing | [Image](04-image-generation/scene-12.md) | [Video](05-video-generation/scene-12.md) |
| 13 | 1:35–1:45 | Tree rises above the house | [Image](04-image-generation/scene-13.md) | [Video](05-video-generation/scene-13.md) |
| 14 | 1:45–1:53 | Tree reaches into the stars | [Image](04-image-generation/scene-14.md) | [Video](05-video-generation/scene-14.md) |
| 15 | 1:53–1:57 | Tree touches the moon | [Image](04-image-generation/scene-15.md) | [Video](05-video-generation/scene-15.md) |
| 16 | 1:57–2:00 | Boy begins climbing toward the moon | [Image](04-image-generation/scene-16.md) | [Video](05-video-generation/scene-16.md) |

---

## 🔁 The Core Principle: Iterate

This was not a `Prompt → Generate → Done` workflow. It was closer to:

`Generate → Evaluate → Refine → Regenerate → Select`

Examples:

- Initial music generation had Persian pronunciation issues, so the lyrics were refined and diacritics were added (see `01-lyrics/04` to `06`).
- Some image generations were rejected and regenerated.
- Some video clips were not used in the final edit.
- Final scene selection was driven by the music and the overall rhythm.

---

## 📊 Project Stats

- Production time: ~5 hours
- Total cost: ~$17
- Final scenes: 16
- Final music tracks: 1 (2:02)

---

## 🚀 Reproduce / Learn From This Project

1. Start with a clear creative brief.
2. Define the story and visual language before generating assets.
3. Generate and refine the music **before** locking scene timing.
4. Create the storyboard from the actual audio timeline.
5. Repeat character and visual-consistency rules in every image prompt.
6. Generate multiple image candidates where necessary.
7. Turn the selected images into short video clips.
8. Edit against the music — not every generated clip belongs in the final cut.
9. Keep failed attempts; they are useful for learning.

---

## 📜 Credits

Project concept / creative direction / editing: **Rouhollah Hatami Bahabadi**

Event: **Algoritm Open Innovation**

Tools: ChatGPT · Claude · Suno · GPT Image 2 · Kling 2.5 Turbo Pro · Shotcut · Matis
