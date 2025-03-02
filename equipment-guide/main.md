---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:45:03.607Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide
[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

<html>
<head>
  <meta charset="UTF-8"/>
  <title>Fixed-Width Iframe Container</title>
  <style>
    /* 
      Container is fixed at 1400px wide, 
      so screens smaller than 1400px will have a horizontal scrollbar 
      on the main page (not the iframe).
    */
    #iframeContainer {
      width: 1400px;       /* fixed width, won't shrink below 1400px */
      height: 800px;       /* pick any fixed height you want */
      margin: 0 auto;      /* optional: center on larger screens */
      overflow: hidden;    /* hide scrollbars on the *container* itself */
      border: 1px solid #ccc; /* optional border so you can see the container clearly */
    }

    /*
      The iframe will always match the container's width (1400px)
      and fill its entire height (800px).
      Use 'overflow: auto;' or 'scrolling="yes"' to allow internal scrollbars
      for content that doesn't fit vertically.
    */
    #fixedWidthIframe {
      width: 1400px;    /* match container width */
      height: 100%;     /* fill container’s height */
      border: none;     /* remove default iframe border */
      overflow: auto;   /* show scrollbars if content is bigger than 1400x800 */
    }
  </style>
</head>
<body>

<div id="iframeContainer">
  <iframe
    id="fixedWidthIframe"
    src="https://www.thjdi.cc/items"
    scrolling="yes"
  ></iframe>
</div>

</body>
</html>



