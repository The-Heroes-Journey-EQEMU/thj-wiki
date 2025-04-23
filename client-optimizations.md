---
title: Client Optimizations
description: Client Optimizations for ROF2 on The Heroes Journey Emulator
published: true
date: 2025-04-23T16:40:20.159Z
tags: 
editor: markdown
dateCreated: 2025-04-23T16:40:20.159Z
---

![optimizations_banner.png](/misc/optimizations_banner.png){.align-center}
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Client Optimization - The Heroes' Journey</title>
  <link rel="stylesheet" href="/wiki/styles/client-optimization.css" />
  <script defer src="/wiki/scripts/client-optimization.js"></script>
</head>
<body>
  <section class="intro">
    <h1>Client Optimization</h1>
    <p>
      Welcome to <strong>The Heroes' Journey</strong>. Optimizing your EQ client helps reduce zoning crashes,
      dinput8.dll errors, and improves overall gameplay stability.
    </p>
    <p>
      If you cannot see embeds or links in Discord, ensure "Show embeds and preview website links" is enabled in your
      Discord settings under <em>Chat</em>.
    </p>
  </section>
  <section class="card-grid">
    <div class="card">
      <h2>Patcher Extras</h2>
      <img src="https://iili.io/3RtzJ4e.jpg" alt="Patcher Extras" />
      <p>
        Use the new patcher <code>heroesjourneyemu.exe</code> found in your game folder. The Extras tab allows
        automatic application of client-side optimizations.
      </p>
    </div>
    <div class="card">
      <h2>4GB Patch & Memory Optimization</h2>
      <img src="https://iili.io/3Rtur9s.png" alt="4GB Patch & Memory" />
      <p>
        Use the patcher Extras tab to enable 4GB patching and memory tweaks. Windowed mode (Alt+Enter twice) is
        strongly recommended.
      </p>
    </div>
    <div class="card">
      <h2>Memory.ini Swap</h2>
      <p>
        Press "Open THJ Folder" in your patcher. Copy <code>memory.ini</code> from the <code>extra</code> folder and
        overwrite the version in <code>resources</code>.
      </p>
    </div>
    <div class="card">
      <h2>Exclusions (VPN, Defender)</h2>
      <p>
        Exclude your game folder in Windows Defender. Avoid using a VPN when logging in. Some antivirus software may
        block downloads or interfere with connectivity.
      </p>
    </div>
    <div class="card">
      <h2>CPU Affinity Settings</h2>
      <p>
        Open Task Manager (Ctrl+Alt+Del → Details Tab → eqgame.exe). Right-click → Set Priority → High.<br />
        Then set CPU Affinity and select 2 or 4 staggered cores (skip CPU 0 & 1).
      </p>
      <p>
        To automate this, consider using <a href="https://bitsum.com/download-process-lasso/" target="_blank">Process Lasso</a>.
      </p>
    </div>
    <div class="card">
      <h2>Disable Voicechat</h2>
      <img src="https://iili.io/3RDaaXs.png" alt="Disable Voicechat" />
      <p>
        In-game, disable voicechat from the options menu. If issues persist, rename or remove <code>vivoxsdk.dll</code>.
        Need it back? You can find it in our <a href="#">Discord FAQs</a>.
      </p>
    </div>
    <div class="card">
      <h2>Manual Optimizations</h2>
      <p>
        Apply the <a href="https://ntcore.com/4gb-patch/" target="_blank">4GB Patch</a> directly to
        <code>eqgame.exe</code>.
      </p><p></p>
      <pre><code>[Defaults]
UseLitBatches=True
VertexShaders=True
ShowDynamicLights=FALSE
MipMapping=FALSE
TextureCache=FALSE
UseD3DTextureCompression=FALSE
MultiPassLighting=0
PostEffects=0
Shadows=0
StreamItemTextures=0
Bloom=0
[Options]
MaxFPS=60
MaxBGFPS=20
Realism=0
ClipPlane=12
LODBias=5</code></pre>
      <p>Also disable Advanced Lighting in-game via Alt+O settings.</p>
    </div>
  </section>
</body>
</html>


![pagebreak3.webp](/pagebreak3.webp){.align-center}