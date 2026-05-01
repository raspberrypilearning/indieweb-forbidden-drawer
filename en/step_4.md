<h2 class="c-project-heading--task">Make it look badly famous</h2>

Make the outside of the artefact chunkier and more dramatic so opening it feels a bit chaotic.

<h2 class="c-project-heading--explainer">Make this change</h2>

Stay in `style.css` and update the outside drawer rules. Padding, borders, shadows, and text styling can make the closed widget feel heavy before you even open it.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`padding` changes how stuffed and chunky the widget feels.</p>

<p>`border`, `box-shadow`, and `background` make it look stickered, loud, and messy on purpose.</p>

</div>

These rules restyle the outside of the widget: the closed drawer, the open state, and the clickable summary.

### Step 1

Replace the simple `.drawer` rule with this chunkier version.

This rule styles the closed widget itself. It controls the spacing, the bright surface colour, and the heavy shadow before the drawer is opened.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 83
line_highlights: 83-95
---
.drawer {
  margin-top: 24px;
  padding: 18px 18px 16px;
  border: var(--border-size) solid var(--ink);
  border-radius: var(--corner-size);
  background:
    linear-gradient(135deg, rgba(255, 255, 255, 0.28), transparent 45%),
    var(--drawer-bg);
  box-shadow:
    0 12px 0 var(--shadow-color),
    0 18px 28px rgba(0, 0, 0, 0.38);
  transition: transform 180ms ease, background-color 180ms ease;
}
--- /code ---

</div>

Run your code and observe how the closed drawer looks chunkier, brighter, and heavier even before you open it.

### Step 2

Replace the short `.drawer[open]` rule with this version.

This rule only applies after the drawer opens. It changes the background and adds a slight tilt so the open state feels more dramatic.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 97
line_highlights: 97-102
---
.drawer[open] {
  background:
    linear-gradient(135deg, rgba(255, 255, 255, 0.32), transparent 45%),
    var(--drawer-open-bg);
  transform: rotate(-0.7deg) translateY(3px);
}
--- /code ---

</div>

Run your code and observe that opening the drawer now changes its colour and gives it a small wonky shift.

### Step 3

Replace the `summary` rule with this one.

This rule styles the clickable label on the front. It makes the warning text bigger, bolder, and easier to notice.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 104
line_highlights: 104-109
---
summary {
  cursor: pointer;
  font-size: 1.1rem;
  font-weight: 900;
  letter-spacing: 0.02em;
}
--- /code ---

</div>

Run your code and observe that the summary text on the closed drawer looks louder and more important.

## Now run your code

The closed drawer and the warning label should now feel much louder, while the inside panel still looks fairly plain for now.

<div class="c-project-output">
  <img src="images/step_4_output.png" alt="Expected project output after step 4 showing the louder drawer styling before the inside panel gets its final ugly makeover.">
</div>
