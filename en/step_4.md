<h2 class="c-project-heading--task">Make the drawer look wrong</h2>

You will tweak the drawer border, spacing, and hidden panel so opening it feels more dramatic.

Stay in `style.css` and update the drawer rules. Small changes to padding, borders, and shadows can make the closed drawer feel chunky and the open drawer feel even stranger.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`padding` changes how thick and stuffed the drawer feels.</p>

<p>`border` and `box-shadow` change how heavy the drawer looks.</p>

<p>The `.inside` box can feel neat, sticky, rotten, or chaotic depending on its background and border.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 52
line_highlights: 53-78
---

.drawer {
  margin-top: 24px;
  padding: 18px;
  border: var(--border-size) solid var(--ink);
  border-radius: var(--corner-size);
  background: var(--drawer-bg);
  box-shadow: 0 10px 0 #23101b;
}

.drawer[open] {
  background: var(--drawer-open-bg);
}

summary {
  cursor: pointer;
  font-size: 1.1rem;
  font-weight: 900;
  letter-spacing: 0.01em;
}

.inside {
  margin-top: 16px;
  padding: 14px 16px;
  border: 3px dashed var(--ink);
  border-radius: calc(var(--corner-size) - 6px);
  background: var(--inside-bg);
  line-height: 1.6;
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

The drawer should now feel chunkier, and the hidden message box should look clearly separate when you open it.

<div class="c-project-output">
  <img src="images/step_4_output.png" alt="Observed project output after this step.">
</div>
