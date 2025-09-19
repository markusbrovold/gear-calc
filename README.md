# Last War Gear Calculator

Simple single-page calculator for summing upgrade costs in Last War. Everything is self-contained in `index.html`, so you can host it anywhere that serves static files (GitHub Pages, Netlify, etc.).

## Features
- Level picker that covers gear levels 0-40 and star segments.
- Instant feedback of total coin, ore, and ceramic costs.
- Detailed step-by-step breakdown for each upgrade level/segment.
- No build step, no dependencies, and no external requests.

## Local Preview
1. Clone or download this repository.
2. Open `index.html` directly in your browser **or** run a lightweight server, e.g.:
   ```sh
   python -m http.server
   ```
   Then browse to `http://localhost:8000`.

## GitHub Pages Hosting
1. Create a new repository on GitHub and push this project (make sure `index.html` is in the repository root).
2. In the GitHub repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick the default branch (for example `main`) and the `/ (root)` folder.
4. Click **Save**. GitHub will build and publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Customising Data or Text
- All upgrade data lives in the `gearData` constant inside `index.html`. Update the JSON there if the game changes.
- The UI copy (headings, messages, etc.) lives in the same file near the top.

## Project Structure
- `index.html` – HTML, CSS, JavaScript, and data for the calculator.
- `gear_progression.json` – Original data source (kept for reference; not used by the app anymore).

Feel free to remove `gear_progression.json` or adapt the layout if you only need the deployed calculator.
