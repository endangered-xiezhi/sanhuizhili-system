## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors
- bg: #0A0A0A
- secondary_bg: #111111
- primary: #141414
- accent: #4A90D9
- secondary_accent: #6BA3E0
- text: #F2F2F2
- text_secondary: #B3B3B3
- border: #333333
- tertiary_text: #666666
- success: #00796B
- warning: #C41E3A
- image_rendering: photo-realistic
- image_palette: minimalist-dark

## typography
- font_family: Arial, "Microsoft YaHei", sans-serif
- code_family: Consolas, "Courier New", monospace
- body: 24
- title: 48
- subtitle: 36
- annotation: 24

## icons
- library: tabler-outline
- stroke_width: 2
- inventory: box-model, shield-check, engine, database, check, x, arrow-right, arrow-down, file-text, microphone, server

## images
- cover_bg: images/cover_bg.png
- architecture: images/architecture.png

## page_rhythm
- P01: anchor
- P02: dense
- P03: dense
- P04: breathing
- P05: dense
- P06: dense
- P07: anchor

## forbidden
- Mixing icon libraries
- rgba()
- <style>, class, <foreignObject>, textPath, @font-face, <animate*>, <script>, <iframe>, <symbol>+<use>
- <g opacity> (set opacity on each child element individually)
- HTML named entities in text (&nbsp;, &mdash;, &copy;, &ndash;, &reg;, &hellip;, &bull; …) — write as raw Unicode (—, ©, →, NBSP, etc.); XML reserved chars & < > " ' must be escaped as &amp; &lt; &gt; &quot; &apos;. See shared-standards.md §1.0
