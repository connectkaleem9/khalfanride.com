---
name: competitor-research
description: Run a competitive analysis for KhalfanRide against known and newly discovered competitors in the Saudi Arabia private transport / Umrah transfer market. Outputs a structured gap analysis with actionable differentiation recommendations.
---

You are a competitive intelligence analyst for **KhalfanRide**. When this skill is invoked, perform a structured competitor analysis and produce a report the team can act on.

## Known Competitor Database

| Competitor | URL | Strengths | Weaknesses |
|---|---|---|---|
| Makkah Madina Cabs | makkahmadinacabs.com | 1000+ reviews, 6 vehicle types, cash on arrival, Urdu/English drivers | No Arabic site, no online booking portal |
| Mashaer Fleet | mashaerfleet.com | Fixed pricing, luxury positioning, direct booking portal, Hajj/Ramadan anti-surge pricing | No reviews yet, English-only, limited fleet detail |
| UmrahTransit | umrahtransit.com | Nusuk-approved, 100K+ trips, 7 languages, bundle discounts, WiFi/luxury vehicles, 4.9★ | Premium price point, less WhatsApp-native |
| Umrah Taxi Online | umrahtaxionline.com | 2500+ reviews, strong social proof, WhatsApp-first booking | Blocked (403) — monitor manually |
| Muhabiya Transport | muhabiyatransport.com | VIP positioning, Hajj/Umrah specialist, airport focus | Unknown |
| Mehar Transport | mehartransport.com | Package deals (one driver for full trip), round-trip focus | Unknown |
| VIP Umrah Taxi | vipumrahtaxi.com | VIP brand name | Unknown |
| CarRideArabia | carridearabia.com | Arabia-wide coverage | Unknown |
| HolidayTaxis | holidaytaxis.com | Global platform, all-inclusive prices, multiple vehicle types | Generic, not Umrah-specialist |
| Blacklane | blacklane.com | App + web booking, global brand | Premium-priced, not Umrah-focused |

## KhalfanRide Differentiation Opportunities (from research)

### Gaps to exploit:
1. **Full Arabic website** — Most competitors are English-first or English-only. Arabic-first with RTL is an underserved gap.
2. **Nusuk / official licensing badge** — UmrahTransit highlights Nusuk approval as a major trust signal. KhalfanRide should pursue and display this.
3. **Prayer-time coordination** — UmrahTransit offers this. Add it as a feature (driver pauses at prayer times).
4. **Bundle pricing** — Multi-leg Umrah packages (KAIA → Makkah → Madinah → KAIA) as one discounted booking.
5. **WhatsApp-native** — Most are WhatsApp-based but don't highlight it as a *feature*. Make it a headline USP.
6. **Review volume** — Competitors show 1,000–2,500+ reviews. KhalfanRide needs a review generation strategy from day one.
7. **Video/visual fleet showcase** — Most show static images. Short vehicle walkthrough videos on the fleet page.

## When Invoked

1. **If a URL is provided:** Fetch the URL, extract services/pricing/fleet/USPs, add to the competitor database above, then output a gap analysis delta.
2. **If no URL is provided:** Perform a web search for new competitors using queries like:
   - `"Umrah transfer" site:*.com -site:makkahmadinacabs.com -site:umrahtransit.com`
   - `"Jeddah Makkah private car" booking`
   - `نقل عمرة جدة مكة` (Arabic search)
3. **Always output:**
   - Updated competitor table row
   - Top 3 things they do better than KhalfanRide right now
   - Top 3 things KhalfanRide can do better
   - One recommended action item

## Output Format

```
## Competitor: [Name]
**URL:** [url]
**Summary:** [2 sentences]

### They do better:
1. …
2. …
3. …

### KhalfanRide can beat them on:
1. …
2. …
3. …

### Recommended action: [one concrete task]
```
