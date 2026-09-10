# AI Tools Comparison

Single-file site. Snapshot: 8 September 2026.

## Files

| File | Required? | What it is |
|---|---|---|
| `index.html` | **Yes — this is the site** | Full dashboard: Overview, Assistants (KPI, licensing, 9 vendors, CISO), Specialist tools, Cybersecurity |
| `ai-tools-comparison.html` | Optional duplicate | Same content as `index.html`. Only needed if you want both names |
| `ai-assistant-dashboard.html` | **No** | Older assistants-only file. Do not upload unless you want the pre-merge version |

Upload **`index.html` only**. GitHub Pages serves that name at the repo root URL.

---

## Publish with github.com only (no Git, no Terminal)

### A. Create the repository

1. Sign in at [https://github.com](https://github.com).
2. Click the **+** in the top right → **New repository**.
3. Repository name: `ai-tools-comparison` (any name works).
4. Set it to **Public** if you want a free `*.github.io` URL that anyone can open. Private Pages need GitHub Pro.
5. Check **Add a README file** (optional; you can also upload this README next).
6. Click **Create repository**.

### B. Upload the site file

1. On the new repo page click **Add file** → **Upload files**.
2. Drag in `index.html` from your computer (download it from the chat first).
3. Commit message: `Add AI Tools Comparison dashboard`.
4. Click **Commit changes**.

If you already added a README in step A, you now have two files: `README.md` and `index.html`. That is correct.

### C. Turn on GitHub Pages

1. In the repo click **Settings**.
2. Left sidebar → **Pages**.
3. Under **Build and deployment** → **Source**, choose **Deploy from a branch**.
4. Branch: **main** (or `master` if that is what GitHub created).
5. Folder: **/ (root)**.
6. Click **Save**.
7. Wait 30–90 seconds. Refresh the Pages settings page.
8. GitHub shows the live URL:

`https://YOUR-USERNAME.github.io/ai-tools-comparison/`

That URL is the site. Bookmark it. Send that link to share.

### D. Update the site later (weekly or whenever)

1. Open the repo on github.com.
2. Click `index.html`.
3. Click the pencil (**Edit**) icon.
4. Select all, delete, paste the new file contents  
   **or** delete the file (**…** menu → Delete file), commit, then **Add file → Upload files** with the new `index.html`.
5. Commit. Pages rebuilds in about a minute. Same URL.

### E. Custom domain (optional)

In **Settings → Pages → Custom domain**, enter a hostname you own (example: `ai.yourcompany.com`) and add a CNAME at your DNS host pointing to `YOUR-USERNAME.github.io`. GitHub will prompt for HTTPS.

---

## What people will see

- **Overview** — buy-path, default stack, do-not-double-pay
- **Assistants** — 9 models, KPI matrix, licensing, per-vendor tabs, CISO
- **Specialist tools** — writing, decks, video, design, meetings, research, automation
- **Cybersecurity** — EDR, NDR, SIEM, agentic SOC, AppSec, identity

Scores are synthesized reviews of 2026 product surfaces, not lab benchmarks.
