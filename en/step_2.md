<h2 class="c-project-heading--task">Add the drawer HTML</h2>

Add the drawer underneath the header so the page has something dramatic to open.

<h2 class="c-project-heading--explainer">Make this change</h2>

Add a `<details class="drawer">` element with a clickable `<summary>` and a hidden `<section class="inside">`.

`<details>` makes a built-in open-and-close widget with no JavaScript. The `<summary>` is the part people click, and everything else inside stays hidden until it opens.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 9
line_highlights: 14-19
---
    <main class="page">
      <p class="eyebrow">Recovered profile artefact // last updated 2:13am</p>
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

## Now run your code

Open the drawer and you should see the new warning on the tab and `6-7` inside.

<div class="c-project-output">
  <img src="images/step_2_output.png" alt="Expected project output after step 2 showing the new drawer warning and hidden message.">
</div>
