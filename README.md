# Big Easy Roofing, service and location cluster page prototypes

Three directions for the third level of BER's location cluster, the page that does not exist yet:
**one service in one city**. Sample page is Roof Replacement in Metairie, LA.

Proposed URL pattern: `/service-areas/louisiana/metairie/roof-replacement/`

## Open it

`index.html` is a picker. Keys `1` `2` `3` or the arrow keys switch variants, `R` replays the entrance.
Each variant is also a standalone page: `variant-a.html`, `variant-b.html`, `variant-c.html`.

| Variant | Axis | Leads with |
|---|---|---|
| A, Price Led | Information density | The published cost band and an interactive size estimator |
| B, Local Authority | Editorial and place | Metairie itself, the parish rules, long form reading |
| C, Cluster Console | Navigation and system | A service and city switcher, comparison table, the full 98 page matrix |

## Colour and type

Measured off the live bigeasyroofing.com homepage with a real browser on 2026-08-30, not guessed.

| Token | Value | Where it comes from |
|---|---|---|
| Yellow | `#ffeb01` | Primary CTA fill, black text, 45px pill |
| Blue | `#2388da` | Secondary CTA fill, and the second phrase in every heading |
| Deep blue | `#15477e` | Used here for blue *text*, because `#2388da` on white is 3.75:1 and fails small text |
| Navy | `#071018` | Dark bands and body text |
| Cream | `#f8f5ef` | Alternate section background |
| Sand | `#eeeadd` | Table headers and panels |
| Headings | Poppins 700 | Live site |
| Body | DM Sans 500, 18px | Live site |

Two live site defects were deliberately **not** copied, since this is a new page and not a retrofit:
H1 and H2 both render at 60px/700 on the live site with no step between them, and H3 is split across
Poppins and DM Sans. These prototypes use a real type scale and one heading family.

## Facts on the page, and where they came from

Verified at source on 2026-08-30:

- Jefferson Parish residential re roofing permit is **$50**, paid by card via MGO Connect, no plans
  and no survey required. Source: jeffparish.gov. **This corrects the $175 figure carried in the
  earlier prototype round.**
- From **1 January 2026**, residential roof work valued at **$7,500 or more** requires a Louisiana
  Residential Roofing or Residential Construction licence. Source: jeffparish.gov, statute
  La. R.S. 37:2156.4. A Codex cross-check corrected this from "over $7,500"; the statute reads
  "or more", and on a threshold claim that difference is the whole claim.
- Re roofing must comply with the **2021 International Residential Code**. Source: jeffparish.gov.
- Jefferson Parish sends **no inspector**. Phases are verified from geo tagged photographs showing
  the nailing pattern and material packaging with wind ratings. Source: jeffparish.gov.
- Louisiana Fortify Homes Program grants **up to $10,000**, "limited to construction costs", toward
  a roof that meets the FORTIFIED standard, and the homeowner pays everything above the grant plus
  the separate evaluator fees. The grant must be **awarded before work starts**. Source: ldi.la.gov.
  A Codex cross-check corrected an earlier draft that described it as covering only the incremental
  upgrade above a standard replacement, which understated it.
- Phone `(504) 800-8196` and address `4523 Croyden Ave, New Orleans LA` read from the
  `RoofingContractor` JSON-LD in BER's own page source, not off a rendered page.

**Not verified, needs BER sign off before launch:** every price band ($7,000 to $18,000,
$16,000 to $28,000, $65 to $95 a sheet, $1,800 to $4,500, $900 to $2,400) and the
neighbourhood characterisations in variant B. These come from BER's own unpublished draft copy.

## Cross-check

A Codex CLI cross-check was run over all seven factual and accessibility claims on 2026-08-30.
It confirmed five and **rejected two**, both of which were then verified at source and corrected
in all three variants: the licence threshold wording, and the scope of the state grant. Regulatory
statements now carry an "as of August 2026" line on the page, also on its recommendation.
No second-model review of the prose itself has run.

## Images

Two photos, both from BER's own media library and both checked at full size first.
`hero-tearoff.jpg` and `crew.jpg` are asphalt shingle work on US housing stock.
The two files in BER's library actually named "Metairie" were **rejected**: both show
Mediterranean terracotta barrel tile, which does not exist on Metairie housing stock.
