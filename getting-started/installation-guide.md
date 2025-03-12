---
title: Installation Guide
description: 
published: true
date: 2025-03-12T20:17:56.974Z
tags: 
editor: markdown
dateCreated: 2025-02-26T19:27:47.188Z
---

![gettingstartedbanner.webp](/gettingstartedbanner.webp){.align-center}

# Windows Install
> Below is a way to install, also found on the #getting-started page on our discord. (and don't forget we have an installer now!)

## INSTALLATION INSTRUCTIONS

This guide will walk you through the process of setting up everything needed to play. Follow these steps carefully.

> You can also check out Broken Stoic's install video for more help: https://www.youtube.com/watch?v=qoZfkxzYRaY 

(We recommend our installer, on the #getting-started on the discord.)

---

## **Step 1: Create an EQEmulator Account**
Before logging into the game, you need an account on EQEmulator.

1. Visit the [EQEmulator forum registration page](https://www.eqemulator.org/forums/register.php).
2. When asked, *"What Game is this forum for?"*, the answer is **EverQuest**.
3. Ensure you correctly capitalize your credentials, as formatting matters.

---

## **Step 2: Create a Loginserver Account on EQEmulator**
Once you have an EQEmulator account, you need a loginserver account to access the game.

1. Log into the [EQEmulator forum](https://www.eqemulator.org/forums/).
2. Visit the [loginserver account creation page](https://www.eqemulator.org/account/?CreateLS).
3. Ensure you're logged in before proceeding.
4. If you do not receive a verification email, request another one [here](https://www.eqemulator.org/forums/register.php?do=requestemail).

![Loginserver Account Creation](https://iili.io/2ZyduAQ.png)

---

## **Step 3: Create a THJ Folder in Your C Drive**
You need to create a dedicated folder for THJ.

1. Open **File Explorer** (`Windows + E`).
2. In the left panel, navigate to **This PC**.
3. Click on **Local Disk (C:)**.
4. Right-click and select **New Folder**.
5. Name it **THJ**.

This ensures there are no permission issues that might arise from installing in `Program Files`.

---

## **Step 4: Add EverQuest to Your Steam Library**
We are obtaining the **RoF2 client** from Steam but **not** downloading EverQuest.

1. Open **Steam**.
2. Search for **EverQuest** in the top-right search bar.
3. Scroll down and click **Add to Library**.
4. **Do not download** the game at this stage.

![Add EverQuest to Steam](https://iili.io/2ZydbOQ.png)

---

## **Step 5: Open the Steam Console**
The Steam Console allows us to download specific game files.

1. Press `Windows + R` to open the **Run** dialog.
2. Copy and paste the following command:
   ```
   steam://open/console
   ```
3. Press **Enter**.
4. The Steam Console tab will now be visible.

[Explanation of what this does](https://discord.com/channels/1204418766318862356/1333166462650548346).

![Steam Console](https://iili.io/2bgNwsj.png)

---

## **Step 6: Download the RoF2 Client**
Now, use the Steam Console to download the required client files.

1. In the Steam Console, enter the following command:
   ```
   download_depot 205710 205711 1926608638440811669
   ```
2. Once downloading begins, you'll see a message like:
   ```
   downloading depot 205711
   ```
3. There is **no progress bar**, and the process may take a few hours.

![Downloading RoF2 Client](https://iili.io/2ZyFoKX.png)

---

## **Step 7: Locate and Copy the Downloaded Game Files**
After your **depot download** is complete, follow these steps:

1. Navigate to the folder:
   ```
   %ProgramFiles(x86)%\Steam\steamapps\content\app_205710\depot_205711
   ```
2. Open the **`depot_205711`** folder.
3. Copy all the contents inside.
4. Paste them into your **`C:\THJ`** folder.

At this point, you should have the **RoF2 client** correctly installed—not a live EverQuest client or P99.

![Locating the Game Files](https://iili.io/2bgvy8l.png)

---

## **Step 8: Download and Install the Patcher**
To ensure you receive updates and patches for **The Heroes' Journey**, download and install the patcher.

1. Download **heroesjourneyeq.exe** from [here](https://github.com/The-Heroes-Journey-EQEMU/eqemupatcher/releases/latest/download/heroesjourneyeq.exe).
2. Move **heroesjourneyeq.exe** into **`C:\THJ`** alongside the rest of your game files.
3. Your **C:\THJ** folder should now resemble the following image:

![THJ Folder Structure](https://iili.io/2ZyTYF4.png)

---

## **Step 9: Verify the Patcher is in the Correct Folder**
Before proceeding, ensure everything is set up properly:

- **`heroesjourneyeq.exe` must be in the same folder as your EQ files**, or you will receive a *file not found* error.
- If you are missing **.dll files**, refer to [this guide](https://discord.com/channels/1204418766318862356/1336713553079435294).
- If you receive a **"Cannot find file specified"** error, double-check that **heroesjourneyeq.exe** is in `C:\THJ`.

---

## **Step 10: Run the Patcher as Administrator and Create a Shortcut**
To ensure smooth operation, configure the patcher to run with administrator privileges.

1. **Right-click** on `heroesjourneyeq.exe`.
2. Select **Properties** → **Compatibility Tab**.
3. Check **Run this program as an administrator** and click **OK**.
4. **Create a shortcut**:
   - Right-click **heroesjourneyeq.exe**.
   - Select **Create Shortcut**.
   - Move this shortcut to your desktop.
   - Rename it to **THJ** (optional).

Now, you can easily launch the game from your desktop!

![Creating a Shortcut](https://iili.io/2bgrTdJ.png)

---

## **Step 11: Run the Patcher**
1. Open **heroesjourneyeq.exe**.
2. The patcher window will appear.
3. Click the **big red Patch button**.
4. Let it patch the game files—this may take some time.

---

## **Step 12: Find the Server and Play**
Once the patching process is complete:

1. Launch the game.
2. Locate the **"The Heroes' Journey [Multiclass Solo/Duo No-Box]"** server.
3. Select the server and hit **Play**.

![Server Selection](https://iili.io/2ZydUOl.png)

---

## **Step 13: Optimizations (Highly Recommended)**
To prevent crashes and improve performance, follow the recommended optimizations:

- [Check out the optimization guide on discord.](https://discord.com/channels/1204418766318862356/1332467859112071271).
- Certain settings can **prevent crashes** (such as `dinput8.dll` errors and out-of-memory issues).
- Players and contributors have compiled fixes to improve gameplay stability.


---

## **Frequently Asked Questions and Help**

### Common Issues and Fixes

#### **Can't click on the UI or create a new character?**  
- See the [AMD Fix](#running-on-an-amd-cpu) below.

#### **Black screen when launching the game?**  
- Press `Alt + Enter` **twice** or run the game in **windowed mode**.

#### **DirectX issues?**  
- Check the [DirectX Fix](#get-the-d3dx9_30dll-error) below.

#### **Crashing when zoning or experiencing random disconnects?**  
- See the troubleshooting links:  
  - [Zone crashes](https://discord.com/channels/1204418766318862356/1336716075890643026)  
  - [Random disconnects](https://discord.com/channels/1204418766318862356/1336723062527365121)

#### **Moving way too fast?**  
- Check the [AMD Fix](#running-on-an-amd-cpu).

---

## **Technical Fixes**

### **Running on an AMD CPU?**
- You will need the [AMD fix](https://github.com/xackery/eq-core-dll/releases).  
- Download and place it in the same folder as **eqgame.exe**.

---

### **Get the D3DX9_30.dll Error?**
- You need to **reinstall DirectX** from [here](https://www.microsoft.com/en-us/download/details.aspx?id=8109).  
- Install it and try launching the game again.

---

### **Crashing when zoning? High memory usage?**
- Apply the **4GB Patch** from [here](https://ntcore.com/4gb-patch/).  
- This is *not* a large file—it simply enables **eqgame.exe** to use more memory.

---

### **Further Support**
For additional issues, check the troubleshooting channels on Discord:  
[Help and Support](https://discord.com/channels/1204418766318862356/1299429412902670397).

---

## **Helpful Links**

### **Official Website**  
[Heroes' Journey Website](https://heroesjourneyemu.com)

### **Game Wiki**  
[The Heroes' Journey Wiki](https://thj-wiki.web.app)

### **Items and Database Info**  
- [Heroes' Journey Info](https://info.heroesjourneyemu.com)  
- [THJ Database](https://www.thjdi.cc)

### **FAQ on Discord**  
[Discord FAQ](https://discord.com/channels/1204418766318862356/1317696921527390228)

### **Community and Streams**  
[Heroes' Journey Twitch Team](https://www.twitch.tv/team/theheroesjourney)

---

![pagebreak2.webp](/pagebreak2.webp){.align-center}