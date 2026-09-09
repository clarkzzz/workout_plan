# Foundations — Beginner Strength Plan

An interactive, single-page version of a beginner-friendly 3-day strength plan (dumbbell, kettlebell, flywheel, mat). Includes lightweight animated icons for each movement pattern and embedded YouTube demonstrations for every exercise.

## View it live

Once hosted on GitHub Pages, the site will be available at:
`https://<your-username>.github.io/<repo-name>/`

## How to publish this on GitHub Pages

1. Create a new repository on GitHub (e.g. `training-plan`).
2. Upload `index.html` (and this `README.md`) to the repository — either via the GitHub web UI ("Add file" → "Upload files") or via git:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Add training plan site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, choose branch `main` and folder `/ (root)`, then click **Save**.
5. Wait a minute or two — GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/`.

## Editing the plan

All exercise data lives in the `days` array near the bottom of `index.html` (inside the `<script>` tag). Each exercise has:
- `name`, `sets`, `note`, `cue` — the text shown in the card
- `icon` — one of `squat`, `hinge`, `row`, `press`, `lunge`, `halo`, `plank`, `twist`, `swing`
- `videoId` — the YouTube video ID for the embedded form demonstration
- `query` — the search term used for finding alternate YouTube tutorials and variations

Edit these values directly and re-upload to update the site — no build step required, it's a single static HTML file.
