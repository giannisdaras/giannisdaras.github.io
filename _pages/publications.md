---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

<p class="scholar-note">
  For the most updated list of my publications, check my
  <a href="https://scholar.google.com/citations?user=LaScvbQAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
  page.
</p>

{% include bib_search.liquid %}

<div class="pub-filters" role="group" aria-label="Filter publications">
  <button type="button" class="pub-filter is-active" data-filter="all" aria-pressed="true">All</button>
  <button type="button" class="pub-filter" data-filter="award" aria-pressed="false">Awards, orals &amp; spotlights</button>
  <span class="pub-filter-count" aria-live="polite"></span>
</div>

<div class="publications">

{% bibliography %}

</div>

<script>
  (function () {
    // The theme's own text search hides entries with an .unloaded class and
    // clears that class on every keystroke, so this filter marks its own
    // entries with data-pub-filtered instead. The two then compose: an entry
    // is visible only when neither has hidden it.
    var root = document.querySelector(".publications");
    if (!root) return;
    var buttons = document.querySelectorAll(".pub-filter");
    var count = document.querySelector(".pub-filter-count");
    var mode = "all";

    function apply() {
      var shown = 0,
        total = 0;
      root.querySelectorAll("ol.bibliography").forEach(function (list) {
        var kept = 0;
        list.querySelectorAll(":scope > li").forEach(function (li) {
          total++;
          // An award, oral or spotlight is the only thing rendering a .award button.
          var keep = mode === "all" || li.querySelector(".links a.award") !== null;
          li.toggleAttribute("data-pub-filtered", !keep);
          if (keep) {
            kept++;
            shown++;
          }
        });
        list.toggleAttribute("data-pub-filtered", kept === 0);
        var heading = list.previousElementSibling;
        if (heading && heading.tagName === "H2") heading.toggleAttribute("data-pub-filtered", kept === 0);
      });
      count.textContent = mode === "all" ? "" : shown + " of " + total;
    }

    buttons.forEach(function (btn) {
      btn.addEventListener("click", function () {
        mode = btn.dataset.filter;
        buttons.forEach(function (b) {
          var on = b === btn;
          b.classList.toggle("is-active", on);
          b.setAttribute("aria-pressed", on ? "true" : "false");
        });
        apply();
      });
    });

    // Re-assert after the text search rewrites visibility.
    var search = document.getElementById("bibsearch");
    if (search) search.addEventListener("input", function () { setTimeout(apply, 350); });
  })();
</script>
