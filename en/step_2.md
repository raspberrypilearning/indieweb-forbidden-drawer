<h2 class="c-project-heading--task">Build the warning tab</h2>

### Step 1

Add the clickable shell for the artefact, then make the outside of it feel much louder.

`<details>` makes a built-in open-and-close widget with no JavaScript. `<summary>` is the part people click on the front.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 9
line_highlights: 14-16
---
    <main class="page">
      <p class="eyebrow">Recovered profile artefact // last updated 2:13am</p>
      <h1>DO NOT OPEN_final_FINAL2.html</h1>
      <p class="status">mood: banned from the computer room</p>

      <details class="drawer">
        <summary>open this if you want to get cooked</summary>
      </details>
    </main>
--- /code ---

</div>

### Step 2

Go to `style.css` and replace the simple outside drawer rules with these ones.

This rule styles the **closed** widget. It controls the spacing, the bright surface colour, and the heavy shadow before the collapse is opened.

Replace the simple `.drawer` rule with this crazier version, or choose your own options.


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

### Step 3

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

### Step 4

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


## Now run your code

The page should now have a chunky warning tab that you can click open and closed, even though the inside is still missing.

<div class="c-project-output">
  <img src="images/step_2_output.png" alt="Expected project output after step 2 showing a loud clickable warning tab underneath the profile header.">
</div>
