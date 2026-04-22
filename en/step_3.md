<h2 class="c-project-heading--task">Change the page colours</h2>

You will change a few CSS values so the drawer gets its own rotten mood.

Open `style.css` and edit the custom properties at the top. These small values control the page background, the drawer colours, the border size, and the font.

<div class="c-project-tip">

<h3>Tip</h3>

<p>Try colours that feel sticky, mouldy, suspicious, or just plain wrong.</p>

<p>Swap the font if you want the page to feel cleaner, louder, or more handwritten.</p>

</div>

<div class="c-project-code">

--- code ---
---
language: css
filename: style.css
line_numbers: true
line_number_start: 1
line_highlights: 2-12
---
/* Change these values to make the drawer feel more cursed. */
:root {
  --page-bg: #efe3c2;
  --ink: #23101b;
  --panel-bg: #fff7ec;
  --drawer-bg: #c8f06b;
  --drawer-open-bg: #ffd976;
  --inside-bg: #fff9ef;
  --border-size: 4px;
  --corner-size: 22px;
  --body-font: "Trebuchet MS", Verdana, sans-serif;
  --drawer-width: 32rem;
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

The page should still work, but the colours and font should now feel more suspicious.

<div class="c-project-output">
  <img src="images/step_3_output.png" alt="Observed project output after this step.">
</div>
