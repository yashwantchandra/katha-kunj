# कथा कुंज — Free Hosting Guide

Your entire site is a **single `index.html` file** — no build, no server, no database. Pick any of these free hosts:

---

## Option 1 — Netlify Drop (easiest, ~30 seconds)

1. Go to **https://app.netlify.com/drop**
2. Drag the whole `hindi-stories-site` folder onto the page.
3. You instantly get a live URL like `https://dreamy-kathakunj-a1b2.netlify.app`.
4. (Optional) Sign up free to claim the site and rename the URL.

No account required for the instant deploy. Free forever for static sites.

---

## Option 2 — GitHub Pages (free custom-ish URL)

1. Create a new repo on GitHub, e.g. `katha-kunj`.
2. Upload `index.html` to the repo (drag-and-drop in the browser works).
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**, Branch: `main`, Folder: `/ (root)`.
5. Save. Your site goes live at `https://<your-username>.github.io/katha-kunj/` in ~1 minute.

---

## Option 3 — Vercel (also 30 seconds)

1. Go to **https://vercel.com** and sign in with GitHub/email.
2. Click **Add New → Project → Import** (or drag-drop in the CLI).
3. Select the folder. Vercel auto-detects a static site. Click **Deploy**.
4. Live at `https://katha-kunj.vercel.app`.

---

## Option 4 — Cloudflare Pages

1. Sign up at **https://pages.cloudflare.com**.
2. Click **Create → Upload assets**.
3. Drag the folder. Deploy.
4. Live at `https://katha-kunj.pages.dev`.

---

## Local preview

Just double-click `index.html` — it opens in any browser. That's it.

---

## Adding / editing stories

Open `index.html`, find the `const stories = [...]` array near the bottom, and add a new object:

```js
{
  cover: 'cover-1',          // cover-1 through cover-5 available
  category: 'लघुकथा · विषय',
  title: 'आपकी कहानी का शीर्षक',
  subtitle: 'एक पंक्ति का परिचय',
  excerpt: 'तीन-चार पंक्ति का झरोखा...',
  content: `
    <p>पहला अनुच्छेद...</p>
    <p>दूसरा अनुच्छेद... <em>ज़ोर देने वाले शब्द</em> ...</p>
  `
}
```

Save → re-upload. Done.
