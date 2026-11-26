---
layout: page
title: about
permalink: /about/
---


## contact

<p id="contactLinks">email: <a href="#" onclick="showEmail(); return false;">click to show</a></p>
<script>
  function showEmail() {
    var contactLinks = document.getElementById("contactLinks");
    var encodedEmail = 'ZHVib2lzIC4gbGlvIGF0IHBtIC4gbWU=';
    var decodedEmail = atob(encodedEmail);

    contactLinks.innerHTML = '<br> email: ' + decodedEmail;
  }
</script>

- elsewhere: [sit amet](#)