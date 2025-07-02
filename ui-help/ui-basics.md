---
title: UI Basics
description: This is intended to give you a summary of the EverQuest UI Engine used from 2002-2023
published: false
date: 2025-07-02T02:14:46.885Z
tags: ui guide
editor: markdown
dateCreated: 2025-06-14T06:20:39.026Z
---

<div class="banner-box">

 <img src="/gettingstartedbanner.webp" alt="gettingstartedbanner">

</div>

<div class="page-wrapper">

<div class="installer-guide">

<div class="jump-buttons">

 <a href="#about_sidl" class="jump-button">About SIDL</a>

 <a href="#installer-faq" class="jump-button">Installer FAQ</a>

 <a href=https://discord.com/invite/heroesjourney class="jump-button">Discord</a>

</div>

<h2 id="about_sidl">EverQuest UI Basics</h2>

<p>The EverQuest UI system is defined using <strong>SUITE Interface Development Language (SIDL)</strong>, an XML specification developed by Sony Online Entertainment and released in 2002, where various UI elements like windows, buttons, and animations are structured and linked. This allows for a modular and customizable interface.</p>

<div class="discord-blurb"> <p>To get help with the UI, join <strong>The Heroes' Journey</strong> community.</p><p></p> <a href="https://discord.com/invite/heroesjourney" target="\_blank" class="discord-button">Join the Discord</a> </div>

<p>Check out our <a href="https://wiki.heroesjourneyemu.com/rules">Rules</a> before you start.</p>

<hr>

<div class="file-structure">

<h3>The SIDL File Structure</h3>

The UI folder will have various different XML files, as well as texture files (.tga and .dds files). Most of the XML files will be related to a single interface window. There are a few exceptions to this: 
  
  <ul>
    <li>**EQUI.xml** - This defines what xml files that the skin will use</li>
    <li>**SIDL.xml** - This holds definitions for all of the individual elements and components</li>
    <li>**EQUI_Animations.xml** - This holds info on textures and how they are loaded into each component</li>
    <li>**EQUI_Templates.xml** - This defines templating for various elements, including texture references</li>
    </ul>
  
The rest of the xml files will be named according to what UI element they create. Some examples are:
  <ul>
    <li>EQUI_Inventory.xml - The Inventory screen. This is the most complex element and contains hundreds of components</li>
    <li>EQUI_PlayerWindow.xml - The player window</li>
    <li>EQUI_TrackingWnd.xml - The tracking window</li>
    </ul>
  <br/>
  All of your textures and miscellaneous other files will also be in the folder:
  <ul>
    <li>Images</li>
    <li>Cursors</li>
    <li>Target Indicators</li>
    </ul>
</div>
  <br/>

<div class="step-container">

<h3>Creating a Custom UI Skin</h3>

<ul>

 <li>Log into the <a href="https://www.eqemulator.org/forums/">EQEmulator forum</a>.</li>

 <li>Create a Loginserver account <a href="https://www.eqemulator.org/account/?CreateLS">here</a>.</li>

</ul>

<img src="https://iili.io/2ZyduAQ.png" alt="Loginserver account creation">

</div>

<div class="step-container">

<h3>Verification Email</h3>

<p>If you don't receive a verification email, request another <a href="https://www.eqemulator.org/forums/register.php?do=requestemail">here</a>. Gmail users may experience issues.</p>

</div>

<div class="recommendation">

<strong>Recommended:</strong> Temporarily disable Windows Defender during installation. Navigate to <code>Windows Security</code> → <code>Virus & threat protection</code> → <code>Manage settings</code> and toggle <code>Real-time protection</code> off. Alternatively, type <code>!!exclude</code> in Discord for an exclusion tutorial.

</div>

<div class="step-container">

<h3>Step 3: Installer</h3>

 <li>Download the installer <a href="https://github.com/The-Heroes-Journey-EQEMU/thj-launcher/releases/latest/download/THJInstaller.zip">here</a>.</li>

 <li>Extract the ZIP file and run the <code>.exe</code> as administrator.</li>

 <li>If prompted by Windows, allow installation.</li>

 <li>If the download fails, delete the folder <code>Steam\\steamapps\\content\\app\_205710</code> and <code>C:\\THJ</code>, then retry.</li>

 <li>Restart Steam if running, and ensure other Steam applications are closed.</li>

</ul>

</div>

<div class="step-container">

<h3>Step 4: Play!</h3>

<ul>

 <li>Join <strong>The Heroes' Journey</strong> under legends servers. We look forward to seeing you in-game!</li>

</ul>

<img src="https://iili.io/2ZydUOl.png" alt="Heroes Journey Game">

</div>

<div class="step-container">

<h3>Optimizations</h3>

<p>Once installed, visit<a href="https://discord.com/channels/1204418766318862356/1332467859112071271"> Optimizations in Discord</a> and apply <strong>all</strong> recommended optimizations.</p>

</div>

</div>

<div class="installer-guide">

<div class="jump-buttons">

 <a href="#install-guide" class="jump-button">Installer Guide</a>

 <a href="#installer-faq" class="jump-button">Installer FAQ</a>

 </div>

<h2 id="manual-install">Manual Installer Guide</h2>

<p>Below is an alternative way to install, also found on the #getting-started page on our Discord. (And don't forget, we have an installer now!)</p>

<p>For more help, check out <a href="https://www.youtube.com/watch?v=qoZfkxzYRaY">Broken Stoic's install video</a>.</p>

<hr>

<div class="step-container">

<h3>Step 1: Create an EQEmulator Account</h3>

<ul>

 <li>Visit the <a href="https://www.eqemulator.org/forums/register.php">EQEmulator forum registration page</a>.</li>

 <li>Answer "What Game is this forum for?" with <strong>EverQuest</strong>.</li>

 <li>Ensure correct capitalization of your credentials.</li>

</ul>

</div>

<div class="step-container">

<h3>Step 2: Create a Loginserver Account</h3>

<ul>

 <li>Log into the <a href="https://www.eqemulator.org/forums/">EQEmulator forum</a>.</li>

 <li>Create a Loginserver account <a href="https://www.eqemulator.org/account/?CreateLS">here</a>.</li>

 <li>If you do not receive a verification email, request another one <a href="https://www.eqemulator.org/forums/register.php?do=requestemail">here</a>.</li>

</ul>

<img src="https://iili.io/2ZyduAQ.png" alt="Loginserver Account Creation">

</div>

<div class="step-container">

<h3>Step 3: Create a THJ Folder in Your C Drive</h3>

<ul>

 <li>Open <strong>File Explorer</strong> (<code>Windows + E</code>).</li>

 <li>Navigate to <strong>This PC → Local Disk (C:)</strong>.</li>

 <li>Right-click and select <strong>New Folder</strong>, then name it <strong>THJ</strong>.</li>

</ul>

</div>

<div class="step-container">

<h3>Step 4: Add EverQuest to Your Steam Library</h3>

<ul>

 <li>Open <strong>Steam</strong>.</li>

 <li>Search for <strong>EverQuest</strong> in the top-right search bar.</li>

 <li>Click <strong>Add to Library</strong>.</li>

 <li><strong>Do not download</strong> the game at this stage.</li>

</ul>

<img src="https://iili.io/2ZydbOQ.png" alt="Add EverQuest to Steam">

</div>

<div class="step-container">

<h3>Step 5: Open the Steam Console</h3>

<ul>

 <li>Press <code>Windows + R</code> to open the <strong>Run</strong> dialog.</li>

 <li>Copy and paste the command: <code>steam://open/console</code> and press Enter.</li>

</ul>

<img src="https://iili.io/2bgNwsj.png" alt="Steam Console">

</div>

<div class="step-container">

<h3>Step 6: Download the RoF2 Client</h3>

<ul>

 <li>Enter the command in Steam Console: <code>download\_depot 205710 205711 1926608638440811669</code></li>

 <li>Downloading will begin, but there is <strong>no progress bar</strong>. It may take time.</li>

</ul>

<img src="https://iili.io/2ZyFoKX.png" alt="Downloading RoF2 Client">

</div>

<div class="step-container">

<h3>Step 7: Locate and Copy the Downloaded Game Files</h3>

<ul>

 <li>Navigate to <code>%ProgramFiles(x86)%\\Steam\\steamapps\\content\\app\_205710\\depot\_205711</code>.</li>

 <li>Copy all the files inside <code>depot\_205711</code> and paste them into <code>C:\\THJ</code>.</li>

</ul>

<img src="https://iili.io/2bgvy8l.png" alt="Locating the Game Files">

</div>

<div class="step-container">

<h3>Step 8: Download and Install the Patcher</h3>

<ul>

 <li>Download <a href="https://github.com/The-Heroes-Journey-EQEMU/thj-patcher/releases/download/1.1.0.150/heroesjourneyemu.exe">heroesjourneyemu.exe</a>.</li>

 <li>Move it into <code>C:\\THJ</code> with your game files.</li>

</ul>

<img src="https://iili.io/2ZyTYF4.png" alt="THJ Folder Structure">

</div>

<div class="step-container">

<h3>Step 9: Verify the Patcher Setup</h3>

<ul>

 <li>Ensure <code>heroesjourneyeq.exe</code> is inside <code>C:\\THJ</code>.</li>

 <li>If missing <code>.dll</code> files, refer to <a href="https://discord.com/channels/1204418766318862356/1336713553079435294">this guide</a>.</li>

</ul>

</div>

<div class="step-container">

<h3>Step 10: Run the Patcher as Administrator</h3>

<ul>

 <li>Right-click <code>heroesjourneyeq.exe</code> → <strong>Properties</strong> → <strong>Compatibility</strong>.</li>

 <li>Check <strong>Run this program as an administrator</strong> and click OK.</li>

</ul>

<img src="https://iili.io/2bgrTdJ.png" alt="Creating a Shortcut">

</div>

<div class="step-container">

<h3>Step 11: Patch and Play</h3>

<ul>

 <li>Run <code>heroesjourneyeq.exe</code> and click the red <strong>Patch</strong> button.</li>

 <li>Once complete, launch the game and select <strong>The Heroes' Journey \[Multiclass Solo/Duo No-Box\]</strong>.</li>

</ul>

<img src="https://iili.io/2ZydUOl.png" alt="Server Selection">

</div>

</div>

<div class="faq-container">

<div class="jump-buttons">

 <a href="#install-guide" class="jump-button">Installer Guide</a>

 <a href="#manual-install" class="jump-button">Manual Installer Guide</a>

 </div>

   <h2 id="installer-faq"> Frequently Asked Questions and Help</h2>

   <h3> Common Issues and Fixes</h3>

   <div class="faq-item">

       <h4> Can't click on the UI or create a new character?</h4>

       <p>See the <a href="#amd-fix">AMD Fix</a> below.</p>

   </div>

   <div class="faq-item">

       <h4> Black screen when launching the game?</h4>

       <p>Press <code>Alt + Enter</code> <strong>twice</strong> or run the game in <strong>windowed mode</strong>.</p>

   </div>

   <div class="faq-item">

       <h4> DirectX issues?</h4>

       <p>Check the <a href="#directx-fix">DirectX Fix</a> below.</p>

   </div>

   <div class="faq-item">

       <h4> Crashing when zoning or experiencing random disconnects?</h4>

       <p>See the troubleshooting links:</p>

       <ul>

           <li><a href="https://discord.com/channels/1204418766318862356/1336716075890643026">Zone crashes</a></li>

           <li><a href="https://discord.com/channels/1204418766318862356/1336723062527365121">Random disconnects</a></li>

       </ul>

   </div>

   <div class="faq-item">

       <h4> Moving way too fast?</h4>

       <p>Check the <a href="#amd-fix">AMD Fix</a>.</p>

   </div>

   <h3 id="technical-fixes"> Technical Fixes</h3>

   <div class="faq-item">

       <h4 id="amd-fix"> Running on an AMD CPU?</h4>

       <p>You will need the <a href="https://github.com/xackery/eq-core-dll/releases">AMD fix</a>.  

       Download and place it in the same folder as <code>eqgame.exe</code>.</p>

   </div>

   <div class="faq-item">

       <h4 id="directx-fix"> Get the D3DX9\_30.dll Error?</h4>

       <p>You need to <strong>reinstall DirectX</strong> from <a href="https://www.microsoft.com/en-us/download/details.aspx?id=8109">here</a>.  

       Install it and try launching the game again.</p>

   </div>

   <div class="faq-item">

       <h4> Crashing when zoning? High memory usage?</h4>

       <p>Apply the <a href="https://ntcore.com/4gb-patch/">4GB Patch</a>.  

       This is <em>not</em> a large file—it simply enables <code>eqgame.exe</code> to use more memory.</p>

   </div>

   <h3> Further Support</h3>

   <p>For additional issues, check the troubleshooting channels on Discord:  

   <a href="https://discord.com/channels/1204418766318862356/1299429412902670397">Help and Support</a>.</p>

   <h2> Helpful Links</h2>

   <ul>

       <li><strong>Official Website:</strong> <a href="https://heroesjourneyemu.com">Heroes' Journey Website</a></li>

       <li><strong>Game Wiki:</strong> <a href="https://thj-wiki.web.app">The Heroes' Journey Wiki</a></li>

       <li><strong>Items and Database Info:</strong></li>

       <ul>

           <li><a href="https://info.heroesjourneyemu.com">Heroes' Journey Info</a></li>

           <li><a href="https://eqdb.net">THJ Database</a></li><br>

       </ul>

       <li><strong>FAQ on Discord:</strong> <a href="https://discord.com/channels/1204418766318862356/1317696921527390228">Discord FAQ</a></li>

       <li><strong>Community and Streams:</strong> <a href="https://www.twitch.tv/team/theheroesjourney">Heroes' Journey Twitch Team</a></li>

   </ul>

   <div class="centered-image">

       <img src="/pagebreak2.webp" alt="Page Break">

   </div>

</div>

</div>