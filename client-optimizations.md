---
title: Client Optimizations
description: Client Optimizations for ROF2 on The Heroes Journey Emulator
published: true
date: 2025-04-23T18:02:46.296Z
tags: 
editor: markdown
dateCreated: 2025-04-23T16:40:20.159Z
---

<!-- Hero Banner -->
<header class="thj-hero" id="top">
  <div class="thj-hero__inner">
    <h1>Optimize Your EQ&nbsp;Client</h1>
    <p>Crush zoning crashes, tame <code>dinput8.dll</code> errors and unleash a silky‑smooth adventure in <strong>The&nbsp;Heroes’ Journey</strong>.</p><p></p><p></p>
    <a href="#get-started" class="thj-btn thj-btn--primary">Get&nbsp;Started</a>
  </div>
</header>

<!-- Intro -->
<section id="get-started" class="thj-section thj-section--narrow">
  <h2>Why Optimize?</h2>
  <p>EverQuest’s RoF2 client can be temperamental on modern hardware. With a few essential tweaks you’ll enjoy <em>fewer crashes</em>, smoother frame‑rates and faster zoning — the perfect recipe for slaying raids ✧</p>
  <p class="thj-note"><strong>It is recommended to do this from the #optimizations channel on our discord. It has every bit of this data, and more.</strong></p>

</section>

<!-- Card Grid -->
<section class="thj-card-grid">
  <!-- FEATURED CARD (all cards are now same width) -->
  <article class="thj-card thj-card--span2">
    <img src="https://iili.io/3RtzJ4e.jpg" alt="Patcher Extras" loading="lazy">
    <h3>Patcher Extras</h3>
    <p>Run <code>heroesjourneyemu.exe</code> → <strong>Extras</strong> to auto‑apply every recommended tweak.</p>
  </article>

  <!-- The rest of the cards now span 2 columns to match -->
  <article class="thj-card thj-card--span2">
    <img src="https://iili.io/3Rtur9s.png" alt="4 GB Patch &amp; Memory" loading="lazy">
    <h3>4 GB Patch &amp; Memory</h3>
    <p>Enable the 4 GB patch + memory optimizations. Press <kbd>Alt</kbd>+<kbd>Enter</kbd> twice for true windowed‑mode stability.</p>
  </article>

  <article class="thj-card thj-card--span2">
    <h3>Memory.ini Swap</h3>
    <p>Open the THJ folder, copy <code>memory.ini</code> from <code>/extra</code> into <code>/resources</code> and overwrite.</p>
  </article>

  <article class="thj-card thj-card--span2">
    <h3>Exclusions (VPN / Defender)</h3>
    <p>Add your game folder to Windows Defender exclusions and avoid VPNs during login.</p>
  </article>

  <article class="thj-card thj-card--span2">
    <h3>CPU Affinity</h3>
    <p>Task Manager → <em>Details</em> → <code>eqgame.exe</code>: set Priority → High and choose 2–4 staggered cores (skip&nbsp;0 &amp; 1).</p>
  </article>

  <article class="thj-card thj-card--span2">
    <img src="https://iili.io/3RDaaXs.png" alt="Disable Voicechat" loading="lazy">
    <h3>Disable Voicechat</h3>
    <p>Turn off voicechat via <kbd>Alt</kbd>+<kbd>O</kbd>. Persistent issues? Rename <code>vivoxsdk.dll</code>.</p>
  </article>

  <!-- Manual tweaks – keep wide at the end -->
  <article class="thj-card thj-card--wide">
    <h3>Manual Tweaks</h3>
    <p>Prefer DIY? Patch <a href="https://ntcore.com/4gb-patch/" target="_blank" rel="noreferrer">eqgame.exe</a> then append:</p>

```
[Defaults]
UseLitBatches=True
VertexShaders=True
ShowDynamicLights=False
MipMapping=False
TextureCache=False
UseD3DTextureCompression=False
MultiPassLighting=0
PostEffects=0
Shadows=0
StreamItemTextures=0
Bloom=0
[Options]
MaxFPS=120
MaxBGFPS=30
Realism=0
ClipPlane=12
LODBias=5
```
  </article>
</section>

![pagebreak3.webp](/pagebreak3.webp){.align-center}<footer class="thj-footer">© 2025 The Heroes’ Journey</footer>
