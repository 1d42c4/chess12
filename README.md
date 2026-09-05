# Calculate with Purpose

**[Open the live GitHub Pages course](https://knightway8.github.io/chess12/)**

Short, reliable lines before long, impressive ones. Generate useful candidates, calculate the opponent’s resistance, and recognize the tactical mechanisms behind a combination.

## Who it is for

Players who know legal moves and want a disciplined way to find and verify tactics.

This is an extensive course through a defined practical skill area, not a claim to cover all of chess. The full four-course route is aimed at human learners building reliable habits from the basics toward club play.

## What is included

- 24 distinct lessons in four modules, each with an explanation, task, answer, common mistake, and recall prompt.
- 120 interactive exercises with saved answer data.
- A six-week study plan and links to the full 24-week route.
- Browser-local progress, a review queue, private study notes, and progress import/export.
- A printable workbook with an answer key, Markdown notes, PGN positions, and structured JSON exercises.
- Offline scripts and styles; no account, analytics, remote fonts, or runtime engine service required.

## Modules

1. Build a calculation process
2. Recognize tactical mechanisms
3. Force the position to change
4. Verify and transfer

## Start here

[Lesson directory](https://knightway8.github.io/chess12/) · [Practice lab](https://knightway8.github.io/chess12/practice.html) · [Study plan](https://knightway8.github.io/chess12/study-plan.html) · [Downloads](https://knightway8.github.io/chess12/downloads.html) · [Sources and verification](https://knightway8.github.io/chess12/sources.html)

## The four-course collection

| Repository | Course | Live site |
| --- | --- | --- |
| [chess11](https://github.com/knightway8/chess11) | See the Board | [Open](https://knightway8.github.io/chess11/) |
| [chess12](https://github.com/knightway8/chess12) | Calculate with Purpose | [Open](https://knightway8.github.io/chess12/) |
| [chess13](https://github.com/knightway8/chess13) | Make a Plan | [Open](https://knightway8.github.io/chess13/) |
| [chess14](https://github.com/knightway8/chess14) | Finish the Game | [Open](https://knightway8.github.io/chess14/) |

## Use offline

Choose **Code → Download ZIP**, extract the archive, and open `index.html` in a browser. External reference and analysis links require internet access. Progress is browser-local; export it before clearing storage or changing devices.

## Verification

The 120 tactical exercises came from original simulated legal games. Stockfish 19 analyzed each selected position with MultiPV 3 and a 200,000-node search. The selected first move had a substantial score gap in that recorded search. This is finite engine analysis, not an exhaustive proof of uniqueness; another legal move may still be playable. The stored principal variation is one continuation, not a claim that every reply is forced.

See [VALIDATION.json](VALIDATION.json) for check results. The original prose is AI-created educational material; report a concrete correction with its lesson or exercise ID. No rating improvement is promised.

## Maintain and publish

The editable source is [data/course.json](data/course.json). Run `node tools/build.mjs` to regenerate the pages, then `node tools/validate.cjs` for content, answer-legality, PGN, and link checks. The browser data and downloadable files are regenerated from the same source.

GitHub Pages serves the root of `main` with `.nojekyll`. Active branch rules require pull requests, prevent force pushes, and prevent deleting the default branch, with no bypass actors. Repository owners can still change settings or delete the repository.

## Credits

Original course writing, interface, and generated practice positions were prepared with AI for knightway8. The bundled chess.js library is BSD-2-Clause licensed; its full notice is in [vendor/chess-LICENSE.txt](vendor/chess-LICENSE.txt). Stockfish was used for local analysis and is not redistributed here. Tablebase facts are credited to the Lichess Syzygy service.
