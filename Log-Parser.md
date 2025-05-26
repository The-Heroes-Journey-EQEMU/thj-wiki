---
title: THJ Log Parser
description: Log Parser for THJ
published: false
date: 2025-05-26T14:40:49.282Z
tags: 
editor: markdown
dateCreated: 2025-05-26T13:36:37.110Z
---

# THJLogParser Wiki

## Overview

**THJLogParser** is a powerful log parsing and analysis tool tailored for The Hero's Journey. Originally based on EQLogParser, it has been extensively customized to support THJ’s unique spells and abilities. The parser automatically loads your most recent log file and provides real-time overlays for DPS and other combat stats. It also features an advanced trigger system inspired by Gina Triggers, enabling you to create, manage, and test custom in-game alerts and automated responses—all within the application.

## Getting Started

The parser is automatically installed by the THJ patcher and kept up to date as new versions are released. By default, all necessary files are placed in the `THJ/THJ Log parser` folder. **Do not move the parser executable or its folder**, as it relies on its directory structure to read spell files and ensure accurate parsing.

To use the parser, you can:

- Click the launch button on the THJ Patcher (recommended and easiest)
- Launch it directly from its installed location
- Create a shortcut to `THJLogParser.exe` on your desktop or taskbar for easier access—just make sure the shortcut points to the original folder and not a copied file

No manual setup is required.

## Features

- **Automatic Installation & Updates:** The THJ patcher automatically installs and keeps the parser up to date, ensuring you always have the latest features and fixes with no manual intervention required.

- **Real-Time Log Parsing:** Instantly processes your most recent log file, providing up-to-date combat statistics and event tracking as you play.

- **Damage Meter Overlay:** Displays a real-time DPS meter overlay in-game, with configuration options available from the parser's menu. The overlay defaults to [DPS] for intuitive use and can be customized to your preferences.

- **Advanced Triggers System:** The built-in trigger system (inspired by Gina Triggers)allows you to create, manage, and test custom alerts for in-game events. Triggers can be configured and tested directly within the application, making it easy to set up notifications and automated responses for important log messages.

- **Labeled Log Breaks:** You can now add labeled breaks to the log list by typing `/say log_break label` in your log. This feature lets you insert custom context into the logs, making it easier to track different parsing activities, such as when testers are running through various combinations of abilities and skills. It can also be used to break up an active fight into segments for more granular analysis.

- **THJ-Specific Customization:** The parser is tailored for The Hero's Journey, with support for its unique spells, abilities, and log formats, ensuring accurate parsing and reporting.

- **User-Friendly Launch Options:** Launch the parser directly, via a desktop/taskbar shortcut, or with a single click from the THJ Patcher for maximum convenience.

## Damage Meter Overlay

The damage meter overlay provides a real-time, in-game display of your DPS and other combat statistics. It updates automatically as you play, allowing you to monitor your performance and compare results without leaving the game. The overlay is highly configurable—position, size, and display options can be adjusted to fit your preferences. By default, it shows [DPS] for quick and intuitive access, helping you stay focused on your gameplay while keeping important stats visible at all times.

## Gina Triggers

The integrated Gina Triggers system allows you to create, manage, and test custom triggers for in-game events directly within the parser. Triggers can be set up to watch for specific log messages, keywords, or patterns, and can respond with alerts, notifications, or automated actions. The trigger editor provides an intuitive interface for adding new triggers, editing existing ones, and testing their behavior in real time. This system is fully integrated and designed to help you stay on top of important events, warnings, or opportunities as you play—without the need for external tools.

**Note:** For triggers to display notifications on your screen:

- "Timer" triggers require a Timer overlay with "Default Overlay" enabled.
- "Text" triggers require a Text overlay with "Default Overlay" enabled.

By default, the parser creates one Timer overlay and one Text overlay for you, so trigger notifications will work out of the box. If you remove these overlays or change their settings, you may need to re-enable or recreate them to see trigger alerts.

## Performance Improvements

THJLogParser is continuously optimized for speed and efficiency. Recent updates have improved log processing times, reduced memory usage, and enhanced the responsiveness of overlays and the user interface. Notably, the parser now runs on .NET 8, providing significant performance and stability improvements over previous versions. These enhancements ensure smooth operation even with large log files or during intense gameplay sessions.

## Fixes & Improvements

The parser receives regular bug fixes and quality-of-life enhancements. These include more accurate spell and damage parsing, better auto-sorting in breakdown panels, improved overlay defaults, and UI consistency updates. For a detailed list of changes, see the Changelog section below.

## Troubleshooting

- If the parser does not auto-load your log file, ensure your EverQuest log directory is set correctly and that the log file exists.
- If overlays are not visible, check that they are enabled in the parser and not hidden behind other windows. Also, verify that the required overlays (Timer/Text) are present and set as default for triggers.
- For trigger issues, confirm that your overlays have not been deleted or disabled. Recreate them if needed.
- Always use the THJ patcher to update the parser to the latest version for best results.
- For additional help or to report a bug, please use the [GitHub Issues section](https://github.com/BND10706/THJLogParser/issues).

## Feature Requests

Have an idea for a new feature or improvement? We welcome your suggestions! Please submit feature requests using the [GitHub Issues section](https://github.com/BND10706/THJLogParser/issues) and tag your post with **[Feature Request]**. This helps us track and prioritize new ideas for future development.

## Contributing

A special thank you to **Melkor** for all the hard work in developing EQLogParser and making it accessible to the community—this build is fully based on Melkor's foundation.

An even bigger thanks to **Castleguard**, who has dedicated countless hours to this project. Nearly all major features and most improvements in this build are thanks to Castleguard's ongoing contributions.

Contributions, feedback, and bug reports are welcome! Please use the [GitHub repository](https://github.com/BND10706/THJLogParser) to submit issues or pull requests. Help improve the parser for the whole THJ community.

## Changelog

Below is a summary of recent changes.

---

### Version 1.0.1.0 (May 24, 2025)

**New Features**

- Auto-load Recent Log: Parser now automatically loads your most recently-opened log file when started
- In-game Damage Meter: Damage meter overlay now functions including configuration (available via View -> Damage Meter menu)
- Header Menu Consistency: Header menu consistency cleaned up
- TRIGGERS!: Gina Triggers functionality is now operational via View -> Triggers menu. Check Wiki for documentation.
- DPS Meter Overlay Default: DPS meter overlay now selects [DPS] by default to correct unintuitive usability on first use
- Trigger Panel Resize: Added resize sliders to Trigger configuration panel edges
- Labeled Log Breaks: Added the ability to add labeled breaks to the log list by typing `/say log_break label` in your log. This allows you to add context to the logs for tracking parsing activities or breaking up active fights into segments.

**Performance Improvements**

- Upgraded to .NET 8 for improved speed and stability
- More performance improvements

**Fixes & Improvements**

- Fixed damage breakdown auto-sorting so that it actually auto-sorts by total damage when the panel opens rather than lying to you

---

### Version 1.0.0.0

**New Features**

- One-click Screenshot: Fast screenshots with frames via the "Copy Parse to Clipboard" button on Breakdown views
- Pet Tracking Improvement: Now correctly tracks and includes "Pets of Pets" (such as swarm proc weapons)
- Additional Data Column: New "Min Damage" column option available in damage breakdowns to show minimum hit values

**Performance Improvements**

- Optimized Log Processing: Significantly faster parsing and processing of log files
- Enhanced DPS Calculation: More accurate DPS calculations based on actual damage-per-encounter-time

**Fixes & Improvements**

- Spell Classification: Spells now correctly categorized as Direct Damage (DD) vs Damage over Time (DoT) based on the game's spell dictionary

---

For more details and previous versions, refer to the full [CHANGELOG.md](EQLogParser/CHANGELOG.md).
