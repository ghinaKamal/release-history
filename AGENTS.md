# Go Helen release history

## User instructions

These instructions record the user's requests for this directory. Apply them to future work on the release history unless the user changes them.

- Read the release history document and provide a Markdown table showing when each release was ready for distribution when requested.
- Maintain an HTML version of that table in `release-history.html`.
- Include a column linking to release notes HTML pages in this directory. Not every release has release notes; missing notes are acceptable.
- Name that links column **In-app release notes**.
- Include another column named **Development release notes**. Leave its cells blank until the user supplies content or requests otherwise.
- Right-align the **Time** column, including its header and values.
- Use a monospaced font for the version numbers in the **Release** column.
- Keep this `AGENTS.md` file as context for future questions and edits in this workspace.

## Current implementation and source conventions

The following details describe the existing implementation, rather than additional explicit user requirements. Preserve them when making focused edits unless the task calls for a change.

- Source documents: `team-helen-versions.md` for Team Helen, `build-helen-versions.md` for Build Helen, `gohelenversionhistory.txt` for Go Helen, `helen_at_home_distribution_history.md` for Helen at Home, `helen_linen_distribution_history.md` for Helen Linen, `# Helen Podcast — iOS Distribution Histo.md` for Helen Podcast, `# Lead Helen — iOS Distribution History.md` for Lead Helen, `# One Helen — iOS Distribution History.md` for One Helen, `# One Nurse — iOS Distribution History.md` for One Nurse, and `ask_helen_distribution_history.md` for Ask Helen.
- HTML output: `release-history.html`, a standalone page with inline CSS, responsive horizontal table scrolling, and print styling.
- Columns, in order: **Release**, **Ready date**, **Time**, **Recorded status**, **In-app release notes**, **Development release notes**.
- List releases newest first and preserve version strings, including leading zeroes and parenthesized build numbers.
- Use the first **Ready for Distribution** event for a release, or the first **Ready for Sale** event for older releases. Do not substitute review, pending release, or replaced dates.
- Retain the source's date and time values. The user has confirmed that the recorded times are Beirut time; explain this in the page introduction without adding “Beirut” to the Time column header.
- Version **1.0.15** first reached **Ready for Sale** on **Apr 7, 2023 at 8:40 PM**, and returned to that status on **Jul 5, 2023 at 12:17 PM** after **Pending Agreement**. Preserve the explanatory note.
- Match in-app release notes by version and build number, ignoring whitespace in filenames; display a dash when no exact match exists.
- For Go Helen only, check release notes at `https://bennettranville.blob.core.windows.net/go-helen/release-notes/en-US/`, followed by the version/build with whitespace removed and `.html` (for example, `2.4.209(3).html`). If that URL is unavailable, try the same filename under `https://bennettranville.blob.core.windows.net/go-helen/release-notes/`. Show an unavailable marker if both URLs fail; do not derive Go Helen links from local documents.
- For example, `2.3.036(1).html` is for build 1 and is not currently linked to the history row for **2.3.036 (2)**.
- Do not add release rows solely because a notes file exists: distribution dates come from the source document.
- At the time this file was created, the table had 41 releases and 13 in-app notes links. These counts describe current data, not permanent limits.
- After edits, check that each row has the expected columns and that local release notes links resolve to existing files.

## Multi-app release history

- Keep one main `release-history.html` page; do not create separate release-history pages for each app.
- Keep the app selector alphabetized: **Ask Helen**, **Ask Helen Kids**, **Build Helen**, **Go Helen**, **Helen Assistant**, **Helen at Home**, **Helen Exec**, **Helen Linen**, **Helen Podcast**, **Lead Helen**, **One Helen**, **One Nurse**, and **Team Helen**. Do not add other apps until the user requests them.
- Mark **Ask Helen Kids**, **Helen Exec**, and **Helen Assistant** as **Not Live** in the selector and selected-app view. Keep their release histories empty until authoritative data is supplied.
- Keep each app's metadata, releases, source, and notices separate so selecting an app displays only that app's history.
- Preserve all existing Go Helen releases and release-notes links.
- Team Helen has 28 releases sourced from `team-helen-versions.md`. Use the earliest ready event for version 1.0.3 and preserve the note about its later return after Pending Agreement.
- Team Helen's source supplies eight remote detailed release-notes URLs; retain those exact links, and show unavailable markers for releases without a supplied link.
- Build Helen has two releases sourced from `build-helen-versions.md`; retain its source values and leave notes cells blank or unavailable until matching notes are supplied.
- Helen at Home has nine releases sourced from `helen_at_home_distribution_history.md`; retain its source values and leave notes cells blank or unavailable until matching notes are supplied.
- Helen Linen has three releases sourced from `helen_linen_distribution_history.md`; retain its source values and leave notes cells blank or unavailable until matching notes are supplied.
- Helen Podcast has two releases sourced from `# Helen Podcast — iOS Distribution Histo.md`; sort them newest to oldest and leave notes cells blank or unavailable until matching notes are supplied.
- Lead Helen has four releases sourced from `# Lead Helen — iOS Distribution History.md`; preserve its three supplied detailed release-notes links and show an unavailable marker for the release explicitly lacking notes.
- One Helen has 15 releases sourced from `# One Helen — iOS Distribution History.md`; sort them newest to oldest and leave notes cells blank or unavailable until matching notes are supplied.
- One Nurse has three releases sourced from `# One Nurse — iOS Distribution History.md`; sort them newest to oldest and leave notes cells blank or unavailable until matching notes are supplied.
- Ask Helen has eight releases sourced from `ask_helen_distribution_history.md`; retain its source values and leave notes cells blank or unavailable until matching notes are supplied.
- Keep releases sorted newest to oldest within each app.
- Make the selected app clear in both the selector and page heading.
- Structure future additions as data entries without duplicating the table or creating more main HTML pages.
- Open detailed release-notes links in a new browser tab so the selected app and table state remain in place.
- Open source-file links in a new browser tab so the selected app and table state remain in place.
