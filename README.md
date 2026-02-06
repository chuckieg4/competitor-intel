# 🐕 UndrDog Creative Director Hub

The ultimate creative operations center for the UndrDog team. A single-page application providing everything the creative team needs to win.

## 🚀 Quick Start

Simply open `index.html` in any modern browser. No build step required.

```bash
# If you have Python installed
python -m http.server 8000
# Then visit http://localhost:8000

# Or with Node
npx serve .
```

## 📊 Features (10 Tabs)

### Tab 1: Performance Dashboard
- **Top 10 Performers** — Last 7 days with CPA, spend, purchases
- **Winners Wall** — All-time best performers with 🏆
- **Format Breakdown** — STAT vs UGC vs VID vs DrChris performance
- **Creator Leaderboard** — Who's producing winners
- **CPA Trend Chart** — Visual trend over time

### Tab 2: Competitor Intel
- **Offer Comparison** — Side-by-side pricing and guarantees
- **Competitor Deep Dive** — Cards for each competitor with:
  - Ad count and creative mix
  - Current offers
  - What's working for them
  - **"Steal This"** — Actionable hooks to swipe
- **Trends** — What's working industry-wide and gaps to exploit

### Tab 3: Creative Briefs
- **Active Briefs** — Current briefs with status, creator, and due dates
- **Brief Templates** — By angle (destructive, health, fit, conspiracy)
- **Hook Library** — Proven scroll-stopping openers by category

### Tab 4: Brand Bible
- **Product Overview** — DuraFlow™ fabric, Alpha Frame Fit
- **Messaging Pillars** — Core brand messages
- **Legal Rules** — ⚠️ Do's and don'ts for compliance
- **Voice & Tone** — How to sound like UndrDog
- **Terminology** — Words to use vs avoid

### Tab 5: Asset Library
- **Creator Folders** — Quick access to each creator's content
- **Content Type Folders** — AOA, B-Roll, Music, Product Shots
- **Destructive Demo Library** — Fire, knife, BB gun, etc.

### Tab 6: Research Vault
- **Approved Studies** — All 8 PubMed studies with:
  - Key findings
  - How to cite (copy-ready)
  - Direct links
- **Citation Guide** — How to frame health claims legally

### Tab 7: Creator Hub
- **Creator Profiles** — MTRX, Aaron, Dr. Chris, Chino, Dalton, Growthpod
- **Performance Stats** — Avg CPA, weekly spend, total winners
- **Current Assignments** — What they're working on
- **Best For** — What each creator does best

### Tab 8: Script Frameworks
- **UGC Rewriter** — The complete Human Ad Script framework
- **Script Structures** — Problem-Agitate-Solution, 3 Reasons, etc.
- **Hook Formulas** — Templates for scroll-stopping openers
- **Demo Templates** — Destruction, smell test, side-by-side

### Tab 9: Calendar
- **Upcoming Drops** — Feb: Project 000, Mar: Polos, Apr: Boxer Briefs
- **Past Drops** — Blue Steel, White Yeti, Daddy Claus, Agent Gold
- **Content Deadlines** — Who needs to deliver what by when
- **Testing Schedule** — Weekly focus areas

### Tab 10: Daily Briefing
- **Auto-generated Summary** — Quick snapshot of today
- **Focus Today** — Top priorities
- **Recent Wins** — Learn from successes
- **Fires to Put Out** — Urgent issues
- **Quick Actions** — Checkable task list

## 📁 Files

```
competitor-dashboard/
├── index.html          # The hub (single-page app)
├── index-backup.html   # Backup of previous version
├── data.json           # All data (edit to update)
└── README.md           # This file
```

## 📝 Updating Data

All data lives in `data.json`. The schema includes:

```javascript
{
  "meta": { /* version, dates */ },
  "performance": { /* top performers, winners, formats, creators, trends */ },
  "competitors": [ /* competitor cards with offers, creatives, steal-this */ ],
  "offerComparison": [ /* pricing table */ ],
  "briefs": { /* active briefs, templates */ },
  "hookLibrary": { /* hooks by category */ },
  "brandBible": { /* product, voice, legal, messaging */ },
  "research": { /* approved studies with citations */ },
  "assets": { /* folder structure */ },
  "creators": [ /* creator profiles */ ],
  "scriptFrameworks": { /* UGC rewriter, structures, formulas */ },
  "calendar": { /* drops, deadlines, testing */ },
  "dailyBriefing": { /* today's focus, wins, fires, actions */ },
  "trends": { /* working, gaps, watch */ }
}
```

### Update Frequency
- **Daily Briefing** — Update daily (or leave static for now)
- **Performance** — Update weekly from Meta Ads
- **Competitors** — Update weekly from Ads Library scans
- **Briefs** — Update as briefs change
- **Everything else** — Update as needed

## 🎨 Design

- **Dark theme** — Easy on the eyes
- **Mobile responsive** — Works on all devices
- **Tab-based navigation** — Quick access to everything
- **No dependencies** — Pure HTML/CSS/JS

## 🔧 Customization

### Adding a new competitor
Add to `data.json` → `competitors` array:
```json
{
  "name": "New Brand",
  "tier": 1,
  "site": "newbrand.com",
  "adCount": "~100",
  "offers": [{ "label": "First Order", "value": "20% off" }],
  "whatsWorking": ["Their winning tactics"],
  "stealThis": ["Ideas to test"]
}
```

### Adding a new study
Add to `data.json` → `research.approvedStudies`:
```json
{
  "id": "S009",
  "title": "Study Title",
  "author": "Author et al",
  "year": 2024,
  "pubmedId": "12345678",
  "keyFinding": "What they found",
  "howToCite": "How to phrase it safely",
  "link": "https://pubmed.ncbi.nlm.nih.gov/12345678/"
}
```

### Adding a new creator
Add to `data.json` → `creators`:
```json
{
  "name": "New Creator",
  "type": "UGC Creator",
  "specialty": ["Talking head", "Demos"],
  "bestFor": "Specific use case",
  "weeklySpend": "$5-10K",
  "currentAssignment": "Current project",
  "avgCpa": 45.00,
  "totalWinners": 0,
  "contact": "Via email",
  "notes": "Notes about them"
}
```

## 🔮 Future Ideas

- [ ] Real-time Meta Ads API integration
- [ ] Search functionality across all content
- [ ] Export reports to PDF
- [ ] Slack integration for notifications
- [ ] Brief generator form
- [ ] Creative scoring system

## 📞 Support

Questions? Ask Jerry (the AI) in #jerry-ai or reach out to the creative team.

---

*Built with 🐕 for UndrDog — Feb 2026*
