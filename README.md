# Subspace.money &mdash; Product Teardown

**A deep product teardown of India's subscription sharing platform, prepared as a take-home assignment for a Product Intern role.**

> Built by Raghav Agarwal &middot; May 2026 &middot; [Live Preview](https://raghav26102000.github.io/subspace-product-teardown)

---

## What This Is

A full-stack product analysis of [Subspace.money](https://subspace.money), an Indian subscription-sharing marketplace generating &#8377;36.5 Cr in annual revenue. The teardown covers trust architecture, monetization mechanics, operational friction, user psychology, and growth constraints, backed by live app screenshots taken from a real account on May 29 to 30, 2026.

This is not a generic PM framework exercise. Every observation is tied to a specific screen, flow, or Play Store review. Every recommendation is shippable with low to medium engineering effort.

---

## What Is Covered

| Section | Description |
|---|---|
| Executive Summary | The 3.5-star problem in one paragraph |
| ICP Analysis | Three distinct user segments with opposing incentives |
| Market Positioning | Why "savings app" is the wrong frame |
| Competitor Landscape | OTT platform risk, SplitGenie, CRED as trust benchmark |
| User Journey Map | 7-step flow with friction tags |
| Key Friction Points | 6 observed issues with screen evidence |
| Product Moat Analysis | What is actually defensible vs. marketing |
| Retention Mechanics | What works, what is broken, and why |
| Growth Opportunities | Tiered across 0 to 6 months, 6 to 18 months, 18+ months |
| Prioritization Matrix | 13 initiatives with P0 to P4 ranking, effort, and key metric |
| 5 Core Feedbacks | Premium identity, trust at checkout, homepage auth wall, admin experience, product sprawl |
| Microcopy Rewrites | 6 before and after rewrites with behavioral principle per change |
| What Most Applicants Will Say | 5 shallow takes and why each is wrong |
| Founder Insights | What actually matters to the business: GMV, AI Mailbox, Superflow, OTT risk window |
| If I Joined Tomorrow | 4-week sprint with hypothesis-based impact estimates |
| 30 Day Roadmap | Day-by-day plan with deliverables and success metrics |
| High Risk / High Reward Ideas | AI subscription audit, savings social layer, Subspace for Teams, campus groups |
| Metrics Framework | 10 metrics with context on why each one matters |
| Appendix A | 12 annotated app screenshots |
| Appendix B | Corrected competitive audit |
| Appendix C | 10 Play Store reviews, filterable by theme |
| Appendix D | 5 product ideas considered and rejected with reasoning |

---

## The 5 Core Feedbacks

**01 &mdash; Premium Has No Identity**
The Premium product card displays "0.0M" subscribers on Subspace's own monetization product. This is textbook negative social proof on the monetization tier. Sold via "Add to Cart" like a Netflix group slot, with no contextual upgrade prompt, the tier has near-zero conversion.

**02 &mdash; Trust Signals Vanish at Checkout**
Admin ratings (up to 5 stars with 1,790+ reviews) are visible in group listing. At checkout, all of that disappears. The admin with 1,790 reviews is just a name at the moment of highest anxiety. The fix costs zero new infrastructure. It is a placement decision.

**03 &mdash; The Homepage Is an Auth Wall**
subspace.money loads with a login modal before showing any product value. A user searching "cheap Netflix India" sees nothing without signing in. The Explore tab with 145+ Netflix groups and live admin ratings is exactly what would convert a skeptical visitor, and it is locked behind auth.

**04 &mdash; The Admin Experience Is Underserved**
Admins with 3-year track records and 1,790+ reviews have no dashboard, no automated payment reminders, and an account-blocking bug that punishes them for removing members who requested removal. One admin leaving equals four to five simultaneous member churn events.

**05 &mdash; Multiple Businesses Fighting for the Same Screen**
Six competing CTAs on the Home screen. Rental feature leads the Explore page above subscription groups. Five tabs at equal visual weight. Hick's Law in action. For a founding team of four managing active operational failures in May 2026, this surface area is an impossible trade-off.

---

## Key Observations Backed by Screenshots

| Screenshot | What It Proves |
|---|---|
| `sub premium.jpeg` | "0.0M" subscribers visible on Premium card |
| `netflix group3.jpeg` | Admin rating missing at checkout despite existing in listing |
| `Wallet.jpeg` | "Locked Amount" displayed in red, the escrow protection looks like a debt |
| `home.jpeg` | 6 competing CTAs with no hierarchy toward core loop |
| `Explore1.jpeg` | Rental feature leads Explore page above subscription groups |
| `netflix group2.jpeg` | Admin trust infrastructure (5 stars, 1.79K reviews) exists in listing |
| `money saved tab.jpeg` | Viral loop (Top Savers, Share button) buried at Account item 5 of 12 |
| `ai mail box.jpeg` | AI Mailbox (@rylo.club) exists but is never surfaced at group-joining |

---

## Structure

```
SUBSPACE/
├── index.html    # Interactive report (open in browser)
├── Subspace_Product_Teardown_Raghav_Agrawal.pdf
└── assets/
    ├── home.jpeg
    ├── Explore1.jpeg
    ├── Explore2.jpeg
    ├── netflix group.jpeg
    ├── netflix group2.jpeg
    ├── netflix group3.jpeg
    ├── sub premium.jpeg
    ├── Wallet.jpeg
    ├── money saved tab.jpeg
    ├── ai mail box.jpeg
    ├── account.jpeg
    ├── account1.jpeg
    ├── chat.jpeg
    ├── rating-1star.jpeg
    ├── rating-1starII.jpeg
    ├── rating-2star.jpeg
    ├── rating-3star.jpeg
    ├── rating-4star.jpeg
    └── [annotated versions of key screens]
```

---

## How to View

**Option 1 &mdash; Open the HTML file directly**
Download `index.html` and open it in any browser. All images are embedded. No server required.

**Option 2 &mdash; GitHub Pages**
Visit the live version at `https://raghav26102000.github.io/subspace-product-teardown`

**Option 3 &mdash; PDF**
`Subspace.money-Product Teardown 2026.pdf` is a print-ready version of the full report.

---

## Interactive Features

- Collapsible side navigation with active section tracking
- Animated number counters on scroll
- 3D phone gallery for app screenshots with drag-to-scroll
- Click any annotated screenshot to open in fullscreen lightbox
- Filterable Play Store review cards by theme
- Scroll progress indicator
- Fade-in section animations
- Mouse parallax on cover

---

## Evidence Standards

Every claim in this teardown is tagged with one of three evidence levels:

- **Observed** &mdash; directly seen on subspace.money, Play Store listing, or from live app screenshots taken May 29 to 30, 2026
- **Inferred** &mdash; derived from Play Store reviews, behavioral data from analogous products, and first-principles reasoning from product structure
- **Hypothesized** &mdash; strategic reasoning about what is likely true, flagged explicitly. Impact estimates are directional hypotheses, not guarantees

**Sources**

| Data point | Source |
|---|---|
| &#8377;36.5 Cr annual revenue | Tracxn FY25 |
| Team size and founders | Tracxn / LinkedIn |
| App features and flows | Live account screenshots, May 2026 |
| Play Store reviews | Google Play Store, latest version, 1 to 4 stars sampled |
| App rating 3.5 stars | Play Store listing, May 2026 |
| Competitor data | Public sources |

---

## About the Author

**Raghav Agarwal** &mdash; Full Stack Engineer and aspiring Product Manager

- GitHub: [@raghav26102000](https://github.com/raghav26102000)
- LinkedIn: [linkedin.com/in/raghav-agarwal26](https://linkedin.com/in/raghav-agarwal26)

Background in full-stack engineering (React, Next.js, FastAPI), GenAI and RAG systems, and data analytics. Currently exploring roles at the intersection of product, engineering, and growth.

---

*This teardown was prepared as a take-home product intern assignment in May 2026. All analysis is the author's own. Revenue figures are sourced from Tracxn and are publicly available.*
