<h2 class="c-project-heading--task">Make the inside look cursed</h2>

Turn the inside panel and the hidden message into the ugliest part of the artefact.

<h2 class="c-project-heading--explainer">Make this change</h2>

Stay in `style.css` and add louder inside rules underneath the simple starter ones. This is where the opened panel stops looking tidy and starts looking like a truly bad internet discovery.

<div class="c-project-tip">

<h3>Tip</h3>

<p>`border-radius` can make the inside box feel more sticker-like or more sharp-edged.</p>

<p>`text-shadow`, `font-size`, and `transform` can make the hidden message feel more ridiculous without changing the words.</p>

<p>`--inside-bg` can be pale peach, dirty white, washed-out cyan, or any other suspicious colour you chose in step 3.</p>

</div>

These new rules go underneath the simple starter versions in `style.css`. Because they come later in the file, they take over and give the inside panel its final cursed look.

### Step 1

Underneath the starter rules, add a new `.inside` rule like this.

This rule styles the inside panel that appears after opening. It adds the striped background, thicker border, and more space around the hidden message.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 119
line_highlights: 119-135
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

### Step 2

Underneath your new `.inside` rule, add a new `.inside p` rule like this.

This rule only styles the hidden paragraph itself. It turns `6-7` into huge ugly text that is impossible to miss.

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 137
line_highlights: 137-147
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

The inside panel should now feel much messier, and the hidden message should look huge and ugly when you open the drawer.

<div class="c-project-output">
  <img src="images/step_5_output.png" alt="Expected project output after step 5 showing the final cursed-profile artefact with a giant ugly hidden message.">
</div>
