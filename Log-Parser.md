---
title: THJ Log Parser
description: Log Parser for THJ
published: true
date: 2025-05-26T21:33:56.781Z
tags: 
editor: markdown
dateCreated: 2025-05-26T13:36:37.110Z
---


<img src="/log-parser/logparsericon.png" alt="Labeled Log Break Example" class="wiki-image" />
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
        <p><b>To enable combat logging:</b> Edit the <code>EQClient.ini</code> file in your EverQuest installation folder. Locate the <code>Log</code> setting and change it from <code>FALSE</code> to <code>TRUE</code>. You can also enable logging in-game on a session-by-session basis using the commands <code>/log on</code> and <code>/log off</code>. Combat logs will then be located under your EverQuest installation folder, in the <code>\Logs</code> directory.</p>
  <img src="/log-parser/launch1.png" alt="Launch 1" class="wiki-image" />
  <img src="/log-parser/launch2.png" alt="Launch 2" class="wiki-image" />
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
    <p>The damage meter overlay is an in-game meter designed to provide a quick, mid-fight reference for your current combat target. The overlay is automatically hidden after combat ends, so it does not clutter your screen outside of active encounters.</p>
    <ul>
      <li><b>Important:</b> The overlay requires real combat data in your logs to function. If there is no recent combat activity, the overlay may briefly flash and then disappear.</li>
      <li>To use the overlay, open the <b>View</b> menu and hover over <b>Damage Meter</b>.</li>
      <li>Ensure the overlay is <b>enabled</b> to display it during combat.</li>
      <li>Use <b>Reset Position</b> to move the overlay to a default location if it is off-screen or misplaced.</li>
      <li>Choose <b>Set Up</b> to customize the overlay's colors, size, and appearance to your preference.</li>
    </ul>
    <p>The overlay is intended as a real-time tool for monitoring your performance during fights, not as a persistent display. For detailed breakdowns and analysis, refer to the main parser window after combat.</p>
      <img src="/log-parser/dmomenu.png" alt="Launch 1" class="wiki-image" />
    <img src="/log-parser/dmo.png" alt="Launch 1" class="wiki-image" />
  </div>
  <hr class="section-divider" />
  <div class="content-section">
    <h2>Labeled Log Breaks</h2>
    <p>You can add labeled breaks to your log list by typing <code>/say log_break label</code> in your log file. This feature lets you insert custom context into the logs, making it easier to track different parsing activities, such as when testers are running through various combinations of abilities and skills. It can also be used to break up an active fight into segments for more granular analysis. These labeled breaks will appear in the parser, helping you organize and review your log data more effectively.</p>
    <img src="/log-parser/custombreak.png" alt="Labeled Log Break Example" class="wiki-image" />
        <p><b>Tip:</b> This feature is especially useful if you want to exclude 'pull time' from a boss parse, such as when it takes extra time to get the boss into position before the real fight begins. By inserting a labeled break at the start of actual combat, you can ensure your parse reflects only the relevant portion of the encounter.</p>
  </div>
  <hr class="section-divider" />
  <div class="content-section">
   <h2>GINA Style Triggers</h2>
    <p>The integrated GINA Style Triggers system allows you to create, manage, and test custom triggers for in-game events directly within the parser. Triggers can be set up to watch for specific log messages, keywords, or patterns, and can respond with alerts, notifications, or automated actions. The trigger editor provides an intuitive interface for adding new triggers, editing existing ones, and testing their behavior in real time. This system is fully integrated and designed to help you stay on top of important events, warnings, or opportunities as you play—without the need for external tools.</p>
    <div class="section-description">
      <b>How to Use Triggers:</b>
      <ul>
        <li>Select <b>View &rarr; Triggers &rarr; Triggers Manager</b> to open the trigger management window.</li>
        <li>Right-click inside the triggers panel, choose <b>New</b>, and select <b>Trigger</b> to create a new trigger.</li>
        <li>You can also create folders to organize your triggers for better management.</li>
        <li>Right-clicking a trigger gives you options such as renaming, deleting, and setting overlays for that trigger.</li>
        <li>Once your trigger is created, you can assign it to the appropriate overlay or folder.</li>
        <li>For best results, copy the relevant line from your log and paste it into the <b>Matched Pattern</b> field to ensure accurate matching.</li>
        <li>Use <b>View &rarr; Triggers &rarr; Trigger Log</b> to test and verify that your triggers will match the intended log lines.</li>
        <li>The <b>Text to Display</b> option determines what message will be shown on screen when the trigger activates.</li>
        <li>You can use the <b>Trigger Tester</b> to test all your triggers at once. Simply copy your log file into the tester to see which triggers will match and how they will behave.</li>
        <li>You can also create <b>timer triggers</b> that activate when a timer ends, allowing for even more advanced alerting and automation.</li>
      </ul>
      <p>There are <b>so many options</b> for customizing your triggers and alerts—explore the interface to discover all the ways you can tailor notifications to your needs!</p>
      <b>Note:</b> For triggers to display notifications on your screen:
      <ul>
        <li>"Timer" triggers require a Timer overlay with "Default Overlay" enabled.</li>
        <li>"Text" triggers require a Text overlay with "Default Overlay" enabled.</li>
      </ul>
      <p>By default, the parser creates one Timer overlay and one Text overlay for you, so trigger notifications will work out of the box. If you remove these overlays or change their settings, you may need to re-enable or recreate them to see trigger alerts.</p>
            <img src="/log-parser/gina1.png" alt="Launch 1" class="wiki-image" />
    <img src="/log-parser/gina2.png" alt="Launch 1" class="wiki-image" />
                  <img src="/log-parser/gina3.png" alt="Launch 1" class="wiki-image" />
    <img src="/log-parser/tester.png" alt="Launch 1" class="wiki-image" />
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
            <li>Additional Search Options for Logs: Enhanced search and filtering features have been added to the log viewer, improving the ability to find and review specific log entries, combat events, triggers, and labeled breaks.</li>
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
        <b>Quality of Life Improvements</b>
    <ul>
      <li>General Quality of Life (QoL) Improvements: Various usability enhancements throughout the parser, including more intuitive navigation, better overlay defaults, and streamlined workflows.</li>
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
