# Handover: Family Recipes, Erik FM, GymKompis

Three apps share this public repo and its GitHub Pages site (https://vikingkompis.github.io/family-recipes/). Read this first in any new session; rewrite it at the end.

_Last updated: 8 Nov 2026_

## Family Recipes (`/`)
- **What it is:** the family recipe book as an installable phone app (PWA). Moose chef mascot in a Swedish apron.
- **Data:** `recipes.json`, 185 recipes: 85 family cookbook, 77 Charlé Visser, 16 Mom's cookbook (Kook en Geniet), 7 made with Claude. Fields: title, category, ingredients, steps, tips, proTips, serves, time, art/artSvg, source.
- **Rules:** metric only. Every recipe has family tips and a professional finish. Mom's recipes keep her own names, otherwise "Mom's …". Charlé's recipes are rewritten in our own words with attribution, in their own "Charlé's kitchen" tab, not mixed into our categories. No link-outs: full recipes only.
- **Navigation:** category tiles open their own page (no endless scroll).
- **Parked idea:** a "kitchen with the kids" add-on.

## Erik FM (`/radio`)
- **What it is:** personal radio + live TV app for Mac and phone. Home screen: Radio or TV.
- **Radio:** SA (Jacaranda, KFM, 702), UK (BBC Radio 1/2/3, BBC Berkshire, Classic FM, Magic), Sveriges Radio, The Breeze NZ (Ronan Keating).
- **TV:** category tiles first, then channels. World news (direct streams, no YouTube), UK, Sweden incl. Nyheter på lätt svenska, SA (SABC News, WildEarth), food, films & series, sport. Uses hls.js; channels that are off air are hidden.
- **Rules:** nothing horse-related, no music TV channels. Erik wants to be able to add stations himself.
- **Latest:** 7 Nov removed Whiplash Cinema (programming suspended).

## GymKompis (`/gym`, unlisted)
- **What it is:** gym/exercise session builder for Erik's accountability group. Not a fitness tracker.
- **Modules:** home gym, gym, kettlebells, calisthenics, skipping, plus "just build me a session" (still asks how long and how hard). Equipment picked at onboarding. Calorie estimate from age, fitness 1–10, weight. Timer with beeps for timed work. "How to" opens a YouTube search. Up to ~10 saved sessions, share to WhatsApp.
- **No logins:** profile and equipment stay on each phone. Keep API cost near zero.
- **Look:** professional, not toy-like. No Viking mascot (reads as men-only). Logo: "Heart & iron" (kettlebell in a heart) or "Beat bar". Small varied icons with a dash of gold.
- **Open:** Erik asked for a 60–70 s promo video (high-energy music, male voice-over); check whether it was made.

## How to deploy
Push to `main`; GitHub Pages serves it within a minute or two. Each app has its own `sw.js`: bump its cache version on every change, or phones keep the old version.

## Next steps
1. Erik FM: re-check TV streams monthly; drop dead ones.
2. GymKompis: confirm the promo video status; calisthenics depth.
3. Recipes: add new recipes as Erik drops them in chat.
