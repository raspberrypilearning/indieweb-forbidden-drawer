<h2 class="c-project-heading--task">Label the forbidden drawer</h2>

You will change the page title, the main heading, and the clickable warning on the drawer.

Open `index.html` and look inside the `<details>` element. The `<summary>` line is the part people click, and everything after it stays hidden until the drawer opens. Change the text so the page already feels like your own bad idea.

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 1
line_highlights: 6,13,16
---
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Forbidden Drawer</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <!-- This one drawer opens and closes using only HTML. -->
    <main class="page">
      <p class="eyebrow">Homemade Web Toy</p>
      <h1>Do Not Open This Drawer</h1>

      <details class="drawer">
        <!-- <summary> is the clickable warning on the drawer. -->
        <summary>Click here if you enjoy bad decisions</summary>
        <section class="inside">
          <p>Inside is one object you should definitely replace with your own weird idea.</p>
        </section>
      </details>
    </main>
  </body>
</html>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

You should see your new heading on the page, and the warning text should appear on the drawer tab.

<div class="c-project-output">
  <img src="images/step_1_output.png" alt="Observed project output after this step.">
</div>
