---
title: Steam Deck Installation Guide
description: A quick guide on installing and configuring THJ & required components to allow you to take your Heroic Journey mobile on the Steam Deck!
published: true
date: 2025-05-28T20:40:43.958Z
tags: 
editor: markdown
dateCreated: 2025-03-18T00:24:38.253Z
---

# Steam Deck Install
<div class="jump-buttons">
  <a href="#common-issues" class="jump-buttons">Common Issues</a>
  <a href="https://www.reddit.com/r/project1999/comments/11xn4j2/steam_deck_control_scheme/">Control Scheme</a>
  </div>
  
  <div class="step-container">
  <h3>Step 1: Create an EQEmulator Account</h3>
Before logging into the game, you need an account on EQEmulator.
  <ol>
    <li> Visit the <a href="https://www.eqemulator.org/forums/register.php">EQEmulator forum registration page.</a></li>
    <li> When asked, "<b>What Game is this forum for?</b>", the answer is <b>EverQuest</b>.</li>
    <li> Ensure you correctly capitalize your credentials, as formatting matters.</li>
  </ol>
    </div>
  
---

<div class="step-container">
  <h3>Step 2: Create a Loginserver Account on EQEmulator</h3>
Once you have an EQEmulator account, you need a loginserver account to access the game.

<ol>
  <li> Log into the <a href="https://www.eqemulator.org/forums/">EQEmulator forum</a>.</li>
<li> Visit the <a href="https://www.eqemulator.org/account/?CreateLS">loginserver account creation page.</a></li>
  <li> Ensure you're logged in before proceeding.</li>
<li> If you do not receive a verification email, request another one <a href="https://www.eqemulator.org/forums/register.php?do=requestemail">here</a>.</li>
  </ol>
  <br>
<img src="https://iili.io/2ZyduAQ.png" alt="EQEmu Nav Pane">
  </div>
  
---

  <div class="step-container">
  <p align="center"><i>*NOTE*</i>
    <br>The entirety of this guide (with the exception of step 3.1 to verify Developer Mode is enabled) should be followed on the Steam Deck in Desktop Mode. Once everything is complete you can add it to your library as a non-Steam game to launch from Gaming mode.</p>
    <h3>Step 3: Create a Games\THJ Folder in Your Home Directory</h3>
		<p>You need to create a dedicated folder for the THJ install. Mouse and keyboard recommended, or use Steam Link.</p>
    <ol>
      <li> Start your Steam Deck and ensure Developer Mode is enabled</li>
        <ul>
          <li>This is found under Settings while in Game Mode</li>
        </ul>
      <li> In your taskbar, open Dolphin</li>
      <li> Click on <b>Home</b>.</li>
      <li> Click on the hamburger menu (<img src="https://iili.io/3oMizYX.png" alt="hamburger menu" height="20" width="20">) and select <b>Create New --> Folder</b>.</li>
      <li> Name the folder <b>Games</b>.</li>
      <li> Enter the <b>Games</b> folder and repeat step 5, naming the folder <b>THJ</b>.</li>
      <img src="https://iili.io/3oMQfQj.md.png" alt="THJ Folder in Games directory">
  </ol>
  </div>

- - -

  <div class="step-container">
  <h3>Step 4: Add EverQuest to Your Steam Library</h3>
    <p>We are obtaining the <b>RoF2 client</b> from Steam but <b>not</b> downloading EverQuest.</p>

<ol>
  <li> Open <b>Steam</b>.</li>
  <li> Search for <b>EverQuest</b> in the top-right search bar.</li>
  <li> Scroll down and click <b>Add to Library</b>.</li>
  <li> <b>Do not download</b> the game at this stage.</li>
	<br>
  <img src="https://iili.io/2ZydbOQ.png" alt="Everquest add to library button">
  </ol>
  </div>

---
  
  <div class="step-container">
    <h3>Step 5: Install Everquest from Steam Depot</h3>
    <ol>
      <p align="center"><i>NOTE</i>
        <br>Transferring the install files from desktop to the deck will not work. Game files must be downloaded directly to the Deck.</p><br>
      <li>In your task bar, launch Discover and download Konsole</li>
      <li>Launch Konsole and enter the below command
        <pre><code>steam steam://open/console</code></pre></li>
			<li> The Steam console will open. Enter the below command
        <pre><code>download_depot 205710 205711 1926608638440811669</code></pre></li>
			<li>Once the download begins, you'll see a message like this: 
        <pre><code>downloading depot 205711</code></pre></li>
      <li> There is <b>no progress bar</b>, and the process may take several hours depending on your internet speeds.<br></li>
<img src="https://iili.io/2ZyFoKX.png" alt="Steam console download status">
			<li> One the download has completed, navigate to the depot folder, copy the files in it, and paste them into the THJ folder you created in Step 3.</li>
    </ol>
      </div>
  
---

<div class="step-container">
<h3>Step 6: Download and Install the Patcher</h3>
<ol>
  <li>Download <a href="https://github.com/The-Heroes-Journey-EQEMU/thj-patcher/releases/download/1.1.0.150/heroesjourneyemu.exe">heroesjourneyemu.exe</a>.</li>
  <li>Move it into <code>~/Games/THJ</code> with your game files.</li>
</ol>
<img src="https://iili.io/2ZyTYF4.png" alt="THJ Folder Structure">
</div>
  
---

<div class="step-container">
  <h3>Step 7: Install Bottles & Flatseal</h3>
<p>SteamOS doesn't come packaged with Wine, so it doesn't know how to handle executables. We need to use a wrapper so SteamOS can launch the game. That's where Bottles (or Lutris, if you prefer) come in.</p>
	<ol>
    <li> On your Steam Deck, launch Discover.</li>
    <li> Search for Bottles and install</li>
      <br>
<img src="https://iili.io/3oMDeFR.png" alt="Bottles on Discover">
    <li> Search for and install Flatseal</li>
      <br>
      <img src="https://iili.io/3oMmc7V.png" alt="Flatseal on Discover">
  </ol>
</div>

---

<div class="step-container">
  <h3>Step 8: Configure your Bottle</h3>
<p>Bottles is a wrapper that effectively "translates" Windows commands into ones that Linux can handle, allowing us to run executables</p>

<ol>
<li> Launch Bottles and find the button to create a new Bottle (<img src="https://iili.io/3oMyAUx.png" alt="plus button" width="20" height="20">)</li>
  <li>Create a new Gaming bottle - name it whatever you like</li>
  <ul>
	 <li> Bottles will handle creating the Bottle and config. Just let it run until it says Bottle Created</li>
  </ul>
  <li> Select Add Shortcuts...</li>
  <li> Navigate to your THJ Install folder and select the patcher executable.</li>
  <li> Select the launcher submenu and select "Change Launch Options"</li>
  <img src="https://iili.io/3oVT6kN.md.png" alt="Change Launch options">
  <li> In Command Arguments, enter the below:</li>
  <ul>
    <li><pre><code>WINEDLLOVERRIDES="dinput8=n,b" %command%</code></pre></li>
    <li>Click Save</li>
  </ul>
  <li> Select the Settings menu and set the following:</li>
	<ul>
    <li> FidelityFX Super Resolution - OFF</li>
    <li> Discrete Graphics - ON</li>
    <li> Post-Processing Effects & Gamescope - OFF</li>
  </ul>
  <li> Advanced Display Settings</li>
    <ul>
      <li> Virtual Desktop & Mouse Warp -OFF</li>
      <li> Fullscreen Mouse Capture, Take Focus & Window Manager Decorations - ON</li>
    </ul>
  <li>All Performance options - OFF</li>
  <li> Windows Version - 11</li>
  <li> Steam Runtime - ON</li>
  <li> DLL Overrides <b>THIS IS IMPORTANT</b></li>
    <ul>
      <li> Enter <pre><code>DINPUT8.DLL</code></pre> in New Override, then click the blue check.</li>
      <li> Ensure the overide is Native, then Builtin</li>
    </ul>
  </ol>
  <br>
		<img src="https://iili.io/3oVza3l.md.png" alt="DLL Override">
  </div>


---

<div class="step-container">
  <h3>Step 9: Configure FlatSeal & Set Permissions</h3>
<p>Flatseal gives us the ability to manage flatpak permissions to modify files in the game directory. This is necessary for patching.</p>
  
<ol>
  <li> Launch Flatseal and select Bottles on the left</li>
  <li> Scroll down and find Filesystem - enable all four toggles</li>
  <li> Find your ~/Games folder in Dolphin & right click</li>
  <li> Select Properties</li>
  <li> Select Permissions</li>
  <li> Access Permissions</li>
  <ul>
    <li> Set all to Can View & Modify Content</li>
  </ul>
  <li> Ownership</li>
  <ul>
    <li> Change the Group to the group your Steam deck user is (mine's Deck)</li>
  </ul>
  <li> Click Okay, navigate to the patcher in your folder & run the .exe</li>
  </ol>
  </div>

  ---
  
<div class="faq-container">
<div class="jump-buttons">
  </div>
    <h2 id="common-issues">Common Issues</h2>
<div class="faq-item">    
  <h4>Access Denied during patching</h4>
  <ul><li><p>You have misconfigured file permissions somewhere. Double check everything is set as instructed in this guide in steps 7 & 8</p></ul></div>
<div class="faq-item">
  <h4>Getting spammed in game about game version</h4>
<ul><li><p>This is an issue with the dinput8.dll override. Most common issue here is a typo when setting the override. Refer back to step 7.</p></ul></div>
<div class="faq-item">
  <h4>All black textures when game launches</h4>
<ul><li><p>Most commonly seen with incomplete downloads, or clients downloaded on PC and transferred to the Deck. The ROF files <b>must</b> be downloaded onto your deck directly via Steam.</p></ul></div>
