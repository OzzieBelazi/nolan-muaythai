# Nolan Muay Thai — SEO Audit (June 2026)

**Goal:** Rank top of Google for "Muay Thai Beckenham" and related local queries.
**Primary competitor:** [Scorpions Muay Thai Boxing Gym](https://scorpionsthaiboxing.com/) — 189–195 High Street, Beckenham BR3 1AH. Family-run, anchored by 9× world champion Stephen Wakeling, strong local citation footprint (Yell, Hotfrog, Mimoji, multiple directories).

---

## Diagnosis (one paragraph)

Your **on-page SEO is genuinely strong** — 9 schema.org blocks, geo tags, hreflang, Open Graph, manifest, FAQ markup. Technically near best-in-class for a small-business static site. The reasons you're not topping Beckenham searches are:

1. **One on-page miss that mattered a lot:** the H1 and `<title>` did not lead with "Beckenham". (Fixed in this branch.)
2. **No social proof on the site:** zero reviews, testimonials, or `AggregateRating` schema. Google's local algorithm heavily weights review signals.
3. **Off-page weakness vs Scorpions:** they are physically on Beckenham High Street, with more local directory listings and a longer-established Google Business Profile presence.

You will not out-rank Scorpions on proximity alone. You out-rank them with **reviews, citations, and content depth** — none of which are visible on the current site.

---

## What I fixed in this branch (`seo-tune-jun2026`)

| # | Change | File | Impact |
|---|--------|------|--------|
| 1 | H1 changed `"Master the Art of Muay Thai"` → `"Muay Thai Classes in Beckenham"`, subtitle moved into a supporting `<p>` mentioning WBC champion + BR3 | `index.html` | High — single biggest local ranking lever |
| 2 | Homepage `<title>` trimmed from 110 chars → 56 chars, leads with "Muay Thai Beckenham" | `index.html` | High — full title now visible in SERPs |
| 3 | Meta description rewritten — leads with "Muay Thai classes in Beckenham", mentions champion, address, price (CTR boost) | `index.html` | Medium — better click-through |
| 4 | Open Graph + Twitter Card titles & descriptions synced to new copy | `index.html` | Medium — social shares |
| 5 | Footer copyright `2025` → `2026` across all 9 HTML files | all pages | Low — freshness signal |

Net diff: 9 files, +17 / −17 lines. No layout / visual regression — only text and meta swaps.

---

## On-page audit (everything else)

### Already excellent (leave alone)
- ✅ `SportsActivityLocation` schema with full address, geo coords, opening hours, areaServed for 20+ neighbourhoods
- ✅ FAQ schema with 5 Q&A entries
- ✅ Recurring Event schema for kids classes (Sun + Wed)
- ✅ Course schema for 4 class types
- ✅ Person schema for Liam, linked to real [Wikipedia article](https://en.wikipedia.org/wiki/Liam_Nolan_(Muay_Thai))
- ✅ VideoObject schema for the intro reel
- ✅ Canonical URLs, hreflang en-gb, manifest, favicons
- ✅ Sitemap submitted, robots.txt clean
- ✅ Lazy-loaded images, preconnect to Google Fonts, preload hero
- ✅ GA4 installed

### Quick wins still on the table (need your input)
1. **Add `AggregateRating` + `Review` schema to homepage** — needs real star count + 3–5 short review quotes. I won't fabricate these. Pull from Google reviews verbatim.
2. **Add a visible "What our members say" section** — 3–5 testimonial cards on the homepage with name + neighborhood. Massive local trust signal.
3. **Add `LocalBusiness` `@type` alongside `SportsActivityLocation`** — multi-typed schema unlocks more SERP features. Trivial change.
4. **Add an FAQ on the homepage visually** — you have FAQ schema but no FAQ section users see. Mirror them into the page.
5. **Add internal links** from homepage paragraphs to `coaches.html`, `junior-muay-thai.html`, `sign-up.html` — currently navbar-only. Inline contextual links pass more weight.
6. **Add a "Why Nolan Muay Thai?" section** with bullet points name-dropping Beckenham, Bromley, BR3, Elmers End — keyword density in natural copy.
7. **Image filenames are descriptive ✅ but alt text could mention Beckenham more often** — e.g. `about-fighter.jpg` alt should say "Liam Nolan training Muay Thai in Beckenham gym".
8. **Trim other page titles** — `about.html`, `gallery.html`, `sign-up.html`, `contact.html` are all 80+ chars. Same surgical trim as homepage.

### Things that won't move the needle (don't bother)
- Meta keywords tag (Google ignores it, has since 2009)
- More schema blocks (you have enough)
- Reorganising the page structure
- Switching frameworks

---

## Off-page audit — THIS IS WHERE THE RANKING IS WON

You can fix everything on-page perfectly and still lose to Scorpions if these are weak.

### 1. Google Business Profile (highest priority)
- [ ] **Claim & verify** at https://business.google.com — is `Nolan Muay Thai` claimed?
- [ ] **Category:** primary = "Muay Thai gym" or "Martial arts school". Add secondary categories: "Gym", "Personal trainer", "Fitness centre".
- [ ] **Photos:** upload 20+ high-quality photos — exterior, interior, classes, kids classes, Liam with belts. Geo-tag the photos.
- [ ] **Posts:** publish weekly — class spotlights, fighter wins, schedule updates. Google rewards active profiles.
- [ ] **Q&A:** seed 5–10 likely customer questions yourself, answer them.
- [ ] **Services:** list each class type with price.
- [ ] **Reviews:** ask EVERY active member for a Google review. Target = beat Scorpions' count + average. This is the single biggest off-page lever.

### 2. NAP consistency (Name / Address / Phone)
The exact same NAP must appear on every directory listing. Discrepancies hurt rankings.
**Canonical NAP:**
```
Nolan Muay Thai
9-10 Goodwood Parade, Upper Elmers End Rd, Elmers End, Beckenham, BR3 3QZ
+44 7740 961476
```

### 3. Local citations — submit to all of these
- [ ] [Yell.com](https://www.yell.com)
- [ ] [Bing Places](https://www.bingplaces.com)
- [ ] [Apple Maps Connect](https://mapsconnect.apple.com)
- [ ] [Hotfrog](https://www.hotfrog.co.uk)
- [ ] [Cylex](https://www.cylex-uk.co.uk)
- [ ] [FreeIndex](https://www.freeindex.co.uk)
- [ ] [Thomson Local](https://www.thomsonlocal.com)
- [ ] [Scoot](https://www.scoot.co.uk)
- [ ] [The Sun Local](https://local.thesun.co.uk)
- [ ] [Yelp UK](https://www.yelp.co.uk)
- [ ] [Foursquare](https://foursquare.com)

### 4. Sport-specific directories
- [ ] [UKMF (UK Muay Thai Federation)](https://www.ukmf.com) club listing
- [ ] [Find a Gym (sportengland.org)](https://www.sportengland.org)
- [ ] [Wikidata entry for Nolan Muay Thai](https://www.wikidata.org) (linked to Liam's Wikipedia page)
- [ ] Local MMA / combat sports forums and subreddits — r/MuayThai, r/london, r/Beckenham

### 5. Local backlinks (each one moves the needle)
- [ ] [London Borough of Bromley](https://www.bromley.gov.uk) — community sports listings
- [ ] [Beckenham Town Council / Business directory](https://beckenhambusiness.com) (if exists)
- [ ] Local press: News Shopper Bromley, This Is Local London — pitch a Liam Nolan profile piece
- [ ] Local schools — offer free taster sessions, get a backlink from the school site
- [ ] Local podcasts / YouTube fitness channels — Liam as a guest, link in description
- [ ] Beckenham Cricket Club, Crystal Palace FC community pages, local gyms (cross-listing)

### 6. Social signals (correlate with rankings even if not direct)
- [ ] Instagram bio must link to nolanmuaythai.com (it does ✅)
- [ ] Facebook business page (not personal profile) with the canonical NAP and website link
- [ ] YouTube channel for the intro reel + class clips — embed each video on relevant pages, link description back to site

### 7. Reviews strategy (the loop)
1. Print QR-coded "Review us on Google" cards. Hand them out after every kids class to parents (highest review rate).
2. Add a post-class WhatsApp template: "Thanks for training tonight, mind dropping us a Google review? [link]"
3. Target: **20 net-new Google reviews over the next 60 days, 4.8+ average**.
4. Reply to every review within 48 hours. Mention "Beckenham" or "Bromley" in the reply text (Google reads these).

---

## 60-day priority plan

| Week | Action | Owner | Outcome |
|------|--------|-------|---------|
| 1 | Merge this PR | Ozzie | On-page foundation set |
| 1 | Claim / optimise Google Business Profile | Ozzie | Cornerstone for local pack |
| 1–2 | Submit to top 8 directories | Either | NAP consistency built |
| 2 | Add testimonial section + AggregateRating schema (when reviews ≥ 5) | Me | Trust signal live |
| 2–4 | Start review push (QR cards + WhatsApp templates) | Liam | +20 Google reviews |
| 4 | Pitch News Shopper / This Is Local London | Ozzie | Local press backlink |
| 4–6 | Add visible FAQ + Why Choose Us sections | Me | More long-tail keywords |
| 6–8 | Reassess rankings in Google Search Console | Ozzie | Validate progress |

---

## Tracking — set these up if not already

- [ ] [Google Search Console](https://search.google.com/search-console) — verify domain, submit sitemap, check "Muay Thai Beckenham" position weekly
- [ ] [Bing Webmaster Tools](https://www.bing.com/webmasters) — same drill
- [ ] [Google Business Profile Insights](https://business.google.com) — track calls, direction requests, profile views

GA4 is already installed (`G-G2VCKNYKYR`). Make sure Google Ads / GBP is linked.

---

## What I still need from you to push further

1. **A real number of Google reviews + average rating** → I'll add `AggregateRating` schema and a testimonial strip.
2. **5–10 actual review quotes** (member name + neighborhood okay) → I'll style them as testimonial cards.
3. **Confirmation Google Business Profile is claimed** → if not, do that today; I can't claim it for you.
4. **Permission to add a "Why Beckenham Trains Here" content block** with 200–300 words of natural local copy.

Hit me on any of the above and I'll push the next round.

---

*Audit prepared by ABMBot-Master, June 2026. Branch: `seo-tune-jun2026`.*
