# Put the Brain online — one-time setup (~5 min)

Everything you need is in the `GitHub_Upload` folder. I can't create accounts or handle passwords/tokens for you, so these clicks are yours — but it's short.

## 1. Create the repo
1. Go to **github.com** and sign in (or sign up, it's free).
2. Click **+ → New repository**. Name: `resell-brain`. Visibility: **Public** (required for free hosting — note: your pricing rules will be readable by anyone with the link, though nobody will have it). Check **"Add a README"**. Click **Create repository**.

## 2. Upload the files
1. In the repo, click **Add file → Upload files**.
2. Drag the **contents** of the `GitHub_Upload` folder in (index.html, README.md, and the whole `Brain` folder — dragging the Brain folder itself preserves it).
3. Click **Commit changes**.

## 3. Turn on the website
1. Repo **Settings → Pages** (left sidebar).
2. Under "Branch": pick **main**, folder **/ (root)**, click **Save**.
3. After ~1 minute your brain is live at:
   `https://YOUR-USERNAME.github.io/resell-brain/`
   Bookmark it — works on your phone too.

## 4. Make it editable (token)
1. GitHub: click your avatar → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. Name: `resell-brain-edit`. Expiration: 1 year. Repository access: **Only select repositories → resell-brain**. Permissions: **Contents → Read and write**. Generate, then copy the token.
3. Open your brain URL, enter your username + `resell-brain` + paste the token → **Connect**. The token stays in that browser only (repeat on your phone if you want to edit from there).

## 5. Tell Claude
Come back and tell me your GitHub username (or paste the brain URL — NOT the token). I'll point the scheduled tasks at the GitHub Brain and clean up the local copies.
