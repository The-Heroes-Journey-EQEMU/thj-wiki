---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:49:12.398Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide

[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

 Breakpoint Iframe Demo /\* Hide by default so that on load, if we're in the in-between size, it's hidden \*/ .iframe-container { display: none; /\* hidden initially \*/ width: 100%; height: 80vh; /\* a tall, responsive container (80% of viewport height) \*/ position: relative; overflow: hidden; } /\* Make the iframe fill the entire container \*/ .responsive-iframe { width: 100%; height: 100%; border: none; }

/\*\* \* Show or hide the iframe container based on window width. \* - Show if < 768px \* - Show if > 1400px \* - Hide otherwise \*/ function checkScreenSize() { const container = document.getElementById("iframeContainer"); const screenWidth = window.innerWidth; if (screenWidth < 768 || screenWidth > 1400) { container.style.display = "block"; } else { container.style.display = "none"; } } /\*\* \* Attempts to scale content inside the iframe if allowed (same-origin). \* If cross-origin with strict security, this may be blocked. \*/ function fixIframeScaling() { try { const iframe = document.getElementById("scaledIframe"); const iframeDoc = iframe.contentDocument || iframe.contentWindow.document; const iframeBody = iframeDoc.body; // Example: scale down to 90% and adjust width to compensate iframeBody.style.transform = "scale(0.9)"; iframeBody.style.transformOrigin = "top left"; iframeBody.style.width = "111%"; } catch (error) { console.log("Cross-origin restriction prevents styling inside the iframe."); } } // Run on page load checkScreenSize(); // Also check on window resize window.addEventListener("resize", checkScreenSize);