# Valearion website

Static multi-page site. No build step. Deploy the files in this folder as-is.

## Push to GitHub
```
cd valearion
git init
git add .
git commit -m "Valearion website v6"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/valearion.git
git push -u origin main
```

## Deploy on Vercel
Dashboard: vercel.com > Add New > Project > Import your GitHub repo.
Framework Preset: Other. Build command: none. Output directory: leave empty (root).
Deploy, then add your domain (valearion.com) under Project Settings > Domains.

CLI alternative:
```
npm i -g vercel
vercel
vercel --prod
```

## Notes
- Canonical URLs are set to https://valearion.com/ across all pages, robots.txt, sitemap.xml, and llms.txt. Change them if the live domain differs.
- robots.txt, sitemap.xml, and llms.txt must stay at the domain root, next to index.html.
- Drop a logo.png at the root to satisfy the Organization schema logo reference.
