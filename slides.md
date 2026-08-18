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

<div class="mt-2 space-y-4 max-w-4xl">

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">1</div>
<div><p class="font-semibold">Reuse the Shift JIS encoding</p><p class="text-slate-500">Keep the game's original byte scheme.</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">2</div>
<div><p class="font-semibold">Count the characters the translation needs</p><p class="text-slate-500">Only the used set has to fit.</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">3</div>
<div><p class="font-semibold">Swap Japanese font glyphs for Chinese glyphs</p><p class="text-slate-500">The old character slots get new shapes.</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">4</div>
<div><p class="font-semibold">Generate a new byte → character rule</p><p class="text-slate-500">A custom SJIS table for the translated set.</p></div>
</div>

<div class="flex items-start gap-4">
<div class="w-10 h-10 shrink-0 rounded-full bg-[#3D8DFF] text-white font-bold flex items-center justify-center">5</div>
<div><p class="font-semibold">Encode the sentences, inject into the resources</p><p class="text-slate-500">The game renders Chinese without new engine support.</p></div>
</div>

</div>

<div class="mt-6 text-slate-500">That's why Chinese translations work in-game even though the original release never shipped Chinese support.</div>

<!--
Walk through the five steps. The key insight: translators don't switch encodings — they rebuild the byte-to-glyph mapping inside the existing Shift JIS scheme and swap the font glyphs, so the game engine keeps working unchanged.
-->
