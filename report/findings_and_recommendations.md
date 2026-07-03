# Retail Sales — Findings & Recommendations

## Key Findings

**Time Trends**
- Revenue is volatile month to month rather than steadily growing — May was the peak (~53,000), 
  followed by a sharp drop in September (~24,000) before recovering into Q4 (Oct–Dec).
- There is no clean upward or downward trend across the year; the business shows seasonal 
  spikes rather than consistent growth.
- The near-zero data point at Jan 2024 is likely a data artifact (only one or two stray 
  transactions logged into that period) rather than a real collapse in sales — worth flagging 
  as a data quality note rather than a business finding.

**Weekly Pattern**
- Saturday is the strongest day for revenue (~79,000), followed by Monday and Tuesday.
- Thursday is the weakest day (~54,000), with Sunday and Wednesday also trailing behind 
  the rest of the week.
- Combined with the heatmap, the strongest revenue cells cluster on Saturdays in April, 
  June, and October–December, suggesting weekend demand compounds with certain seasonal windows.

**Category Performance**
- Revenue is fairly evenly split across the three categories: Electronics (~157,000), 
  Clothing (~155,000), and Beauty (~143,000).
- Unlike many retail datasets where one category dominates, no single category is driving 
  the business — this points to a genuinely diversified product mix.

**Customer Demographics**
- The 45–55 age group generates the highest revenue (~100,000), followed closely by 25–35.
- The youngest (18–25) and oldest (55–70) age brackets contribute noticeably less, suggesting 
  the core customer base sits in the mid-career age range.

**Gender**
- Average spend is nearly identical between Female ($456.55) and Male ($455.43) customers — 
  a difference of about $1, which is not meaningful. Gender does not appear to be a useful 
  variable for segmenting marketing or promotions in this dataset.

**Top Customers**
- Every customer in this dataset made exactly one purchase — there are no repeat buyers at all. 
  The "top 10 customers by spend" are therefore simply the 10 largest single transactions, 
  not loyal or returning customers. This means customer retention cannot currently be measured 
  or improved from this dataset as-is; it would require order history over a longer time window 
  or a larger sample to observe repeat behavior.

## Recommendations

1. **Investigate the September dip.** A near 50% drop from May's peak is significant — check 
   whether it's a real seasonal lull, a stocking/supply issue, or a data gap, and plan 
   promotions or campaigns to offset it if it recurs.

2. **Shift marketing push toward Thursday and Sunday.** These are consistently the weakest 
   days — targeted discounts or flash sales on these days could help flatten the weekly dip 
   without cannibalizing already-strong Saturday traffic.

3. **Lean into cross-category bundling.** Since Electronics, Clothing, and Beauty perform 
   similarly rather than one dominating, bundle deals across categories (e.g. a clothing + 
   beauty combo) could increase basket size rather than trying to force growth in a single 
   category.

4. **Target campaigns at the 25–55 age range**, since this is where the bulk of revenue comes 
   from — but also test outreach to the under-25 and 55+ segments, which show meaningfully 
   lower engagement and may be an untapped growth opportunity.

5. **Double down on weekend capacity.** Saturday's dominance across nearly every month in the 
   heatmap suggests inventory and staffing should be weighted toward weekends, particularly in 
   Q4 and around April/June.

6. **Clean up the January 2024 data point** before presenting these findings externally — confirm 
   whether it reflects a partial month of data collection versus an actual revenue collapse.

7. **Do not segment marketing by gender.** The near-identical average spend between genders 
   means campaigns are better targeted by category interest or age group, not gender.

8. **Investigate why there are no repeat purchases.** If this reflects the real business 
   (not just a data sampling limit), it's a major finding — the business may be entirely 
   acquisition-driven with no retention. Consider introducing a loyalty program, email 
   follow-ups after purchase, or repeat-purchase discounts to start building a returning 
   customer base, since none currently exists.