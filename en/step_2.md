<h2 class="c-project-heading--task">Build the warning tab</h2>

Add one clickable drawer so the file can open and close without any JavaScript.

<h2 class="c-project-heading--explainer">Make this change</h2>

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
      <p class="eyebrow">THIS PAGE FAILED THE VIBE CHECK<br>// OPEN AT YOUR OWN RISK</p>
      <h1>DO NOT OPEN_final_FINAL2.html</h1>
      <p class="status">mood: banned from the computer room</p>

      <details class="drawer">
        <summary>open this if you want to get cooked</summary>
      </details>
    </main>
--- /code ---

</div>

## Now run your code

The page should now have a chunky warning tab that you can click open and closed, even though the inside is still missing.

<div class="c-project-output">
  <img src="images/step_2_output.png" alt="Expected project output after step 2 showing a loud clickable warning tab underneath the profile header.">
</div>
