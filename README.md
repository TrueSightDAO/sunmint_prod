# sunmint_prod

Sunmint Farmer App — simplified email-link + tree-planting report, TrueSight DAO.

Deployed at **sunmint.truesight.me** via GitHub Pages.

This repo is a GitHub **fork** of `sunmint_beta` (the working base — all changes land
there first). Promote beta → prod via:

```bash
gh repo sync TrueSightDAO/sunmint_prod --source TrueSightDAO/sunmint_beta
```

**⚠️ This repo's `CNAME` (`sunmint.truesight.me`) is deliberately diverged from
beta's (`beta.sunmint.truesight.me`) as of this commit.** `gh repo sync` only
fast-forwards commits and never touches a file beta doesn't also change — so as
long as **beta's `CNAME` is never edited again**, this file stays untouched by
future syncs. If beta's CNAME is ever edited, that change *will* flow into this
repo on the next sync and silently break the live domain — this is exactly what
happened to `truesight_me_prod` on 2025-11-30 (its CNAME got overwritten with
`beta.truesight.me` during a promotion, breaking truesight.me for months
undetected, fixed 2026-08-09). Don't repeat it here.
