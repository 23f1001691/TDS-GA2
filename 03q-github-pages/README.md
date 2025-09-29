## GitHub Pages Deployment

1. **Create a new repository** on [GitHub](https://github.com).

   - Keep it **public** if you want free GitHub Pages hosting.

2. Change your mail id in `index.html`

3. **Upload your files** - `index.html`

   - You can do this manually via GitHub’s web UI → **Add file → Upload files**.
   - Or push from your local machine using `git`.

4. **Go to Repository Settings** → **Pages** (left sidebar, under "Code and automation").

5. Under **Source**, select:

   - **Branch:** `main` (or `master`).
   - **Folder:** `/ (root)` if your `index.html` is at the top level.

6. Click **Save**.

7. Wait 1–2 minutes, then reload the **Pages section**.

   - You’ll see your hosted link in the format:

     ```
     https://<username>.github.io/<repository-name>/
     ```

