# b or d Mouth Check

A single-file web app for small groups of students who mix up b and d.

## How a session works

1. The adult enters each student's name, picks the number of turns per student (default 5), and picks the turn order.
2. A large **b** or **d** card appears with an arrow underneath showing the reading direction (left to right).
3. After a moment, two prompts appear for the adult to read aloud:
   - Straight line or open?
   - Sound?
4. The adult taps **Correct** or **Not yet**. One mark covers both prompts for that turn.
5. After every student finishes their turns, a results table shows correct out of turns, percent, and separate b and d counts for each student.

Each student gets an equal number of b and d cards (one extra of a random letter when the turn count is odd), shuffled so the same letter never appears three times in a row for one student.

Keyboard shortcuts: **C** correct, **N** not yet, **U** undo the last mark.

## Run it

Open `index.html` in any modern browser. No install, no login, no internet needed.

## Put it on GitHub Pages

1. Create a repo and add `index.html` and this README.
2. In the repo, go to Settings, then Pages.
3. Under Source, choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. The app will be at `https://<your-username>.github.io/<repo-name>/`.

## Privacy

Student names and results are held in the page's memory only. Nothing is saved to the browser and nothing is sent anywhere. Use **Copy results** (a text summary) or **Copy for spreadsheet** (tab-separated columns that paste into Google Sheets or Excel) before closing the page.

## Customizing

- Prompt wording is in the `<ol>` inside the `#prompts` block of `index.html`.
- The app uses the Teachers font (SIL Open Font License 1.1), embedded inside `index.html` so the app is one file. The card letter font is the `--letter-font` variable in the CSS, and the rest of the text uses the `font-family` on `body`.
