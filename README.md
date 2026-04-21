# Stack Fighters — Support & Privacy Website

A small static website that serves as Stack Fighters' official support + privacy policy destination. Ready to drop onto GitHub Pages (or any static host) in 5 minutes.

## What's in here

```
stackfighters-site/
├── index.html       Landing page with hero, features, roster, block legend
├── support.html     FAQ, contact info
├── privacy.html     Privacy policy (required for App Store submission)
├── style.css        Shared stylesheet (dark stone / gold aesthetic)
├── assets/          Art assets lifted from the game
│   ├── icon.png
│   ├── title_logo.png
│   ├── hero_bg.png
│   ├── phraya.png / akiko.png / ragnar.png / citlali.png / alaric.png / zoya.png
│   └── block_strike.png / block_vitality.png / block_spirit.png / block_tactics.png
└── README.md        This file
```

## Deploying to GitHub Pages

Takes about 5 minutes.

### 1. Create the repo

```bash
cd stackfighters-site
git init
git add .
git commit -m "Initial site"
git branch -M main
```

Then on GitHub:
1. Create a new public repo named e.g. `stackfighters-site`
2. Copy the remote URL

```bash
git remote add origin git@github.com:YOUR-USERNAME/stackfighters-site.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Repo → **Settings** → **Pages** (left sidebar)
2. **Source:** Deploy from a branch
3. **Branch:** `main`, folder `/ (root)`
4. Save

Within a minute or two, your site will be live at:

```
https://YOUR-USERNAME.github.io/stackfighters-site/
```

### 3. Use the URLs in App Store Connect

- **Support URL:** `https://YOUR-USERNAME.github.io/stackfighters-site/support.html`
- **Privacy Policy URL:** `https://YOUR-USERNAME.github.io/stackfighters-site/privacy.html`
- (Optional) **Marketing URL:** `https://YOUR-USERNAME.github.io/stackfighters-site/`

Paste those into App Store Connect → App Information.

## Custom domain (optional)

If you own `stackfighters.com` (or similar):

1. Settings → Pages → **Custom domain** → enter the domain, save
2. In your DNS provider, add a CNAME record pointing your domain to `YOUR-USERNAME.github.io`
3. Wait 5–60 minutes for DNS + HTTPS cert provisioning
4. Tick "Enforce HTTPS"

Your URLs become `https://stackfighters.com/support.html` etc. — nicer in the App Store listing.

## Editing the site

Everything is plain HTML + CSS — no build step, no framework. Open any `.html` file locally in a browser to preview. Push to `main` to deploy.

Tweaks you'll commonly want:

- **Update the contact email:** replace `pond1982a@gmail.com` in all three HTML files (3 places each)
- **Add an App Store badge** to `index.html` once the app is live — replace the `.hero__cta-note` block with an official Apple "Download on the App Store" SVG + link
- **New FAQ entry:** copy-paste any existing `<details>` block in `support.html` and edit
- **Effective date:** bump the date at the top of `privacy.html` when you make material changes

## Mobile preview

The site is mobile-first — most of your App Store visitors will land here via a phone tap on the Support/Privacy link. Resize your browser below 640px width to see the responsive layout kick in (nav compacts, roster stacks to 2 columns, etc.).

## License

The website code is yours. The art assets are from the Stack Fighters game and shouldn't be redistributed separately — keep them within this site.
