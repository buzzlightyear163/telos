# TELOS

Static site, one file: `index.html`. Deploy the folder as-is on Vercel (no build step).
three.js (r128) loads from cdnjs and its post-processing files from jsDelivr; fonts from Google Fonts.

## Set at launch
Open `index.html`, find `const TELOS = {` near the top of the script and fill in:
- `ca` – the $TELOS contract address (already set: 9TzvCF4fWu6yHPvDygRGJx5QgZVzYTcaZmMPdnGopump)
- `x` – your X profile URL
- `pumpfun` – the pump.fun coin URL (already set)
- `github` – program repo, if public
- `programLive` – set to `true` only once the on-chain program is deployed and wallet signing is wired up

Explore rows are example data (`const COINS = [...]`). Kit numbers in the scroll film are simulated and labelled as such.

## How the page works
- One fixed WebGL stage behind the page. The 3D O sits in the TEL◔S wordmark in the hero, then lifts out as you scroll.
- The same particles re-form for each step: route (80/15/5), Burn, Floor, Draw, Graduate, $TELOS.
- Quality drops automatically on slow devices; no WebGL falls back to the flat logo.

## Brand
`brand/` has the mark and wordmark as SVG (currentColor + light/dark) and the flat pfp in three colourways (2000×2000).
`brand/social/` has the ceramic set for X and pump.fun: avatar, banner, launch post and kits post.
