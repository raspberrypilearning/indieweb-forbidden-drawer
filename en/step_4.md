<h2 class="c-project-heading--task">Make it look badly famous</h2>

Make the clickable artefact chunkier and more dramatic so opening it feels a bit chaotic.

<h2 class="c-project-heading--explainer">Make this change</h2>

Stay in `style.css` and update the drawer rules. Padding, borders, shadows, and text styling can make the closed widget feel heavy and the revealed message feel like a very bad internet discovery.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`padding` changes how stuffed and chunky the widget feels.</p>

<p>`border`, `box-shadow`, and `background` make it look stickered, loud, and messy on purpose.</p>

<p>You can also style `.inside p` so the hidden message looks huge, ugly, and impossible to ignore.</p>

</div>

These rules restyle each part of the widget: the closed drawer, the open state, the clickable summary, the inside panel, and the giant hidden message text.

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

### Step 4

Replace the `.inside` rule with this version.

This rule styles the inside panel that appears after opening. It adds the striped background, thicker border, and more space around the hidden message.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 111
line_highlights: 111-127
---
.inside {
  margin-top: 16px;
  padding: 14px 16px;
  border: 4px dashed var(--ink);
  border-radius: calc(var(--corner-size) - 4px);
  background:
    repeating-linear-gradient(
      -45deg,
      rgba(255, 255, 255, 0.4),
      rgba(255, 255, 255, 0.4) 8px,
      transparent 8px,
      transparent 16px
    ),
    var(--inside-bg);
  box-shadow: inset 0 0 0 2px rgba(255, 255, 255, 0.55);
  line-height: 1.7;
}
--- /code ---

</div>

Run your code and observe that the inside area now feels more like a messy warning panel than a plain box.

### Step 5

Replace the `.inside p` rule with this final version.

This rule only styles the hidden paragraph itself. It turns `6-7` into huge ugly text that is impossible to miss.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 129
line_highlights: 129-139
---
.inside p {
  margin: 0;
  font-family: "Comic Sans MS", Impact, fantasy;
  font-size: clamp(4rem, 18vw, 7rem);
  font-weight: 900;
  line-height: 0.82;
  letter-spacing: 0.08em;
  text-align: center;
  text-shadow: 4px 4px 0 var(--drawer-open-bg);
  transform: rotate(-2deg);
}
--- /code ---

</div>

Run your code and observe that the hidden message now looks huge, warped, and deeply embarrassing.

## Now run your code

The widget should now feel chunkier, louder, and more chaotic when you open it, and the hidden message should look huge and ugly.

<div class="c-project-output">
  <img src="images/step_4_output.png" alt="Expected project output after step 4 showing the final cursed-profile artefact with a giant ugly hidden message.">
</div>
