# autonomous-test-files

Files that Applitools Autonomous tests open by URL (served by GitHub Pages). Not for distribution.

- `estate-snapshot-report-<id>.pdf`: the Estate Snapshot Report, unprotected (PDF test).
- `estate-snapshot-report-protected-<id>.pdf`: the same report, AES-256 encrypted with an open password.
  The password is kept outside this repo.
- `viewer.html?file=<pdf>`: a small PDF.js viewer that asks for a PDF's password, so an Autonomous
  web test can type it (as a masked secret) and check every page. It says
  "This PDF is password protected" / "This PDF is not password protected" on load,
  "Incorrect password" on a wrong one, and "Page N of M" once a page is drawn.
