# Swap Across — Change log

---

## Session 2 — March 2026

### Match cards
- Simplified card layout: only matching skills are shown (no greyed-out chips)
- Removed coloured header zone — single clean white card throughout
- Replaced plain `% match` text with a filled SVG arc ring; colour matches each person's avatar

### Skill library
- Expanded from 13 to 32 skills across five categories: Tech & Digital, Life Skills, Creative, Finance & Career, Fitness & Wellbeing
- Skills are now organised with a `skillCategories` lookup used for filtering

### Skill browse (matches page)
- Replaced plain pill filter buttons with GoFundMe-style icon + label category tiles
- Added a live text search bar — filters cards as you type (e.g. "yoga", "baking")
- Category tile filter and text search work together

### Profiles
- Added 3 new profiles: Aysha (28, Yoga/Mindfulness/Illustration), Derek (68, Public Speaking/Business), Hana (19, Video Editing/Baking)
- Updated Emily bio to reflect her real backstory (lockdown confidence, finances, social media)
- Updated Liz: age corrected to 57, bio updated to match her real story

### Landing page
- Added "A real Swap Across story" section between "How it works" and "How we keep you safe"
- Shows Emily and Liz's profile bubbles, a 3-moment timeline (They matched / They met / Their community grew), and a "Start your own story" CTA
- Hero right-side visual replaced: single stacked card → Emily + Liz two-card swap layout with bidirectional swap icon

### Watermark
- Opacity increased from `0.05` to `0.09` on both the matches and meetups screens

### Meetups page
- Redesigned from stacked layout to Care.com-style 3-panel split: filter sidebar (left), scrollable card list (centre), full-height sticky map (right)
- Meetup cards redesigned as horizontal list items with colour stripe, location icon, date, and "Join meetup" button
- Filter sidebar includes: Location (London), Distance slider, Skills focus checkboxes
- Mobile: sidebar hidden, compact inline map appears above the card list
- Map pins now scroll and highlight the matching card when clicked
- "You are going to" banner appears at the top of the centre column when you join an event, with tick icon and "Going" badge

### Profile screen
- Nav profile chip is now clickable — opens a "Your profile" screen
- Shows avatar (in assigned colour), name, "What I can teach" (orange chips), "What I want to learn" (teal chips)
- Footer note: "This is how other members see your profile" + "Edit profile" placeholder

---

## Session 1 — Earlier 2026

### Project setup
- Single `index.html` prototype — no build tools, opens directly in browser
- Tailwind CSS via CDN, Google Fonts (Inter), Leaflet.js for maps

### Branding
- Inline SVG logo: 6-person circle icon (computed arc paths, matching original logo colours)
- Brand colours: orange `#E8793A`, teal `#3DBFBF`, dark charcoal `#2C3E50`, cream `#F8F6F3`
- Removed "Swap Across" text from logo (too small at nav size)

### Landing page
- Hero with headline, subheading, CTA
- "How it works" section: 3 steps with numbered circles (01/02/03)
- "How we keep you safe" section: 4 safety promise cards

### Onboarding (4 steps)
- Step 1: Name input
- Step 2: Skills you can teach (chip selection)
- Step 3: Skills you want to learn (chip selection)
- Step 4: "You're in good hands" — community promises with checkbox "I'm ready to join the Swap Across community"
- Avatar colour auto-assigned from name (no picker)

### Matches page
- Compatibility calculated from skill overlap (35% base + up to 60% from matched skills)
- Profiles sorted by compatibility
- Nav profile chip shows after onboarding is complete

### Meetups page (original)
- Interactive Leaflet.js map with 5 London meetup locations
- Custom coloured map pins; clicking a pin scrolls and highlights the matching card

### Accessibility & tone
- All emojis removed throughout
- Copy follows Unboxed voice and tone: plain English, active voice, sentence case, no exclamation marks
- `aria-hidden="true"` on all decorative SVGs
- Safety features: shield icons, public venue requirement, report profile button

### GitHub
- Repository: `saskiawrigleyunboxed/swap-across`
- All changes pushed to `main` branch
