<h2 class="c-project-heading--task">Add the hidden panel</h2>

Add the inside box that appears when the artefact opens.

<h2 class="c-project-heading--explainer">Make this change</h2>

Put the hidden `<section>` inside the drawer. The CSS for `.inside` is already in `style.css`, so the panel will appear as soon as you add the HTML.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 9
line_highlights: 16-17
---
    <main class="page">
      <p class="eyebrow">THIS PAGE FAILED THE VIBE CHECK<br>// OPEN AT YOUR OWN RISK</p>
      <h1>DO NOT OPEN_final_FINAL2.html</h1>
      <p class="status">mood: banned from the computer room</p>

      <details class="drawer">
        <summary>open this if you want to get cooked</summary>
        <section class="inside">
        </section>
      </details>
    </main>
--- /code ---

</div>

<div class="c-project-tip">

<h3>Tip</h3>

<p>The `inside` class already has its final styling in `style.css`, so you do not need to write any new CSS in this step.</p>

</div>

## Now run your code

The drawer should now open to an empty hidden panel instead of showing nothing inside.

<div class="c-project-output">
  <img src="images/step_3_output.png" alt="Expected project output after step 3 showing the drawer open with an empty hidden panel inside it.">
</div>
