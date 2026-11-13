# Every command I ran, in order

Site: https://renewal-radar-site.vercel.app
Code: https://github.com/ALENZACODES/renewal-radar-site

## Find my way around and check the tools
```bash
pwd
node -v          # v24.22.1
git --version    # 2.47.3
pnpm -v          # 12.16.1
```

## Bring the site home and run it
```bash
gh repo clone ALENZACODES/renewal-radar-site
cd renewal-radar-site
ls
pnpm install
pnpm dev         # then open http://localhost:3000
curl -s -o /dev/null -w 'HTTP %{http_code}\n' http://localhost:3000   # HTTP 200
```

## Make one real change
Added a "Skip to main content" link that appears when a keyboard user presses Tab, gave the main region an id so the link has somewhere to land, and added a "How it works" link to the header so every section is one click away.

```bash
git status --short
git diff
pnpm build       # production build passes, both routes static
```

## Send it back to GitHub under my own name
```bash
git config user.name "John Khan"
git config user.email 309250657+ALENZACODES@users.noreply.github.com
git add app/page.tsx components/site-header.tsx
git commit -m "Add skip to content link and How it works nav link"
git push origin main
git log -3 --format='%h %an %s'
```
Result: commit 71bed1b on main, https://github.com/ALENZACODES/renewal-radar-site/commit/71bed1b

## Talk to Vercel from the terminal
```bash
npm i -g vercel
vercel --version   # 65.15.0
vercel login
vercel link
vercel list
vercel             # preview deployment
vercel --prod      # put the new commit on the public site
```

Full output of each step is in transcripts/.
