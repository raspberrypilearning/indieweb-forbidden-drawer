<h2 class="c-project-heading--task">Hide something suspicious inside</h2>

You will swap the placeholder reveal for your own mildly gross secret.

Stay in `index.html`. The content after `<summary>` sits inside `<details>`, so it appears when the drawer opens. Replace the paragraph with one funny, weird, or suspicious reveal of your own.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 11
line_highlights: 18
---
    <main class="page">
      <p class="eyebrow">Homemade Web Toy</p>
      <h1>Do Not Open This Drawer</h1>

      <details class="drawer">
        <summary>Click here if you enjoy bad decisions</summary>
        <section class="inside">
          <p>Inside is one suspicious banana, two wet biscuits, and a note that says "it hatched".</p>
        </section>
      </details>
    </main>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

Open the drawer and you should see your new hidden message inside.

<div class="c-project-output">
  <img src="images/step_2_output.png" alt="Observed project output after this step.">
</div>
