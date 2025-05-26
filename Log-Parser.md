---
title: THJ Log Parser
description: Log Parser for THJ
published: false
date: 2025-05-26T15:04:01.775Z
tags: 
editor: markdown
dateCreated: 2025-05-26T13:36:37.110Z
---

<div class="page-wrapper">
  <div class="intro-section">
    <h1>THJLogParser Wiki</h1>
    <p><b>THJLogParser</b> is a powerful log parsing and analysis tool tailored for The Hero's Journey. Originally based on EQLogParser, it has been extensively customized to support THJ’s unique spells and abilities. The parser automatically loads your most recent log file and provides real-time overlays for DPS and other combat stats. It also features an advanced trigger system inspired by Gina Triggers, enabling you to create, manage, and test custom in-game alerts and automated responses—all within the application.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Getting Started</h2>
    <p>The parser is automatically installed by the THJ patcher and kept up to date as new versions are released. By default, all necessary files are placed in the <code>THJ/THJ Log parser</code> folder. <b>Do not move the parser executable or its folder</b>, as it relies on its directory structure to read spell files and ensure accurate parsing.</p>
    <ul>
      <li>Click the launch button on the THJ Patcher (recommended and easiest)</li>
      <li>Launch it directly from its installed location</li>
      <li>Create a shortcut to <code>THJLogParser.exe</code> on your desktop or taskbar for easier access—just make sure the shortcut points to the original folder and not a copied file</li>
    </ul>
    <p>No manual setup is required.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Features</h2>
    <ul>
      <li><b>Automatic Installation & Updates:</b> The THJ patcher automatically installs and keeps the parser up to date, ensuring you always have the latest features and fixes with no manual intervention required.</li>
      <li><b>Real-Time Log Parsing:</b> Instantly processes your most recent log file, providing up-to-date combat statistics and event tracking as you play.</li>
      <li><b>Damage Meter Overlay:</b> Displays a real-time DPS meter overlay in-game, with configuration options available from the parser's menu. The overlay defaults to [DPS] for intuitive use and can be customized to your preferences.</li>
      <li><b>Advanced Triggers System:</b> The built-in trigger system (inspired by Gina Triggers) allows you to create, manage, and test custom alerts for in-game events. Triggers can be configured and tested directly within the application, making it easy to set up notifications and automated responses for important log messages.</li>
      <li><b>Labeled Log Breaks:</b> You can now add labeled breaks to the log list by typing <code>/say log_break label</code> in your log. This feature lets you insert custom context into the logs, making it easier to track different parsing activities, such as when testers are running through various combinations of abilities and skills. It can also be used to break up an active fight into segments for more granular analysis.</li>
      <li><b>THJ-Specific Customization:</b> The parser is tailored for The Hero's Journey, with support for its unique spells, abilities, and log formats, ensuring accurate parsing and reporting.</li>
      <li><b>User-Friendly Launch Options:</b> Launch the parser directly, via a desktop/taskbar shortcut, or with a single click from the THJ Patcher for maximum convenience.</li>
            <li><b>Additional Search Options for Logs:</b> Enhanced log searching capabilities have been added, allowing you to filter and search logs more efficiently. These new options provide greater flexibility and speed when reviewing combat data, triggers, and labeled log breaks, making it easier to find the information you need.</li>
    </ul>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Damage Meter Overlay</h2>
    <p>The damage meter overlay provides a real-time, in-game display of your DPS and other combat statistics. It updates automatically as you play, allowing you to monitor your performance and compare results without leaving the game. The overlay is highly configurable—position, size, and display options can be adjusted to fit your preferences. By default, it shows [DPS] for quick and intuitive access, helping you stay focused on your gameplay while keeping important stats visible at all times.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Labeled Log Breaks</h2>
    <p>You can add labeled breaks to your log list by typing <code>/say log_break label</code> in your log file. This feature lets you insert custom context into the logs, making it easier to track different parsing activities, such as when testers are running through various combinations of abilities and skills. It can also be used to break up an active fight into segments for more granular analysis. These labeled breaks will appear in the parser, helping you organize and review your log data more effectively.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>GINA Style Triggers</h2>
    <p>The integrated GINA Style Triggers system allows you to create, manage, and test custom triggers for in-game events directly within the parser. Triggers can be set up to watch for specific log messages, keywords, or patterns, and can respond with alerts, notifications, or automated actions. The trigger editor provides an intuitive interface for adding new triggers, editing existing ones, and testing their behavior in real time. This system is fully integrated and designed to help you stay on top of important events, warnings, or opportunities as you play—without the need for external tools.</p>
    <div class="section-description">
      <b>Note:</b> For triggers to display notifications on your screen:
      <ul>
        <li>"Timer" triggers require a Timer overlay with "Default Overlay" enabled.</li>
        <li>"Text" triggers require a Text overlay with "Default Overlay" enabled.</li>
      </ul>
      <p>By default, the parser creates one Timer overlay and one Text overlay for you, so trigger notifications will work out of the box. If you remove these overlays or change their settings, you may need to re-enable or recreate them to see trigger alerts.</p>
    </div>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Performance Improvements</h2>
    <p>THJLogParser is continuously optimized for speed and efficiency. Recent updates have improved log processing times, reduced memory usage, and enhanced the responsiveness of overlays and the user interface. Notably, the parser now runs on .NET 8, providing significant performance and stability improvements over previous versions. These enhancements ensure smooth operation even with large log files or during intense gameplay sessions.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Fixes & Improvements</h2>
    <p>The parser receives regular bug fixes and quality-of-life enhancements. These include more accurate spell and damage parsing, better auto-sorting in breakdown panels, improved overlay defaults, and UI consistency updates. For a detailed list of changes, see the Changelog section below.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Troubleshooting</h2>
    <ul>
      <li>If the parser does not auto-load your log file, ensure your EverQuest log directory is set correctly and that the log file exists.</li>
      <li>If overlays are not visible, check that they are enabled in the parser and not hidden behind other windows. Also, verify that the required overlays (Timer/Text) are present and set as default for triggers.</li>
      <li>For trigger issues, confirm that your overlays have not been deleted or disabled. Recreate them if needed.</li>
      <li>Always use the THJ patcher to update the parser to the latest version for best results.</li>
      <li>For additional help or to report a bug, please use the <a href="https://github.com/BND10706/THJLogParser/issues">GitHub Issues section</a>.</li>
    </ul>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Feature Requests</h2>
    <p>Have an idea for a new feature or improvement? We welcome your suggestions! Please submit feature requests using the <a href="https://github.com/BND10706/THJLogParser/issues">GitHub Issues section</a> and tag your post with <b>[Feature Request]</b>. This helps us track and prioritize new ideas for future development.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Contributing</h2>
    <p>A special thank you to <b>Melkor</b> for all the hard work in developing EQLogParser and making it accessible to the community—this build is fully based on Melkor's foundation.</p>
    <p>An even bigger thanks to <b>Castleguard</b>, who has dedicated countless hours to this project. Nearly all major features and most improvements in this build are thanks to Castleguard's ongoing contributions.</p>
    <p>Contributions, feedback, and bug reports are welcome! Please use the <a href="https://github.com/BND10706/THJLogParser">GitHub repository</a> to submit issues or pull requests. Help improve the parser for the whole THJ community.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Changelog</h2>
    <p>Below is a summary of recent changes.</p>
    <hr />
    <h3>Version 1.0.1.0 (May 24, 2025)</h3>
    <b>New Features</b>
    <ul>
      <li>Auto-load Recent Log: Parser now automatically loads your most recently-opened log file when started</li>
      <li>In-game Damage Meter: Damage meter overlay now functions including configuration (available via View -> Damage Meter menu)</li>
      <li>Header Menu Consistency: Header menu consistency cleaned up</li>
      <li>TRIGGERS!: Gina Triggers functionality is now operational via View -> Triggers menu. Check Wiki for documentation.</li>
      <li>DPS Meter Overlay Default: DPS meter overlay now selects [DPS] by default to correct unintuitive usability on first use</li>
      <li>Trigger Panel Resize: Added resize sliders to Trigger configuration panel edges</li>
      <li>Labeled Log Breaks: Added the ability to add labeled breaks to the log list by typing <code>/say log_break label</code> in your log. This allows you to add context to the logs for tracking parsing activities or breaking up active fights into segments.</li>
    </ul>
    <b>Performance Improvements</b>
    <ul>
      <li>Upgraded to .NET 8 for improved speed and stability</li>
      <li>More performance improvements</li>
    </ul>
    <b>Fixes & Improvements</b>
    <ul>
      <li>Fixed damage breakdown auto-sorting so that it actually auto-sorts by total damage when the panel opens rather than lying to you</li>
    </ul>
    <hr />
    <h3>Version 1.0.0.0</h3>
    <b>New Features</b>
    <ul>
      <li>One-click Screenshot: Fast screenshots with frames via the "Copy Parse to Clipboard" button on Breakdown views</li>
      <li>Pet Tracking Improvement: Now correctly tracks and includes "Pets of Pets" (such as swarm proc weapons)</li>
      <li>Additional Data Column: New "Min Damage" column option available in damage breakdowns to show minimum hit values</li>
    </ul>
    <b>Performance Improvements</b>
    <ul>
      <li>Optimized Log Processing: Significantly faster parsing and processing of log files</li>
      <li>Enhanced DPS Calculation: More accurate DPS calculations based on actual damage-per-encounter-time</li>
    </ul>
    <b>Fixes & Improvements</b>
    <ul>
      <li>Spell Classification: Spells now correctly categorized as Direct Damage (DD) vs Damage over Time (DoT) based on the game's spell dictionary</li>
    </ul>
    <hr />
  </div>
</div>
