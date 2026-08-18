---
# try also 'default' to start simple
theme: seriph
# some information about your slides (markdown enabled)
title: Chinese Fan Translation on PSP
info: "Han Hua (汉化): the Chinese fan-localization scene on PSP — scale,
  encoding, and fonts."
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
---

# Chinese Fan Translation on PSP

**汉化 (Han Hua)** — “Chinese-izing” a game

More than 600 fan translations · one encoding problem

<!--
Open with the scale of the scene: roughly 600 PSP games fan-translated into Chinese, versus 57 English translations on romhacking.net. Most came out of the 2010s, when the PSP was the most popular handheld in China, and most are based on Japanese releases. With LLMs, more games are now being reversed and translated than ever before.
-->

---
layout: center
class: text-center
---

<div class="text-[10rem] font-bold leading-none text-slate-800">汉化</div>
<div class="mt-10 text-3xl text-slate-500 tracking-[0.4em]">Chinese -lize</div>

---

<div class="flex flex-col h-full justify-center max-w-5xl mx-auto w-full">

# Chinese Fan Translation on PSP

<div class="grid grid-cols-2 gap-8 mt-8">

<div class="rounded-2xl border-2 border-[#3D8DFF] bg-[#EEF5FF] p-8 text-center">
<div class="text-6xl font-bold text-[#3D8DFF]">600+</div>
<div class="mt-2 text-xl text-slate-700">PSP games fan-translated into Chinese</div>
</div>

<div class="rounded-2xl border-2 border-slate-200 bg-white p-8 text-center">
<div class="text-6xl font-bold text-slate-400">57</div>
<div class="mt-2 text-xl text-slate-600">English translations on romhacking.net</div>
</div>

</div>

<div class="mt-8 space-y-3 text-lg text-slate-600">

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>Most appeared in the <b>2010s</b>, when the PSP was the most popular handheld in China</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>Most are based on <b>Japanese versions</b> of the games</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>With <b>LLMs</b>, more games are now being reverse-engineered and translated than ever before</span>
</div>

</div>

</div>

---

<div class="flex flex-col h-full justify-center max-w-6xl mx-auto w-full">

# Challenges

In English translations, the problem usually lies in **Memory**.

<div class="flex flex-col gap-9 mt-8">

<!-- Chinese -->
<div class="flex items-center gap-5">
<span class="w-20 shrink-0 text-xl font-semibold text-slate-700">Chinese</span>
<div class="flex gap-1.5">
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">我</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">喝</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">水</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
</div>
<span class="text-2xl font-bold text-slate-400">=</span>
<span class="px-4 py-1.5 rounded-full bg-[#3D8DFF] text-white text-xl font-bold">6 bytes</span>
</div>

<!-- Japanese -->
<div class="flex items-center gap-5">
<span class="w-20 shrink-0 text-xl font-semibold text-slate-700">Japanese</span>
<div class="flex gap-1.5">
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">水</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">を</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">飲</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-12 h-14 rounded-lg border-2 border-[#3D8DFF] bg-white flex items-center justify-center text-2xl font-semibold text-slate-800">む</div>
<span class="mt-1 text-xs font-semibold text-[#3D8DFF]">2B</span>
</div>
</div>
<span class="text-2xl font-bold text-slate-400">=</span>
<span class="px-4 py-1.5 rounded-full bg-[#3D8DFF] text-white text-xl font-bold">8 bytes</span>
</div>

<!-- English -->
<div class="flex items-center gap-5">
<span class="w-20 shrink-0 text-xl font-semibold text-slate-700">English</span>
<div class="flex gap-1">
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">I</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border border-slate-200 bg-slate-50"></div>
<span class="mt-0.5 text-[10px] font-semibold text-slate-300">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">d</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">r</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">i</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">n</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">k</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border border-slate-200 bg-slate-50"></div>
<span class="mt-0.5 text-[10px] font-semibold text-slate-300">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">w</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">a</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">t</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">e</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
<div class="flex flex-col items-center">
<div class="w-8 h-10 rounded border-2 border-[#F59E0B] bg-white flex items-center justify-center text-base font-semibold text-slate-800">r</div>
<span class="mt-0.5 text-[10px] font-semibold text-[#F59E0B]">1B</span>
</div>
</div>
<span class="text-2xl font-bold text-slate-400">=</span>
<span class="px-4 py-1.5 rounded-full bg-[#F59E0B] text-white text-xl font-bold">13 bytes</span>
</div>

</div>

<div class="mt-8 text-center text-lg text-slate-500">Avoiding overflow needs a lot of remapping on memory layout</div>

</div>

---

# Challenges: Encoding and Fonts

<div class="grid grid-cols-2 gap-10 items-stretch mt-4">

<div class="flex flex-col justify-center gap-4 text-[1.15rem] leading-relaxed">

For **Chinese** translations, the core problems are **encoding** and **font**:

<ul class="list-disc ml-6 space-y-2">
<li><b>Shift JIS</b>, the encoding used by most PSP games, covers <b>6,355</b> kanji</li>
<li><b>GB2312</b>, a subset of GB18030 (87,887 characters), has <b>6,763</b> characters</li>
<li>Only <b>3,331</b> share the same encoding in Unicode</li>
</ul>

</div>

<div class="flex flex-col items-center justify-center gap-3">

<div class="relative h-44 w-72">
<div class="absolute left-0 top-1/2 -translate-y-1/2 w-44 h-44 rounded-full bg-[#6DCBF4]/60 flex flex-col items-center justify-center font-bold text-slate-800"><span>Shift JIS</span><span class="text-3xl">6,355</span></div>
<div class="absolute right-0 top-1/2 -translate-y-1/2 w-44 h-44 rounded-full bg-[#3D8DFF]/50 flex flex-col items-center justify-center font-bold text-white"><span>GB2312</span><span class="text-3xl">6,763</span></div>
<div class="absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 w-20 h-20 rounded-full bg-white border-2 border-slate-400 z-10 flex flex-col items-center justify-center text-center"><span class="text-xl font-bold text-slate-800">3,331</span><span class="text-[10px] leading-tight text-slate-500">shared in Unicode</span></div>
</div>

<img src="/GB2312inSJIS.png" alt="GB2312-80 character map" class="block max-h-32 rounded-lg border border-slate-200 shadow-md" />

<div class="text-center text-xs text-slate-400">GB2312-80 character map, White ones are not presented in Shift-JIS</div>

<div class="text-sm text-slate-500 text-center max-w-xs">The characters a translation needs simply aren't in the Japanese encoding.</div>

</div>

</div>

<!--
The memory slide showed the English pain with a byte-count example; Chinese translations hit an encoding-and-font wall instead. Sources: roughly 600 Chinese fan translations vs 57 English ones on romhacking.net (count as of the recording); Shift JIS 6,355 kanji, GB2312 6,763 characters (a subset of GB18030's 87,887), and 3,331 characters shared at the same Unicode encoding — from the speaker's research notes.
-->

---

# The usual fix: remap glyphs, keep Shift JIS

Reuse the Shift-JIS encoding byte scheme.

<div class="grid grid-cols-[1fr_auto] gap-10 items-start mt-4">

<div class="space-y-4">

<!-- <div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">1</div>
<div><p class="font-semibold">Reuse the Shift JIS encoding</p><p class="text-slate-500">Keep the game's original byte scheme.</p></div>
</div> -->

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">2</div>
<div><p class="font-semibold">Count the characters the translation needs</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">3</div>
<div><p class="font-semibold">Swap Japanese font glyphs for Chinese glyphs</p><p class="text-slate-500">The old character slots get new shapes.</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">4</div>
<div><p class="font-semibold">Generate a new byte → character mapping</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">5</div>
<div><p class="font-semibold">Encode the sentences, inject into the resources</p></div>
</div>

</div>

<div class="w-80 shrink-0 rounded-2xl border border-slate-200 bg-white/80 p-6 shadow-sm">

<div class="text-lg font-semibold text-slate-800 mb-4">Shift JIS byte ranges</div>

<div class="mb-5">
<div class="text-sm font-bold text-[#3D8DFF] mb-2">Single-byte (1B)</div>
<div class="space-y-1.5 text-sm">
<div class="flex items-center gap-2"><span class="font-mono px-2 py-0.5 rounded bg-slate-100 text-[13px]">00–7F</span><span class="text-slate-500">ASCII</span></div>
<div class="flex items-center gap-2"><span class="font-mono px-2 py-0.5 rounded bg-slate-100 text-[13px]">A1–DF</span><span class="text-slate-500">half-width katakana</span></div>
</div>
</div>

<div>
<div class="text-sm font-bold text-[#3D8DFF] mb-2">Double-byte (2B): Kanji and Kana</div>
<div class="space-y-1.5 text-sm">
<div class="flex items-center gap-2"><span class="font-mono px-2 py-0.5 rounded bg-slate-100 text-[13px]">81–9F, E0–EF</span><span class="text-slate-500">lead byte</span></div>
<div class="flex items-center gap-2"><span class="font-mono px-2 py-0.5 rounded bg-slate-100 text-[13px]">40–7E, 80–FC</span><span class="text-slate-500">trail byte</span></div>
</div>
</div>

<div class="mt-4 pt-3 border-t border-slate-100 text-xs text-slate-500 leading-relaxed">Glyphs in 2-byte range are replaced with Chinese characters.</div>

</div>

</div>

The Glyphs are usually stored as Texture or Bitmap in the game resources.

<!--
Walk through the five steps. The key insight: translators don't switch encodings — they rebuild the byte-to-glyph mapping inside the existing Shift JIS scheme and swap the font glyphs, so the game engine keeps working unchanged.
-->

---

# The Game

<div class="text-slate-500 mt-1 text-lg">Neon Genesis Evangelion 2: Tsukurareshi Sekai -another cases-</div>

<div class="grid grid-cols-[1.2fr_auto] gap-10 items-center mt-6 max-w-5xl mx-auto">

<div class="space-y-3 text-lg text-slate-600">

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>PS2 in 2003, enhanced version on PSP in 2006</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span><b>Fully Voiced</b> with <b>37,000</b> lines of dialogue</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>Play as <b>Shinji, Rei, Asuka</b> and other characters. Choices shape relationships and story branches</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>3D locations and battles, with 2D event scenes and character portraits</span>
</div>

It's basically the definitive Evangelion game.

</div>

<div class="w-64 shrink-0 overflow-hidden rounded-lg border border-slate-300 bg-white shadow-md">

<div class="bg-slate-50 border-b border-slate-200 flex items-center justify-center">
<img src="/71176_front.jpg" alt="Neon Genesis Evangelion 2 PSP cover" class="h-48 object-contain" />
</div>

<div class="px-3 py-1 text-sm font-semibold text-slate-700">Neon Genesis Evangelion 2</div>

<div class="px-3 py-1 text-sm">

<div class="flex justify-between gap-3 py-0.5 border-b border-slate-100"><span class="text-slate-500 shrink-0">Platform</span><span class="text-slate-800 text-right">PSP</span></div>

<div class="flex justify-between gap-3 py-0.5 border-b border-slate-100"><span class="text-slate-500 shrink-0">Developer</span><span class="text-slate-800 text-right">AlfaSystem</span></div>

<div class="flex justify-between gap-3 py-0.5 border-b border-slate-100"><span class="text-slate-500 shrink-0">Publisher</span><span class="text-slate-800 text-right">Bandai</span></div>

<div class="flex justify-between gap-3 py-0.5 border-b border-slate-100"><span class="text-slate-500 shrink-0">Release Date</span><span class="text-slate-800 text-right">2006-04-27 (JP)</span></div>

<div class="flex justify-between gap-3 py-0.5"><span class="text-slate-500 shrink-0">Genre</span><span class="text-slate-800 text-right">SLG</span></div>

</div>

</div>

</div>

<!--
This is the game the talk's reverse-engineering project targets: the PSP release (ULJS-00064) of Neon Genesis Evangelion 2: The Created World -Another Cases-. Sources: English Wikipedia, EvaGeeks wiki, Launchbox DB, GameSpot preview.
-->

---

# The hook point: sceFont

<div class="flex items-center justify-center gap-5 mt-10">

<div class="text-center">
<div class="text-xl font-semibold text-slate-700">Shift-JIS text</div>
<div class="text-sm text-slate-400 mt-1">stored in game data</div>
</div>

<div class="text-3xl text-slate-300">→</div>

<div class="text-center">
<div class="text-xl font-bold text-[#3D8DFF]">SJIS → UTF-16</div>
<div class="text-sm font-semibold text-[#3D8DFF] mt-1">▲ hook here</div>
</div>

<div class="text-3xl text-slate-300">→</div>

<div class="text-center">
<div class="text-xl font-semibold text-slate-700">sceFont</div>
<div class="text-sm text-slate-400 mt-1">PSP font library renders</div>
</div>

</div>

<div class="mt-12 max-w-4xl mx-auto space-y-4 text-[1.05rem] text-slate-600 leading-relaxed">

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>The game stores its text as <b>Shift-JIS</b> strings</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>PSP text rendering goes through the <b>sceFont</b> library, which consumes <b>UTF-16</b></span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>Every draw call converts <b>SJIS → UTF-16</b> first — hook that conversion and sceFont renders whatever we feed it</span>
</div>

</div>

---

# Custom Shift-JIS → UTF-16 mapping

<div class="text-slate-500 mt-1 text-lg">Borrowing unused code points so Chinese and Japanese can coexist</div>

<div class="grid grid-cols-2 gap-10 items-center mt-5">

<div class="space-y-5 text-[1rem] text-slate-600 leading-relaxed">

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>Shift-JIS is <b>variable-length</b> — the lead byte decides whether a character takes <b>1 byte or 2 bytes</b>.</span>
</div>

<div class="flex items-start gap-3">
<span class="w-2 h-2 rounded-full bg-[#3D8DFF] mt-3 shrink-0"></span>
<span>We customized the Shift-JIS → UTF-16 parsing so ranges normally read as <b>single-byte</b> can also carry <b>two-byte sequences</b> — borrowing unused code points to store Chinese characters.</span>
</div>

</div>

<div class="rounded-2xl border border-slate-200 bg-white p-3 shadow-sm">
<video src="/SJIS_Hack_Visual.mp4" controls class="w-full rounded-lg"></video>
<div class="text-center text-xs text-slate-400 mt-2">Demo · Chinese text rendered with the custom mapping</div>
</div>

</div>

<div class="grid grid-cols-3 gap-4 mt-5">

<div class="rounded-xl border border-slate-200 bg-white p-3 text-center">
<div class="text-sm font-bold text-slate-800 mb-1">Japanese untouched</div>
<div class="text-[0.85rem] text-slate-500">Original double-byte code points keep working</div>
</div>

<div class="rounded-xl border border-slate-200 bg-white p-3 text-center">
<div class="text-sm font-bold text-slate-800 mb-1">Unused region reused</div>
<div class="text-[0.85rem] text-slate-500">Only part of the half-width katakana area — unused by this game</div>
</div>

<div class="rounded-xl border border-slate-200 bg-white p-3 text-center">
<div class="text-sm font-bold text-slate-800 mb-1">No conflicts</div>
<div class="text-[0.85rem] text-slate-500">Untranslated Japanese and translated Chinese coexist</div>
</div>

</div>

---

# Background: the game's memory system

<div class="text-slate-500 mt-1 text-lg">The game generates <b>memory sentences</b> at runtime from past events</div>

<div class="flex gap-4 mt-6">
<img src="/wordorder/memory-1.jpeg" class="flex-1 h-40 object-cover rounded-lg border border-slate-200 shadow-sm" />
<img src="/wordorder/memory-2.jpeg" class="flex-1 h-40 object-cover rounded-lg border border-slate-200 shadow-sm" />
<img src="/wordorder/memory-3.jpeg" class="flex-1 h-40 object-cover rounded-lg border border-slate-200 shadow-sm" />
</div>

<div class="mt-5 text-center text-lg text-slate-500">These sentences are composed from <b>fixed templates</b> — not written by hand</div>

---

# The problem: fixed-slot sentence templates

<div class="flex flex-wrap justify-center gap-x-4 gap-y-1.5 mt-3 text-xs">
<span class="px-2 py-0.5 rounded border-2 bg-blue-100 border-blue-400 text-blue-800">Subject</span>
<span class="px-2 py-0.5 rounded border-2 bg-slate-100 border-slate-300 text-slate-600">particle</span>
<span class="px-2 py-0.5 rounded border-2 bg-amber-100 border-amber-400 text-amber-800">Object</span>
<span class="px-2 py-0.5 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800">fixed ending</span>
</div>

<div class="grid grid-cols-2 gap-7 mt-4">

<div class="rounded-xl border border-slate-200 bg-white p-4">
<div class="text-xs font-semibold text-slate-700 mb-2">Japanese: SOV fits the slots</div>
<div class="flex flex-wrap justify-center gap-1.5">
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">shinji</span><span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm mt-1">シンジ</span><span class="text-[11px] text-slate-500 mt-1">Shinji</span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">ga</span><span class="px-2 py-1 rounded border-2 bg-slate-100 border-slate-300 text-slate-600 font-mono text-sm mt-1">が</span><span class="text-[11px] text-slate-500 mt-1"></span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">jibun</span><span class="px-2 py-1 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-sm mt-1">自分</span><span class="text-[11px] text-slate-500 mt-1">myself</span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">o</span><span class="px-2 py-1 rounded border-2 bg-slate-100 border-slate-300 text-slate-600 font-mono text-sm mt-1">を</span><span class="text-[11px] text-slate-500 mt-1"></span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">tsuyoku dakishimeta</span><span class="px-2 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm mt-1">強く抱きしめた</span><span class="text-[11px] text-slate-500 mt-1">hugged tightly</span></div>
</div>
<div class="text-xs font-semibold text-slate-700 mt-3 mb-2">What the game fills in</div>
<div class="flex flex-wrap justify-center gap-1.5">
<span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm">Shinji</span>
<span class="px-2 py-1 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-sm">myself</span>
<span class="px-2 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm">hugged … tightly</span>
</div>
<div class="mt-2 text-center text-sm text-red-500">✗ — the object lands before the verb</div>
</div>

<div class="rounded-xl border border-slate-200 bg-white p-4">
<div class="text-xs font-semibold text-slate-700 mb-2">English: SVO + preposition breaks the slots</div>
<div class="flex flex-wrap justify-center gap-1.5">
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">penpen</span><span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm mt-1">ペンペン</span><span class="text-[11px] text-slate-500 mt-1">Pen Pen</span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">ga</span><span class="px-2 py-1 rounded border-2 bg-slate-100 border-slate-300 text-slate-600 font-mono text-sm mt-1">が</span><span class="text-[11px] text-slate-500 mt-1"></span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">jibun</span><span class="px-2 py-1 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-sm mt-1">自分</span><span class="text-[11px] text-slate-500 mt-1">myself</span></div>
<div class="flex flex-col items-center"><span class="px-1.5 py-0.5 rounded border border-dashed border-slate-300 text-slate-400 font-mono text-xs">ni, tawainai hanashi o shita</span><span class="px-2 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm mt-1">に、たわいもない話をした</span><span class="text-[11px] text-slate-500 mt-1">talked about trivial things</span></div>
</div>
<div class="text-xs font-semibold text-slate-700 mt-3 mb-2">What the game fills in</div>
<div class="flex flex-wrap justify-center gap-1.5">
<span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm">Pen Pen</span>
<span class="px-2 py-1 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-sm">myself</span>
<span class="px-2 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm">said trivial things to …</span>
</div>
<div class="mt-2 text-center text-sm text-red-500">✗ — the object lands before the preposition</div>
</div>

</div>

<div class="mt-4 text-center text-lg text-slate-500">The object has to move <b>into</b> the fixed ending</div>

---

# The fix: move the object into the template

<div class="text-slate-500 mt-1 text-lg"><span class="font-mono text-[0.9em] bg-slate-100 px-2 py-0.5 rounded">object + predicate → sprintf(predicate, object)</span> — the fixed ending absorbs the object as <b>{B}</b></div>

<div class="grid grid-cols-2 gap-6 mt-5">

<div class="rounded-xl border border-slate-200 bg-white p-4">
<div class="font-mono text-sm text-slate-600">“に照れたこと”</div>
<div class="mt-2 text-lg font-medium text-slate-800">→ shy of <span class="px-1.5 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-base">{B}</span></div>
</div>

<div class="rounded-xl border border-slate-200 bg-white p-4">
<div class="font-mono text-sm text-slate-600">“に対して不快感を持ったこと”</div>
<div class="mt-2 text-lg font-medium text-slate-800">→ felt uneasy toward <span class="px-1.5 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-base">{B}</span></div>
</div>

</div>

<div class="mt-5 rounded-xl border border-[#3D8DFF]/30 bg-[#EEF5FF] p-4">
<div class="text-xs font-semibold text-slate-700 mb-3 text-center">The same sentence, rebuilt</div>

<div class="flex flex-wrap justify-center gap-1.5">
<div class="flex flex-col items-center"><span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm">シンジ</span><span class="text-[11px] text-slate-500 mt-1">Shinji</span></div>
<div class="flex flex-col items-center"><span class="px-2 py-1 rounded border-2 bg-slate-100 border-slate-300 text-slate-600 font-mono text-sm">が</span><span class="text-[11px] text-slate-500 mt-1">subj.</span></div>
<div class="flex flex-col items-center"><span class="px-2 py-1 rounded border-2 bg-amber-100 border-amber-400 text-amber-800 font-mono text-sm">自分</span><span class="text-[11px] text-slate-500 mt-1">myself(me)</span></div>
<div class="flex flex-col items-center"><span class="px-2 py-1 rounded border-2 bg-slate-100 border-slate-300 text-slate-600 font-mono text-sm">を</span><span class="text-[11px] text-slate-500 mt-1">obj.</span></div>
<div class="flex flex-col items-center"><span class="px-2 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm">強く抱きしめた</span><span class="text-[11px] text-slate-500 mt-1">hugged tightly</span></div>
</div>

<div class="text-center text-slate-400 text-lg leading-none my-2">↓</div>

<div class="flex flex-wrap justify-center gap-1.5">
<span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm">Shinji</span>
<span class="px-3 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm">hugged <span class="px-1.5 rounded border-2 bg-amber-100 border-amber-400 text-amber-800">{B}</span> tightly</span>
</div>

<div class="text-center text-sm text-slate-500 my-2">fill {B} = me</div>

<div class="flex flex-wrap justify-center gap-1.5">
<span class="px-2 py-1 rounded border-2 bg-blue-100 border-blue-400 text-blue-800 font-mono text-sm">Shinji</span>
<span class="px-3 py-1 rounded border-2 bg-emerald-100 border-emerald-400 text-emerald-800 font-mono text-sm">hugged <span class="px-1.5 rounded border-2 bg-amber-100 border-amber-400 text-amber-800">me</span> tightly</span>
<span class="text-xl font-bold text-emerald-600 mt-1">✓</span>
</div>
</div>

---

# Effect: memory text in Chinese

<div class="text-slate-500 mt-1 text-lg">The rebuilt templates produce grammatical Chinese from the same memory events</div>

<div class="relative flex justify-center mt-5">
<img src="/wordorder/effect.png" class="h-80 rounded-xl border border-slate-200 shadow-md" />
<div class="absolute bottom-2 left-1/2 -translate-x-1/2 w-[93%] rounded-lg bg-[#153A6E]/90 px-4 py-2 text-center text-sm text-white leading-snug">
Shinji told Pen Pen, 3 days ago, here, Misato became interested in Pen Pen's words.
</div>
</div>

---

# Architecture: three modules, one RAM

<div class="text-slate-500 mt-1 text-lg">A <b>loader</b> replaces the game's EBOOT, then pulls in the <b>game</b> and a <b>runtime plugin</b> — all three share the PSP's 32 MB of main RAM</div>

<div class="grid grid-cols-[1fr_auto] gap-12 items-center mt-4">

<div class="space-y-4 max-w-md">
<div class="flex items-start gap-2">
<span class="w-3 h-3 mt-1.5 rounded-sm bg-[#3D8DFF] shrink-0"></span>
<div><b>Loader · EBOOT.BIN</b><div class="text-slate-500 text-[12px]">first user module at 0x08804000 — menu, then loads the other two</div></div>
</div>
<div class="flex items-start gap-2">
<span class="w-3 h-3 mt-1.5 rounded-sm bg-amber-400 shrink-0"></span>
<div><b>Game · BOOT.BIN</b><div class="text-slate-500 text-[12px]">decrypted original EBOOT — loaded, patched, then started</div></div>
</div>
<div class="flex items-start gap-2">
<span class="w-3 h-3 mt-1.5 rounded-sm bg-emerald-400 shrink-0"></span>
<div><b>Runtime · EVA2RT.PRX</b><div class="text-slate-500 text-[12px]">resident patch engine — hooks, font, EBTRANS text</div></div>
</div>
<div class="text-[12px] text-slate-500 pt-1">Patch addresses are rebased at runtime: <span class="font-mono text-[0.9em] bg-slate-100 px-1.5 py-0.5 rounded">patch_addr = game_base + (IDA_addr − 0x08804000)</span></div>
</div>

<div class="flex gap-3 items-stretch">

<div class="flex flex-col justify-between text-right font-mono text-[11px] text-slate-400 leading-none py-1">
<span>0x09FFFFFF</span>
<span>0x08800000</span>
</div>

<div class="w-16 h-72 flex flex-col overflow-hidden rounded-lg border-2 border-slate-300 shadow-sm">
<div class="flex-1 bg-emerald-100 border-b-2 border-emerald-400 flex items-center justify-center font-mono text-[11px] font-bold text-emerald-800">EVA2RT</div>
<div class="flex-1 bg-amber-100 border-b-2 border-amber-400 flex items-center justify-center font-mono text-[11px] font-bold text-amber-800">BOOT</div>
<div class="h-14 bg-[#3D8DFF] flex items-center justify-center font-mono text-[11px] font-bold text-white">EBOOT</div>
</div>

<div class="flex flex-col text-left font-mono text-[11px] leading-none">
<div class="flex-1 flex items-center"><span class="text-emerald-600">runtime · dynamic</span></div>
<div class="flex-1 flex items-center"><span class="text-amber-600">game · dynamic</span></div>
<div class="h-14 flex items-center"><span class="text-[#3D8DFF]">loader · 0x08804000</span></div>
</div>

</div>

</div>

<!--
The three modules coexist in the PSP's 32 MB user memory. The firmware loads EBOOT.BIN (the loader) first at 0x08804000; it replaces the original game's EBOOT in SYSDIR. The original EBOOT.BIN is decrypted and renamed BOOT.BIN, and the runtime is EVA2RT.PRX, both loaded into free RAM — so only the loader base is fixed. The runtime receives the game's module id, calls sceKernelQueryModuleInfo to get segmentaddr[0] as game_base, and converts every IDA-era address (from the 0x08804000 static base) into the real location with game_base + (addr − 0x08804000). The loader's menu framebuffers live in VRAM (0x04000000+), separate from main RAM; the runtime's font atlas and GB2312 tables are compiled-in C arrays.
-->

---

# Startup order: loader → runtime → game

<div class="text-slate-500 mt-1 text-lg">The runtime patches the game image <b>before</b> the game's code ever runs</div>

<div class="grid grid-cols-[1.05fr_0.95fr] gap-10 mt-5 items-start">

<div class="space-y-2 text-[0.95rem]">

<div class="flex items-start gap-3">
<div class="w-8 h-8 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center text-sm">1</div>
<div><b>Firmware boots EBOOT.BIN</b> — the loader, not the game, becomes the first user module at 0x08804000.</div>
</div>

<div class="text-center text-slate-300 leading-none">↓</div>

<div class="flex items-start gap-3">
<div class="w-8 h-8 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center text-sm">2</div>
<div><b>Loader UI</b> — start menu with debug toggles, then the contributor screen (<span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">metadata.raw</span>).</div>
</div>

<div class="text-center text-slate-300 leading-none">↓</div>

<div class="flex items-start gap-3">
<div class="w-8 h-8 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center text-sm">3</div>
<div><b>Load both modules</b> — <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">BOOT.BIN</span> (game) then <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">EVA2RT.PRX</span> (runtime) are mapped into free RAM; neither runs yet.</div>
</div>

<div class="text-center text-slate-300 leading-none">↓</div>

<div class="flex items-start gap-3">
<div class="w-8 h-8 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center text-sm">4</div>
<div><b>Runtime boots first</b> — receives <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">{boot_mid, flags}</span>, queries the game's base, installs every patch into the stopped game image, flushes caches.</div>
</div>

<div class="text-center text-slate-300 leading-none">↓</div>

<div class="flex items-start gap-3">
<div class="w-8 h-8 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center text-sm">5</div>
<div><b>Game boots</b> — the loader starts the patched game; the runtime stays resident for hooks.</div>
</div>

</div>

<div class="rounded-2xl border border-slate-200 bg-white/80 p-5">

<div class="text-xs font-bold text-[#3D8DFF] tracking-[0.2em] uppercase mb-3">The hand-off in code</div>

<pre class="rounded-lg bg-slate-50 border border-slate-200 p-3 text-[11px] leading-relaxed overflow-x-auto"><code class="font-mono"><span class="text-slate-500">// loader.c</span>
<span class="text-slate-600">SceUID game</span> = sceKernelLoadModule(<span class="text-emerald-700">"disc0:/PSP_GAME/SYSDIR/BOOT.BIN"</span>, ...);
<span class="text-slate-600">SceUID runtime</span> = sceKernelLoadModule(<span class="text-emerald-700">"disc0:/PSP_GAME/SYSDIR/EVA2RT.PRX"</span>, ...);

Eva2RuntimeStartArgs args = { <span class="text-amber-700">game</span>, flags };
<span class="text-[#3D8DFF]">sceKernelStartModule(runtime, sizeof(args), &amp;args, ...)</span>; <span class="text-slate-500">// patches land here</span>
<span class="text-[#3D8DFF]">sceKernelStartModule(game, 0, NULL, ...)</span>;                <span class="text-slate-500">// game boots patched</span></code></pre>

<pre class="rounded-lg bg-slate-50 border border-slate-200 p-3 text-[11px] leading-relaxed overflow-x-auto mt-3"><code class="font-mono"><span class="text-slate-500">// runtime_entry.c</span>
sceKernelQueryModuleInfo(boot_mid, &amp;info);
<span class="text-[#3D8DFF]">RuntimePatch_InstallAll(info.segmentaddr[0], flags)</span>;
HookWrite_FlushCaches(); <span class="text-slate-500">// dcache write-back, icache invalidate</span></code></pre>

<div class="mt-3 text-[12px] text-slate-500 leading-relaxed">
Patches include: text encoding range, sentence/UTF-8, <span class="font-mono text-[0.85em] bg-slate-100 px-1 py-0.5 rounded">EBTRANS.BIN</span> injection, <span class="font-mono text-[0.85em] bg-slate-100 px-1 py-0.5 rounded">sceFont</span> replacement, save-data language, memory-text templates, staff roll, debug menus.
</div>

</div>

</div>

<!--
The order matters: the runtime starts before the game, so it can rewrite the game's loaded-but-idle image. module_start receives the game's module id and flags, queries the module info to find the real base (segmentaddr[0]), installs every patch (each is a direct 32-bit store or a JAL/J rewrite via _sw), then HookWrite_FlushCaches does dcache write-back and icache invalidate so the running game sees consistent code. Only then does the loader start the game module. The runtime stays resident: hooks like sceFont text rendering, memory-text fill-ins, the staff roll and debug menus run from its code.
-->

---

# Milestones in Reverse Engineering the Game

<!-- <div class="text-slate-500 mt-1 text-lg">One EvaGeeks thread on this game · 741 posts · 2006 – 2026</div> -->

<div class="grid grid-cols-2 gap-x-12 mt-6">

<div>
<div class="text-xs font-bold text-[#3D8DFF] tracking-[0.2em] uppercase mb-3">The EvaGeeks thread · 2006 –</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-16 shrink-0 font-bold text-[#3D8DFF]">2010</span><span class="text-slate-600">English-menu patch proof-of-concept on a real PSP</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-16 shrink-0 font-bold text-[#3D8DFF]">2011</span><span class="text-slate-600">Text files located in the ISO — <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">imtext.bin</span> / <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">btimtext.bin</span> (Shift-JIS → UTF-8)</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-20 shrink-0 font-bold text-[#3D8DFF]">2018-01-07</span><span class="text-slate-600">rezual creates the <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">nge_2_re</span> repo</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-16 shrink-0 font-bold text-[#3D8DFF]">2018-01</span><span class="text-slate-600">HAR archives unpacked (<span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">hgar.py</span>); HGPT image conversion; game's own decompression run in a mini PSP interpreter</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-16 shrink-0 font-bold text-[#3D8DFF]">2018-02</span><span class="text-slate-600">EVS scripts &amp; data tables mapped; file replacement working</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
</div>
<div class="min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-16 shrink-0 font-bold text-[#3D8DFF]">2020</span><span class="text-slate-600">Compression identified as DEFLATE — compressor + decompressor complete</span></div>
</div>
</div>

</div>

<div>
<div class="text-xs font-bold text-[#3D8DFF] tracking-[0.2em] uppercase mb-3">This project · 2024 –</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2024-04-19</span><span class="text-slate-600">Fork of rezual's <span class="font-mono text-[0.85em] bg-slate-100 px-1.5 py-0.5 rounded">nge_2_re</span></span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2024-04→06</span><span class="text-slate-600">Encoding-conversion functions &amp; glyph table located</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2024-06→09</span><span class="text-slate-600">Crowdin + DeepL, then LLM-assisted machine translation</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2025</span><span class="text-slate-600">EBOOT loader; custom encoding implemented</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2026-01→02</span><span class="text-slate-600">Qwen3-VL OCR for image text; contributor startup screen</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
<span class="flex-1 w-0.5 bg-[#3D8DFF]/25"></span>
</div>
<div class="pb-3 min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2026-06</span><span class="text-slate-600">Loader + runtime plugin architecture</span></div>
</div>
</div>

<div class="flex gap-3">
<div class="flex flex-col items-center">
<span class="w-3 h-3 mt-1.5 rounded-full bg-[#3D8DFF] ring-4 ring-[#3D8DFF]/20 shrink-0"></span>
</div>
<div class="min-w-0">
<div class="flex items-baseline gap-3 text-[0.9rem] leading-snug"><span class="w-24 shrink-0 font-bold text-[#3D8DFF]">2026-06</span><span class="text-slate-600">Memory text localized at runtime — word-order patches</span></div>
</div>
</div>

</div>

</div>

<!--
Two timelines. Left, the EvaGeeks thread's file-format RE: 2010 English-menu patch proof-of-concept; 2011 text files located in the ISO (imtext.bin / btimtext.bin), Shift-JIS → UTF-8; 2018-01-07 rezual creates the nge_2_re repo; 2018-01 HAR archives unpacked (hgar.py), HGPT image conversion, and the game's own decompression run in a mini PSP interpreter; 2018-02 EVS scripts mapped and file replacement working; 2020 compression identified as DEFLATE, so compressor + decompressor both complete. Right, this project: 2024-04-19 fork of rezual's nge_2_re (this repo); 2024-04/06 encoding-conversion functions and the glyph table located; 2024-06/09 Crowdin + DeepL then LLM-assisted MT; 2025 EBOOT loader and custom encoding; 2026-01/02 Qwen3-VL OCR and the contributor startup screen; 2026-06 loader + runtime plugin architecture and runtime memory-text (word-order) patches.
-->
