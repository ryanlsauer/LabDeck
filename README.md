# LabDeck

A free, private study app for Medical Laboratory Science (MLS) students, built around the Sentara RMH School of Medical Laboratory Science curriculum. It runs entirely in your browser on a laptop or phone, works offline, and has no accounts, ads or server.

LabDeck combines the study methods with the strongest evidence behind them (active recall, spaced repetition, interleaving, elaboration and error correction) with lessons, games and tools written for MLS coursework.

---

## What's inside

### Learn
- **Head start lessons.** About 94 guided lessons across 11 units, from "science from zero" through every course: lab orientation and safety, phlebotomy, immunology, microbiology, hematology and hemostasis, chemistry, blood bank, and urinalysis. Bootcamp lessons start with a quick warm-up from earlier lessons and a no-penalty guess at what's coming, teach in small steps (read, recall the missing terms, check understanding), and finish with a recap of the key ideas you can save as fill-in-the-blank cards. Each unit ends with a review.
- **Learn mode.** A gentle first pass through any deck: see each card, pick the answer from four, then recall it yourself. Missed cards come back twice until they stick, and learned cards move into spaced review.
- **Memory hooks.** Silly sentences and memory palaces for lists and sequences (order of draw, coagulation factors, MUDPILES and more). Each hook is also a review card in the deck you link it to. Starter hooks are included and can be edited, deleted or restored.
- **Explain it.** Write an explanation in your own words. It's graded idea by idea against a model answer and checks for common MLS misconceptions.
- **Glossary.** Every abbreviation the app uses, spelled out. Tap any dotted-underlined term anywhere to see its meaning. Add your own.
- **Formula sheet.** Every lab-math formula with what each variable means and a worked example.
- **Listen.** Hands-free review: it reads each question, pauses for you to answer out loud, then reads the answer.

### Practice and test
- **Study (spaced repetition).** Rate each card Again, Hard, Good or Easy:
  - **Again:** back after 3 cards, then needs two good answers this session. Due again tomorrow.
  - **Hard:** comes back once more about 8 cards later. Small step forward.
  - **Good:** done for today. Normal spacing.
  - **Easy:** done for today. Big step forward. Easy three times in a row means mastered.
- **Deck modes.** Multiple choice, type it, select all that apply, unknown ID, picture ID, match and sequence.
- **Mixed practice, look-alike drills, range drills and lab math** with fresh numbers every time, so you learn the method instead of memorizing an answer.
- **Board practice and a comprehensive exam,** weighted by course credit hours or by the ASCP BOC content areas.
- **Case studies and case presentations,** including a builder for the chemistry case-study assignment.
- **Mistake journal.** A question lands here only if you miss it twice (or miss it on an exam). End each day with a short mistake review; get each one right twice and it's cleared.

### Play
Fourteen leveled games with points, lives and high scores, all in one games hub (your recent games also show on the home screen and sidebar). Levels climb from recognizing to reasoning. Each game unlocks when you pass the lesson that teaches it:
- **Tube trainer:** drag tubes into the order of draw, then pick tubes for real orders.
- **Smear practice:** find, name and count cells, from normal cells to a mini differential.
- **Urine sediment:** casts, crystals and cells.
- **Gram stain:** read stains, judge specimen quality, and beat the clock.
- **Antibody panel:** identify antibodies and do rule-outs.
- **Acid-base:** read blood gases, from pH to compensation.
- **Westgard judge:** accept or reject QC runs, tell random from systematic error, prove a rejection by tapping the points that break the rule, and choose the right next step.
- **Critical call:** learn critical limits, then report, call or recollect.
- **Bench unknown:** identify organisms with the fewest tests.
- **ID flowcharts:** Gram stain first, then walk the charts to an identification.
- **Coag detective:** read PT/PTT patterns, interpret mixing studies, and solve bleeding and clotting cases.
- **Anemia workup:** size the anemia, read iron studies, and diagnose from indices, retic count and smear findings.
- **ABO & Rh typing:** type from forward and reverse reactions, pick compatible red cells and plasma, and solve typing discrepancies.
- **UA detective:** what each dipstick pad really detects, when the dipstick and microscope disagree, and whole-picture urinalysis cases.

### Plan
- **Today's targets:** a short, realistic list each day that ends with your mistake review.
- **Dashboard:** due cards, daily goal, streak, the week at a glance, next exam, mastery and lessons.
- **My program:** all 10 courses and 1,110 objectives from the curriculum guide, a readiness meter per course, objective ratings, an exam map for each course, and rotation prep.
- **Exams:** add exam dates for countdowns, focused prep and last-minute cramming.
- **Course map, study timer, study plan, starter packs** (35 ready-made decks) and **slide photos** (turn your own microscope photos into picture practice).
- **Badges:** about 130 achievements for long-term habits, mastery, games and milestones.

### Make it yours
- Create decks with term and definition cards, profile cards (for example, an organism with fields like Gram stain, catalase and oxidase), fill-in-the-blank cards and image cards.
- Every card can hold a note and a "why."
- Import from a pasted list or a spreadsheet.
- Group decks with color-coded labels, star cards, and add a new card in the middle of any study session.

---

## Keyboard
Press **Enter** to move to the next screen whenever a Next or Continue button is showing, and **1–4** to pick an answer. In study, **Space** flips the card.

## Where your data lives
- **On each device,** in the browser's storage for this website (IndexedDB, plus a second copy in localStorage).
- **Optionally, in a private GitHub gist** if you turn on sync in Settings. Sync keeps your phone and laptop in step. Changes merge both ways, and for settings like game unlocks, the most recent choice wins.
- Your data is never stored in the app's files, so updating the app never touches your progress.

## Setting up sync
1. On GitHub, go to Settings > Developer settings > Personal access tokens > Tokens (classic).
2. Create a token with only the **gist** box checked. Set the expiration to "No expiration" or a long date.
3. In LabDeck, open Settings > Sync between devices, paste the token, and tap Connect.
4. Repeat step 3 on each device you use.

The token stays in your browser. It can only read and write your gists.

## Installing on a phone
- **iPhone (Safari):** open the site, tap Share, then Add to Home Screen.
- **Android (Chrome):** open the menu, then Install app or Add to Home screen.

LabDeck then opens full screen like an app and works offline.

## Updating the app
1. In your GitHub repository, click **Add file > Upload files**.
2. Drop in the new `index.html` and `sw.js` (and any other changed files), then click **Commit changes**.
3. Wait about a minute for GitHub Pages to finish (the Actions tab shows a green check).
4. Close and reopen LabDeck. The version number in Settings confirms the update.

On iPhone, if the home-screen icon changes in an update, remove the shortcut and add it again.

## Backups
**Settings > Download backup** saves everything (decks, images, review history, progress) to one file. Use **Restore or import** to load it on any device. Spreadsheet exports of your study log, lesson scores and deck stats are also available there.

## Files
| File | Purpose |
|---|---|
| `index.html` | The entire app: interface, content and logic |
| `sw.js` | Service worker that makes the app work offline |
| `manifest.webmanifest` | Lets phones install LabDeck as an app |
| `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` | App icons |
| `README.md` | This file |

## A note on content
LabDeck's lessons and starter decks follow standard MLS textbook values and the program's curriculum guide. Reference ranges, critical values and procedures vary by laboratory. When your instructors' materials or your lab's policies differ, theirs are the ones to follow.
