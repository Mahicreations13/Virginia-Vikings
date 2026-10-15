# Virginia Vikings — Free Cricket Team Website

A responsive, professional static website for Virginia Vikings, designed for free hosting on **GitHub Pages**.

## What's included
- Virginia Vikings, USCL T20, Wesley Elite Sports, and ProCorp Systems branding
- Leadership profiles and clickable social icons (no visible profile URLs)
- Empty coach-photo frame as requested
- 20 editable player slots
- Media room for match highlights, posters/flyers, and team moments
- Match journal starter posts
- Mobile-friendly layout

## Preview locally
Open `index.html` in a browser. For best results, use VS Code's Live Server extension.

## Publish for free on GitHub Pages
1. Extract the ZIP.
2. Open your GitHub repository.
3. Upload **the contents** of this folder (not the enclosing folder) to the repository root. Make sure `index.html`, `styles.css`, `script.js`, and `assets/` are at the root.
4. Commit the changes to the `main` branch.
5. Open **Settings → Pages**.
6. Under Build and deployment, select **Deploy from a branch**.
7. Choose branch `main` and folder `/(root)`, then click **Save**.
8. Wait a few minutes and refresh the Pages screen to find the published site URL.

## Add selected players
1. Add each player's image into `assets/`, e.g. `player-01.jpg`.
2. Open `script.js`.
3. In the `players` array, update each slot's `name`, `role`, and `image`.
   Example:
   `{ number: "01", name: "Player Name", role: "BATTER", image: "assets/player-01.jpg" }`
4. Save and upload the updated files to GitHub.

## Add a coach photo
Put the selected coach photo in `assets/` and edit the coach card in `index.html`. The frame is intentionally empty right now.

## Add match posters and blogs
- Add poster/flyer images to `assets/`.
- Add a new item to the `journalPosts` array in `script.js` for each match report or announcement.
- To display a poster in a post, extend the post data and the journal-card markup in `script.js`, or replace one of the media visuals in `index.html` with an image tag.
- Commit and push the changes to GitHub; GitHub Pages will publish the update.

## Add YouTube highlights
Add YouTube video IDs to `highlightVideoIds` in `script.js`. To show them on the public page, embed them using an iframe in the media section of `index.html`. YouTube ID is the part after `v=` in a YouTube video URL. (The included media room is ready for customization.)

## Important: static website limitations
GitHub Pages is free and does not include a private admin panel or database. Files uploaded through a public website form would not automatically persist for all visitors. To update public content, replace/add assets and edit `script.js` or `index.html`, then commit the changes to GitHub. Avoid uploading private or sensitive information.
