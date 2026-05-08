<h2 class="c-project-heading--task">Add the cursed message</h2>

Add the final message inside the hidden panel so the drawer reveals something when it opens.

<h2 class="c-project-heading--explainer">Make this change</h2>

Put the hidden message inside the `<section class="inside">`.

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
          <p>6-7</p>
        </section>
      </details>
    </main>
--- /code ---

</div>

<div class="c-project-tip">

<h3>Tip</h3>

<p>The hidden message already has its final styling in `style.css`, so the text will look loud as soon as you add it.</p>

</div>

## Now run your code

The drawer should now reveal the secret message when you open it.

<div class="c-project-output">
  <img src="images/step_4_output.png" alt="Expected project output after step 4 showing the final cursed profile artefact with its hidden message revealed.">
</div>
