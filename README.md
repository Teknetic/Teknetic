## Rawle Felix

  I reverse-engineer and automate things other
  developers give up on —
  binary analysis, browser internals, fingerprinting
  and anti-bot behaviour,
  and scraping targets that actively resist
  automation.

  ### Recent work

  A claims audit of a commercial anti-detect
  browser. I diffed its 295 MB
  patched `chrome.dll` against a version-matched
  stock Chromium reference and
  tested every marketing claim empirically, then
  wrote the results up as a
  verdict ledger:

  **26 confirmed true · 13 traced to the exact
  upstream source · 2 partial · 1 provably false**

  The finding that mattered: its canvas, WebGL and
  audio fingerprint noise are
  each a pure deterministic function of one launch
  seed, and the default seed
  space is only 90,000 values — so every
  "randomised" fingerprint it produces
  can be precomputed and reverse-looked-up.

  I then automated the whole investigation into a
  14-stage pipeline, so the
  same audit runs against any browser build from one
  command.

  → [**browserdiff**](https://github.com/Teknetic/browserdiff) — the pipeline, open    source

  ### Available for

  Browser-security audits · anti-bot and detection
  diagnosis · reverse
  engineering · scraping that survives · verifying a
  vendor's claims before
  you buy.

  ### Contact

  **asterncer@gmail.com**
