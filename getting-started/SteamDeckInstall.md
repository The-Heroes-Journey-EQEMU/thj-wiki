---
title: Steam Deck Installation Guide
description: A quick guide on installing and configuring THJ & required components to allow you to take your Heroic Journey mobile on the Steam Deck!
published: true
date: 2025-04-30T13:05:43.222Z
tags: getting started, installation guide, steam deck, steamos, steam
editor: markdown
dateCreated: 2025-03-18T00:24:38.253Z
---

# Steam Deck Install
---

<div class="step-container">
  <h3>Step 1: Create an EQEmulator Account</h3>
Before logging into the game, you need an account on EQEmulator.
<ol>
<li> Visit the <a href="https://www.eqemulator.org/forums/register.php">EQEmulator forum registration page.</a>
  <li> When asked, "<b>What Game is this forum for?</b>", the answer is <b>EverQuest</b>.
<li> Ensure you correctly capitalize your credentials, as formatting matters.

---

## **Step 2: Create a Loginserver Account on EQEmulator**
Once you have an EQEmulator account, you need a loginserver account to access the game.

1. Log into the [EQEmulator forum](https://www.eqemulator.org/forums/).
2. Visit the [loginserver account creation page](https://www.eqemulator.org/account/?CreateLS).
3. Ensure you're logged in before proceeding.
4. If you do not receive a verification email, request another one [here](https://www.eqemulator.org/forums/register.php?do=requestemail).

![Loginserver Account Creation](https://iili.io/2ZyduAQ.png)

---

## **Step 3: Create a Games\THJ Folder in Your Home Directory**
You need to create a dedicated folder for the THJ install. Mouse and keyboard recommended, or use Steam Link.

1. Start your Steam Deck and ensure Developer Mode is enabled
	- This is found in Settings in Game Mode
2. Enter Desktop Mode
3. In your taskbar, open Dolphin
4. Click on **Home**.
5. Click on the hamburger menu (<img src="https://iili.io/3oMizYX.png" alt="hamburger menu" height="20" width="20">) and select **Create New --> Folder**.
6. Name the folder **Games**.
7. Enter the **Games** folder and repeat step 4, naming the folder **THJ**.
![3oMQfQj.md.png](https://iili.io/3oMQfQj.md.png)

- - -

## **Step 4: Add EverQuest to Your Steam Library**
We are obtaining the **RoF2 client** from Steam but **not** downloading EverQuest.

1. Open **Steam**.
2. Search for **EverQuest** in the top-right search bar.
3. Scroll down and click **Add to Library**.
4. **Do not download** the game at this stage.

![Add EverQuest to Steam](https://iili.io/2ZydbOQ.png)

---
## Step 5: Install Everquest from Steam Depot
1. Still in Desktop mode, go to Discover and download Konsole
2. Launch Konsole and enter the below command
```
Steam Steam://open/console
```
3. The Steam console will open. Enter the below command
```
download_depot 205710 205711 1926608638440811669
```
4. Once the download begins, you'll see a message like : 
```
downloading depot 205711
```
5. There is **no progress bar**, and the process may take several hours depending on your internet speeds.
![Downloading RoF2 Client](https://iili.io/2ZyFoKX.png)
6. One the download has completed, navigate to the depot folder, copy the files in it, and paste them into the THJ folder you created in Step 3.

- - -

## Step 6: Install Bottles & Flatseal
SteamOS doesn't come packaged with Wine, so it doesn't know how to handle executables. We need to use a wrapper so SteamOS can launch the game. That's where Bottles (or Lutris, if you prefer) come in.

1. On your Steam Deck, launch Discover.
2. Search for Bottles and install
	 ![3oMDeFR.png](https://iili.io/3oMDeFR.png)
3. Search for and install Flatseal
	 ![3oMmc7V.png](https://iili.io/3oMmc7V.png)

- - -

## Step 7: Configure your Bottle
Bottles is a wrapper that effectively "translates" Windows commands into ones that Linux can handle, allowing us to run executables

1. Launch Bottles and find the button to create a new Bottle (<img src="https://iili.io/3oMyAUx.png" alt="plus button" width="20" height="20">)
2. Create a new Gaming bottle - name it whatever you like
	 - Bottles will handle creating the Bottle and config. Just let it run until it says Bottle Created
3. Select Add Shortcuts...
4. Navigate to your THJ Install folder and select the patcher executable.
5. Select the launcher submenu and select "Change Launch Options"
  ![3oVT6kN.md.png|400](https://iili.io/3oVT6kN.md.png)
7. In Command Arguments, enter the below:
	- WINEDLLOVERRIDES="dinput8=n,b" %command%
	- Click Save
8. Select the Settings menu and set the following - 
	- FidelityFX Super Resolution - OFF
	- Discrete Graphics - ON
	- Post-Processing Effects & Gamescope - OFF
	- Advanced Display Settings
		-  Virtual Desktop & Mouse Warp- OFF
		-  Fullscreen Mouse Capture, Take Focus & Window Manager Decorations - ON
	- All Performance options - OFF
	- Windows Version - 11
	- Steam Runtime - ON
	- DLL Overrides **THIS IS IMPORTANT**
		- Enter "DINPUT8.DLL" (no quotes) in New Override, click the blue check.
		- Ensure the overide is Native, then Builtin
		![3oVza3l.md.png|400](https://iili.io/3oVza3l.md.png)

---

## Step 8: Configure FlatSeal & Set Permissions
Flatseal gives us the ability to manage flatpak permissions to modify files in the game directory. This is necessary for patching.

1. Launch Flatseal and select Bottles on the left
2. Scroll down and find Filesystem - enable all four toggles
3. Find your ~/Games folder in Dolphin & right click
4. Select Properties
5. Select Permissions
6. Access Permissions
	1. Set all to Can View & Modify Content
7. Ownership
	1. Change the Group to the group your Steam deck user is (mine's Deck)
8. Click Okay, navigate to the patcher in your folder & run the .exe

### Common Issues
- Access Denied during patching
	- You have misconfigured file permissions somewhere. Double check everything is set as instructed in this guide in steps 7 & 8
- Getting spammed in game about game version
	- This is an issue with the dinput8.dll override. Most common issue here is a typo when setting the override. Refer back to step 7.
- All black textures when game launches
	- Most commonly seen with incomplete downloads, or clients downloaded on PC and transferred to the Deck. The ROF files **must** be downloaded onto your deck directly via Steam.
