# ISPSC Model Congress | House of Representatives

Website of the ISPSC Model Congress, the legislative simulation of the Bachelor of Public Administration (BPA) program, College of Business, Management, and Entrepreneurship, Ilocos Sur Polytechnic State College.

## What is in this repository

| Path | What it is |
|---|---|
| `index.html` | The website: Home (About), Org Chart, Committees, Hon. Members, District Map, Legislation, Documents, Print, Admin |
| `console/index.html` | Session Console for the plenary session (presenter controls + projector window, timers) |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

Everything is self-contained: photos, logos, the map, and the data are built into each HTML file. No server, database, or build step is needed.

## Publish with GitHub Pages

1. Create a new repository on GitHub (for example `ispsc-model-congress`). Set it to **Public** (GitHub Pages on a free account needs a public repository).
2. Click **Add file > Upload files**, drag in `index.html`, the `console` folder, and `.nojekyll`, then click **Commit changes**.
3. Go to **Settings > Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, **Branch** to `main` and folder `/ (root)`, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/ispsc-model-congress/`.
   The Session Console is at `https://<your-username>.github.io/ispsc-model-congress/console/`.

## Updating the website

The site has no server, so edits made in the Admin tab are first saved only in the browser where they were made. To publish them:

1. Open the live site, go to **Admin**, sign in, and make the edits (members, photos, House Bills, documents, About text).
2. Go to **Admin > Publish and Backup** and click **Download updated website**.
3. Rename the downloaded file to `index.html`.
4. In the repository, click **Add file > Upload files**, upload the new `index.html` (it replaces the old one), and **Commit changes**.
5. The live site updates in about a minute. Press Ctrl + F5 if the old version still shows.

## Notes

- **Admin password.** Change the default password in **Admin > Site and Password** before the first upload. The password only keeps casual visitors out of the editing screens: the site is a public static file, so do not store confidential information in it.
- **Attached documents.** Files attached in the Documents tab are packed inside `index.html` when you download the updated website. GitHub's web uploader accepts files up to 25 MB, so keep attachments small (PDF, ideally under 5 MB each). Put large files on Google Drive (sharing: "Anyone with the link") and paste the link instead.
- **Privacy.** The site shows students' names and photos. Make sure the Members have agreed to this before publishing. The page includes a `noindex` tag so search engines do not list it; remove the line `<meta name="robots" content="noindex, nofollow">` from `index.html` if you want it to appear in search results.
- **National Anthem in the Session Console.** Do not upload the anthem video to this public repository. On session day, use the console's file picker to load the MP4 from the presenting computer.
- **Academic simulation.** Titles, districts, and party-list affiliations are role assignments for the simulation. This is not an official website of the House of Representatives of the Philippines.
