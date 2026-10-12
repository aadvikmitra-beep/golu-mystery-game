# Navaratri Golu Mystery Game

A static website for GitHub Pages. It uses the 40 catalogue entries, picks five random unique questions per round, reveals optional hints and answers, displays the answer picture, and offers review/replay at the end.

## Test it on your computer
Because the game loads `questions.json` using `fetch`, open it through a local web server rather than double-clicking `index.html`.
1. Install Python if needed.
2. Open Command Prompt in this folder.
3. Run: `python -m http.server 8000`
4. Open `http://localhost:8000` in your browser.

## Publish with GitHub Pages
1. Sign in to GitHub and create a new repository, for example `golu-mystery-game`.
2. Upload **all contents** of this folder (the `index.html`, `questions.json`, `images` folder, and this README) to the repository's root.
3. Open the repository's **Settings → Pages**.
4. Under build/deployment, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/(root)`, then Save.
6. Wait for GitHub Pages to publish the site. The URL will be shown in Settings → Pages.
7. Open the published URL on your phone and test all five questions and image display.
8. Create a QR code that points to the published URL, then print it for your Golu display.

## Updating questions or pictures
- Edit `questions.json` to change a title, description, hint, answer, or image path.
- Replace an image in `images/` with the same filename to update a photo.
- Item 23 (Horse Carriage) is currently a placeholder because the uploaded document appears to reuse the Bullock Cart photo for that item. Replace `images/23.svg` with the correct image file and update item 23's `image` value in `questions.json` to `images/23.jpg` (or the filename you use).
- After editing, upload/commit the changed files to GitHub. GitHub Pages will redeploy automatically.

## Notes
- The game does not save progress or scores.
- A new round picks five unique items at random; questions can reappear in later rounds.
- Keep the names and folder paths exactly as written, including uppercase/lowercase.
