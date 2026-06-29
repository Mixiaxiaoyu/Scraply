---
name: scraply
description: Scraply (拾页) generates finished paper scrapbook / journaling collage images from uploaded photos. Default to a stable "perfect classic" open-notebook travel-journal style with clean blue cutting mat, white-border printed photos, cobalt marker title, stickers, tickets, and light clips. Use rich-random mode only when the user includes @S, adding more varied notebook bodies, charms, covers, tabs, paperclips, and accessories. Use when the user asks to make uploaded images into a shouzhang / hand journal, scrapbook, collage diary, sticker journal, travel journal, planner spread, or handmade photo journal image.
---

# Scraply / 拾页

Turn uploaded photos into one polished scrapbook image with the built-in image generation tool. Treat user photos as printed inserts inside the scrapbook, not just mood references. Use every uploaded photo unless the user explicitly allows omission.

Default to the stable "perfect classic" result: realistic open notebook / double-page spread on a clean blue cutting mat, cream grid paper, white-border printed photos, chunky cobalt-blue marker title, theme-matched stickers, tickets, washi tape, one or two clips, and balanced blank space. Use rich-random notebook-body variation only when the user's request includes `@S`. Use a single loose sheet only when the user asks for it.

Do not wait for the user to upload sticker references. Infer the scrapbook theme from the photos and automatically create stickers that echo the visible subjects, place, mood, and activity.

## Mode Switch

- Default mode: if the user does not include `@S`, generate the "perfect classic" style. Keep the notebook body stable and clean: open cream grid notebook, blue cutting mat, simple spine/cover edge, one binder clip or paperclip, optional pen, tickets, labels, and white-border stickers. Do not over-randomize covers, charms, tabs, straps, or accessories.
- Rich-random mode: if the user includes `@S`, enable richer physical notebook variation: clear cover, ring binder edge, elastic strap, metal clips, dangling charms, paperclips, tab dividers, bookmark ribbons, pen loops, transparent pockets, or small attached ephemera.
- Treat `@S` as a control command only. Never render `@S` as visible text in the image.

## Workflow

1. Collect all image attachments in the current user request. If the newest image is only a screenshot showing a group of previous photos, use the actual source photos from the conversation and do not include the chat UI screenshot as a scrapbook insert.
2. Count the user photos and plan how every photo will appear:
   - 1 photo: one hero printed photo with generous blank paper.
   - 2-4 photos: one hero photo plus supporting inserts in an open notebook spread.
   - 5-8 photos: double-page spread with 2-3 larger photos and the rest as mini prints, film frames, ticket scraps, or small clipped inserts.
   - 9+ photos: clean high-density spread with contact-sheet or film-strip groups; do not intentionally omit photos.
3. Choose one randomized page-role split:
   - photo-heavy left page + notes/stickers right page
   - photo-heavy right page + notes/stickers left page
   - one hero-photo page + one clean text-and-sticker page
   - film-strip page + handwritten memory page
   - ticket-pocket page + simple photo feature page
   - mostly blank doodle/silhouette page + tidy collage page
4. Choose one randomized title placement. Do not default to left-side titles:
   - top-left area of the left page
   - top-right area of the right page
   - centered across the upper middle of the spread
   - slightly crossing the spine near the top
   - above the hero photo on the photo-heavy page
   - on the cleaner text-and-sticker page with supporting doodles around it
   - Title placement should respond to the page-role split and available blank space, while staying readable and balanced.
5. Choose the notebook-body mode:
   - Default mode: use the perfect classic notebook body: open cream grid notebook, blue cutting mat, subtle cover edge, one binder clip or paperclip, one pen or ticket tag when useful. Keep the body elegant and familiar, close to the reference-style successful result.
   - Rich-random mode (`@S`): choose one randomized notebook-body style and make the physical journal visibly different between generations:
     - clear PVC cover with rounded corners, faint reflections, and colored side tabs
     - spiral or ring-bound notebook with two or three visible metal rings
     - cream traveler's notebook with a vertical elastic band and bookmark ribbon
     - binder journal with a large metal binder clip on one side
     - soft planner with stitched edge, pen loop, and snap strap
     - transparent cover sleeve with tucked ticket scraps and label tabs
     - grid-paper notebook on a cutting mat with a ruler edge and small clips
     - scrapbook album with thick rounded pages and tiny corner protectors
6. Add physical accessories according to the mode:
   - Default mode: add only 1-3 restrained accessories such as one binder clip, one paperclip, a blue pen, a ticket tag, washi tape, or a kraft label. Keep accessories secondary so the clean classic composition stays dominant.
   - Rich-random mode (`@S`): add 2-5 randomized physical accessories around or attached to the notebook. Choose from dangling camera/star/heart/flower charms, brass keyring charms, binder clips, mini bulldog clips, paperclips, shaped clips, clothespins, ribbon bookmark tails, elastic strap, page tabs, corner protectors, sticker flakes, washi tape rolls, pen, date stamp, small scissors, ticket tag, luggage tag, or transparent pocket.
   - Accessories should feel handmade and useful, not like generic decoration.
7. Infer the theme and choose matching sticker motifs. Use the photos, user text, and visible subjects:
   - nature / forest / flowers: botanical cutouts, leaf stickers, flower stickers, tree silhouettes, soft nature labels
   - lake / swan / animal: animal-shaped kiss-cut stickers, water ripples, small habitat icons, gentle speech bubbles
   - city / travel / transport: tickets, maps, route lines, tram/train/bus stickers, luggage tags, location pins
   - hiking / outdoor: boots, backpack, trail signs, mountain stickers, compass/map labels
   - cafe / food: cups, receipts, menu labels, dessert stickers, barcode tags
   - people / portrait: white-border photo cutout figures, outfit/detail stickers, name tags, speech bubbles
   - birthday / party: cake, candles, gift labels, confetti stickers, date badges
   - study / work: stationery stickers, tabs, checklist labels, clips, memo notes
   - fan / pop / playful: merch-style sticker pack, bold word stickers, comic bubbles, barcode/tag stickers
   - Sticker trigger strength matters: for each hero photo, add 2-4 obvious theme-matched sticker or ephemera elements; for each supporting photo, add 1-2 obvious theme-matched sticker or ephemera elements. Across the full spread, aim for at least 6-12 clearly readable theme-linked sticker, label, stamp, or ephemera pieces.
8. Choose one visibly distinct decor system:
   - silhouette stickers: cutout people, objects, plants, landmarks, trees, travel shapes
   - kiss-cut sticker pack: white-border die-cut characters, photo cutout figures, merch-style sticker pieces, small name tags, barcode strips, comic labels, and speech bubbles
   - graphic word stickers: bold outlined phrases, bubble letters, graffiti words, curved labels, and tiny slogan tags
   - mini photo stickers: small polaroid frames, tiny printed snapshots, contact-sheet pieces, or postage-stamp photo stickers
   - hand-drawn doodles: chunky blue marker stars, arrows, flowers, maps, cameras, routes
   - printed sticker pack: cute icons, labels, tabs, calendar stickers, small travel stamps
   - paper ephemera: tickets, receipts, luggage tags, postcards, torn kraft scraps
   - transparent stickers: translucent tape, acetate tabs, faint grid labels
   - tape-and-label system: washi strips, masking tape corners, binder clips, date tabs
9. Generate one finished image. Save or copy the final PNG into a project run folder only when the user needs a persisted file.
10. Show the image and keep the final response short.

## Visual Rules

- Keep the result clean and handmade: visible cream/white/grid paper, medium detail, balanced spacing, no dirty paper, no overfilled clutter.
- Use overhead realistic paper photography. Default mode should look like the proven classic reference: blue cutting mat, open cream grid notebook, white-border photos, cobalt marker writing, stickers, tickets, clips, tape, labels, and a pen.
- In default mode, keep the physical notebook body restrained and stable. Do not force a distinctive cover, ring binding, strap, charm chain, or heavy accessory system.
- In rich-random mode (`@S`), the physical notebook body must have at least one distinctive feature beyond plain pages: visible cover edge, clasp, rings, elastic, bookmark ribbon, tab dividers, clear sleeve, charm chain, clip system, or pen loop.
- Randomize the notebook body and accessories only in rich-random mode. In default mode, keep variation mostly inside layout, stickers, text, photo sizing, tickets, and tape.
- In default mode, keep the page clean but not sparse. Prioritize clearly readable sticker groups over excessive empty paper.
- Sticker triggering should feel strong at first glance: the viewer should immediately read the theme from the sticker system, not only from the photos.
- In rich-random mode (`@S`), increase sticker density and variety beyond the default mode, not only notebook-body richness.
- Randomize the title position each run. Do not keep placing the main title on the left by habit.
- Make the title placement feel intentional: it should use available blank space, avoid covering faces or key subjects, and visually balance the photos, stickers, and tickets.
- Keep charms, clips, and paperclips near page edges, spine, or cover edges so they enrich the object without covering the user photos.
- Use all uploaded photos as recognizable printed photo inserts. Do not add unrelated extra photo subjects.
- When using kiss-cut stickers, make them look like real vinyl sticker pieces: irregular white outlines, slight paper thickness, tiny drop shadows, and separated sticker shapes placed on the page.
- Sticker motifs must connect to the photo theme. For example, nature photos should trigger leaves, flowers, trees, animal cutouts, and soft nature labels; city travel should trigger tickets, maps, location pins, and transit stickers; portraits should trigger white-border cutout figures, small name tags, and speech bubbles.
- If sticker references are supplied, they may influence the sticker language, but the skill should still generate theme-matched stickers automatically when no sticker references exist.
- Do not cover faces or main subjects with stickers, text, or tape.
- Avoid a simple grid, PPT collage, UI card layout, ecommerce collage, glossy 3D, neon glow, or generic album template.
- Avoid repeating the same "photos on both pages evenly" layout. Let the two pages have different roles.

## Text And Date Rules

- Visible text must be Chinese and/or English only unless the user explicitly requests another language.
- Do not generate Japanese text, hiragana, katakana, kana, pseudo-Japanese, or Japanese-style filler labels.
- If any calendar, date stamp, ticket, month label, or planner date appears, use the current invocation date from the task context.
- Use short readable Chinese or English text, such as travel diary titles, memory labels, date labels, and simple route notes.
- Vary the copy every generation. Do not default to the same `TRAVEL DIARY`, `GOOD DAY`, `DAY 1`, `TODAY'S PLAN`, or identical checklist wording unless the user specifically requests those words.
- Build the visible copy from mixed pools:
  - Main title options: `今日小记`, `出发日记`, `风景收集`, `旅途碎片`, `慢慢走`, `夏日存档`, `城市漫游`, `山野来信`, `光影备忘`, `Weekend Notes`, `Little Journey`, `Memory Map`, `Field Notes`, `Soft Adventure`.
  - Label options: `路过这里`, `把风装进口袋`, `这一刻很轻`, `慢一点也很好`, `今天有阳光`, `沿途收集`, `小小坐标`, `值得记住`, `风景暂停`, `此刻保存`, `seen today`, `tiny stop`, `best moment`, `soft pause`, `keep this`.
  - Checklist options: `看云`, `散步`, `拍照`, `喝点热的`, `买票`, `写明信片`, `等风来`, `坐到窗边`, `留一张票根`, `记住颜色`, `walk slow`, `take photos`, `save tickets`, `find coffee`, `look around`.
  - Speech bubble options: `好喜欢这里`, `风刚刚好`, `像走进画里`, `今天很满`, `下次还来`, `太治愈了`, `我们到了`, `小小快乐`, `keep going`, `sweet view`, `good little day`.
  - Date/ticket options: `DATE: {current date}`, `STAMPED {current date}`, `MEMO {current date}`, `ROUTE CARD`, `CITY TICKET`, `FIELD TICKET`, `PHOTO PASS`, `WEEKEND PASS`.
- Combine 5-10 short text pieces total, mixing Chinese and simple English naturally. Keep text sparse and legible; avoid long paragraphs.
- Prefer chunky cobalt-blue marker handwriting: rounded, uneven, playful, bold, like the HIGHTIDE-style reference. Avoid thin digital fonts and long unreadable text blocks.

## Background Rules

- If a cutting mat appears, it must be true overhead / orthographic: square mat edges, straight horizontal/vertical grid lines, parallel to the image borders, evenly spaced.
- Do not allow warped, tilted, curved, bowed, wavy, or perspective-skewed grid lines.
- A clean neutral tabletop is also acceptable.

## Prompt Skeleton

Use this as the core prompt and adapt it to the current images:

```text
Create one finished realistic open-notebook double-page scrapbook spread from the uploaded user photos.
Use every uploaded photo as a recognizable printed photo insert; do not add unrelated extra photo subjects.
Default to a double-page hand-decorated journal, not a single loose sheet.
Mode selection: if the user request includes @S, use rich-random mode; otherwise use default perfect classic mode. Never render @S as visible text.
Default perfect classic mode: clean blue cutting mat, open cream grid notebook, balanced white-border printed photos, chunky cobalt-blue marker title, theme-matched kiss-cut stickers, tickets, washi tape, kraft labels, one or two clips, optional blue pen, readable travel-journal composition, not too many physical notebook accessories.
Rich-random mode only when @S is present: randomize the physical notebook body with clear cover, rings, elastic band, bookmark ribbon, tab dividers, clip system, transparent sleeve, stitched planner edge, or charm chain; add 2-5 realistic edge accessories such as dangling camera/star/heart/flower charms, brass keyrings, binder clips, paperclips, shaped clips, ribbon tails, page tabs, washi tape rolls, pen, ticket tag, or transparent pocket.
Use a randomized page-role split: one page can be photo-heavy while the other is mostly clean handwriting, silhouette stickers, doodles, tickets, labels, and blank paper.
Randomize the main title placement: choose top-left, top-right, upper-center, slightly across the spine, above the hero photo, or on the cleaner text page. Do not default to a left-side title. Use the blankest balanced area and keep the title clear of major subjects.
Infer the theme from the photos and automatically trigger matching stickers: subject cutouts, animal/plant/transport/food/study icons, theme labels, and mood-matched decorative pieces.
Sticker strength rule: for each hero photo, add 2-4 obvious strongly related sticker, label, stamp, or ephemera elements; for each supporting photo, add 1-2. Across the spread, make sure there are at least 6-12 clearly readable theme-linked sticker or ephemera pieces. Default mode should still feel clean, but not weak. @S mode should feel even stronger.
Use a visibly distinct decor system: kiss-cut white-border character stickers, silhouette stickers, graphic word stickers, mini photo stickers, hand-drawn blue doodles, printed stickers, paper ephemera, transparent stickers, or tape-and-label details.
Use the kiss-cut sticker language when appropriate: die-cut white outlines, merch sticker pack feeling, photo cutout characters, comic speech bubbles, barcode/tag stickers, bold outlined word stickers, and small irregular sticker clusters.
Keep the paper clean and fresh with visible blank cream/white/grid areas, medium detail, balanced spacing, no dirty texture, and no chaotic clutter. Do not make the spread feel empty or under-decorated.
Use chunky cobalt-blue marker handwriting and doodles.
Visible text: Chinese and English only; no Japanese, no kana, no pseudo-Japanese.
Vary the copy every run. Use a fresh mix of short titles, labels, speech bubbles, route notes, checklists, and ticket/date stamps such as 今日小记, 风景收集, 旅途碎片, 慢慢走, 城市漫游, 山野来信, 路过这里, 把风装进口袋, 这一刻很轻, 值得记住, Weekend Notes, Field Notes, Memory Map, tiny stop, soft pause, keep this. Avoid repeating the same TRAVEL DIARY / GOOD DAY wording by default.
Calendar/date/ticket text must use the current invocation date.
If a cutting mat appears, its grid must be perfectly straight, level, evenly spaced, and parallel to the image borders.
Avoid UI collage, PPT grid, album template, warped mat grid, thin digital fonts, messy paper, and repeated fixed layouts.
```

## QA Before Final

Check the generated image before responding:

- All requested photos appear and no unrelated photo insert was added.
- The output is an open notebook / double-page spread unless the user asked otherwise.
- The two pages have different roles.
- The main title is not always on the left; its placement looks intentionally chosen for this layout and uses available blank space without covering key subjects.
- Sticker triggering is visibly strong: hero photos have clear related sticker groups, supporting photos also have noticeable matching sticker cues, and the spread theme is readable at a glance.
- If `@S` was absent, the result follows the perfect classic style: clean blue cutting mat, open cream grid notebook, strong white-border photo/sticker/ticket composition, restrained accessories, and no overbuilt notebook body.
- If `@S` was present, the physical notebook body is not plain: it has a visible distinctive cover/binding/strap/tab/clip/charm feature, with varied plausible accessories placed on edges without covering important photo subjects, and sticker strength is at least as strong as the default mode.
- The decor system is visibly specific, not the same generic tape/label set every run.
- Stickers clearly match the scrapbook theme inferred from the photos, such as nature stickers for nature photos, transit/ticket stickers for city travel, food stickers for cafe images, or white-border cutout/person stickers for portraits.
- Text is Chinese/English only, date labels use the current invocation date, and the copy is not the same fixed set of title/checklist/speech-bubble phrases from previous runs.
- Cutting mat grids, if present, are straight and parallel.
- The paper is clean, readable, and not over-detailed.
