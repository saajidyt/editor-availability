# YT4B Editor Availability

Daily standup tracker: who is Free / Busy / On leave, for the full day, 1st half or 2nd half.

- **Site:** this repo, served by GitHub Pages at https://editoravailability.ytforbrands.com (branch `main`, root).
- **Data + sign-in:** a Google Apps Script web app (Code.gs, kept out of this repo) writing to the "YT4B Editor Availability" Google Sheet. Its URL goes in `config.js`.
- **Access:** set in Code.gs (`ALLOWED`), not in this repo.

## Day-to-day
- Add / remove people and switch Pod lead / Editor under "Manage people" on the site, or edit the People tab in the sheet.
- Change the password: in Apps Script run `setPassword("new password")` once (signs everyone out).
- After editing Code.gs: Deploy → Manage deployments → Edit → Version: New version → Deploy (keeps the same URL).
