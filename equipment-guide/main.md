---
title: Equipment Guide
description: 
published: true
date: 2025-03-02T03:15:34.669Z
tags: 
editor: markdown
dateCreated: 2025-02-28T15:23:41.110Z
---

# Equipment Guide
[Epics](/equipment-guide/epics/_indexen) | [Proc Weapons](/equipment-guide/procs/_indexen) | [Sympathetic Items](/equipment-guide/symp-items) | [Tribute](/equipment-guide/tribute)

---

<style>
  /* Ensure the iframe container takes up full width */
  .iframe-container {
    width: 100%;
    height: 90vh; /* Increase height to take up 90% of the viewport */
    display: flex;
    justify-content: center; /* Centers iframe if needed */
    align-items: center;
  }

  /* Make the iframe take up full width and most of the height */
  .responsive-iframe {
    width: 95%; /* Slight padding to prevent edge clipping */
    height: 90vh; /* Use 90% of the viewport height */
    max-width: 100%;
    border: none;
  }
</style>

<div class="iframe-container">
  <iframe 
    id="dynamicIframe" 
    src="https://www.thjdi.cc/items" 
    class="responsive-iframe" 
    onload="adjustIframe()">
  </iframe>
</div>

<script>
  function adjustIframe() {
    var iframe = document.getElementById("dynamicIframe");

    // Attempt to adjust height based on content dynamically
    try {
      var newHeight = iframe.contentWindow.document.body.scrollHeight;
      if (newHeight > window.innerHeight * 0.9) {
        iframe.style.height = newHeight + "px"; // Make sure it expands enough
      } else {
        iframe.style.height = "90vh"; // Default to large size if content is smaller
      }
    } catch (error) {
      // If blocked by CORS, default to a large height
      iframe.style.height = "90vh";
    }

    // Ensure form inside iframe scales properly
    var iframeDoc = iframe.contentDocument || iframe.contentWindow.document;
    if (iframeDoc) {
      var forms = iframeDoc.getElementsByTagName("form");
      for (var i = 0; i < forms.length; i++) {
        forms[i].style.width = "100%"; // Expands form to match iframe width
      }
    }
  }

  // Resize on window resize for better responsiveness
  window.addEventListener("resize", adjustIframe);
</script>


---

