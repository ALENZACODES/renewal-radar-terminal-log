# Renewal Radar, Shipped from the Terminal

![Cover](cover.png)

A log of taking my Renewal Radar site from GitHub to my own machine and back, using only typed commands.

Live site: https://renewal-radar-site.vercel.app
Site code: https://github.com/ALENZACODES/renewal-radar-site
The commit I pushed: https://github.com/ALENZACODES/renewal-radar-site/commit/71bed1b

![The commit](images/commit-71bed1b.png)

## What I did
1. Checked my tools: Node 24.22.1, Git 2.47.3, pnpm 12.16.1
2. Cloned the repo with `gh repo clone`, installed with `pnpm install`, ran it with `pnpm dev` and got HTTP 200 on localhost:3000
3. Made one real change: a "Skip to main content" link for keyboard users and a "How it works" link in the header
4. Ran `pnpm build` to make sure the production build still passes
5. Committed under my own name and pushed to main
6. Installed the Vercel CLI to make a preview deployment

![The site running locally with the skip link showing](images/local-site-skip-link.png)

## Files
| File | What it is |
| --- | --- |
| COMMANDS.md | Every command, in order, with what it does |
| transcripts/01-clone-install-run.txt | Raw output: tools, clone, install, local run |
| transcripts/02-change-build-commit-push.txt | Raw output: diff, build, commit, push |
| transcripts/03-vercel-cli.txt | Raw output: Vercel CLI install and login check |

Built by John Khan, ALENZA CODES, Toronto, Ontario.
