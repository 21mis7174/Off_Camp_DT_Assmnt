# DeepThought Round 1: Finding 25 Target Companies

## What this is about

This project finds companies that DeepThought can work with. These are companies with 50 crore to 500 crore revenue that want to build better systems inside their business. They're called Federer companies - they have good products, capable founders, and they want to improve how they run things.

---

## Part A: We found 25 companies

### What we did

We researched companies to find 25 good targets. Here's how we did it:

1. We gathered company names from government websites (MCA, DSIR, Google search)
2. We checked if they were real manufacturers (not just traders or distributors)
3. We checked if they operate in India with a real office or facility
4. We scored each company on 6 criteria to see how good a fit they are
5. We picked the top 25

### Two key checks we did

E1 check: Is the company a real producer? Does it make things or deliver services in its own facility? We removed traders and distributors.

E2 check: Is the company actually in India where we can visit and work? Not just registered but has real operations we can access.

### Scoring criteria

We scored companies on:
- Differentiation: Do they have patents, special equipment, or unique processes?
- Decision-maker quality: Is the founder or CEO well-educated or do they understand business systems?
- Growing sector: Is the industry getting support from government or growing fast?
- Growth signals: Is the company hiring, expanding, getting certifications?
- Systems maturity: Do they have ERP software, structured costing, organized planning?
- Leadership: Do they have people trained to take over? Do they have good managers outside the family?

### Output files from Part A

company_top25_shortlist.csv - The 25 companies we selected with their scores and evidence for each criterion

company_scored_companies_ranked.csv - All 104 companies we researched, ranked by score

---

## Part B: Strategy to find 1000 companies

### The challenge

Finding 25 companies manually took a lot of time. We needed a plan to find 1000 companies but without taking forever.

### Our strategy

We split it into 4 weeks and made each week simpler:

Week 1: Gather 2500 company names from government sources and industry associations. Keep the basics like name, website, location.

Week 2: Filter down to real producers (E1 check) - about 1400 companies stay. Then filter to accessible companies in India (E2 check) - about 1200 stay.

Week 3: Quick screening - classify each of 1200 as high potential, medium, or low in 5 minutes each. Then deep research the top 300-400 high potential ones in 15 minutes each.

Week 4: Rank all 1200, pick top 1000. Spot check 20 random ones to make sure they're real. Save the final list.

### Why this works

We don't score all 1000 deeply. That would take too long. Instead we screen first to narrow down, then only deep dive on the best ones. This saves a lot of time.

### Files from Part B

PART_B_ANSWERS.txt - Detailed answers about where to find companies and the full 4-week plan

FLOWCHART_DIAGRAM_TO_DRAW.txt - Step by step instructions for drawing the flowchart on paper

1000_company_sourcing_flowchart.png - Hand-drawn flowchart showing the complete process

---

## The notebooks and scripts

04_company_ranking_pipeline.ipynb - Python notebook that filters, ranks, and exports the 25 companies from a larger list

This notebook:
- Loads company data from CSV
- Checks eligibility gates (E1 and E2)
- Ranks by total score
- Exports the top 25
- Exports other rankings for review

---

## What we learned

Company research at scale requires:
1. Good data sources - government data, associations, industry lists
2. Automation where possible - use scripts to check websites, filter traders, verify locations
3. Smart filtering - don't score everything deeply, screen first then focus
4. Quality checks - spot check random companies to catch mistakes

---

## How to use this

If you want to find 25 companies:
1. Use company_top25_shortlist.csv
2. Read PART_B_ANSWERS.txt for the methodology
3. Look at the notebook to see how we processed the data

If you want to scale to 1000 companies:
1. Read the 4-week plan in PART_B_ANSWERS.txt
2. Look at the flowchart to see the stages
3. Use the notebook as a template for automation
---

## Files in this folder

output/final_csv/ - CSV files with company data
- company_top25_shortlist.csv - The 25 companies we selected
- company_scored_companies_ranked.csv - All companies ranked by score

notebooks/ - Python notebooks
- 04_company_ranking_pipeline.ipynb - Code to filter, rank, and export companies

PART_B_ANSWERS.txt - Answers to the 2 questions in Part B
FLOWCHART_DIAGRAM_TO_DRAW.txt - Instructions for drawing the flowchart
1000_company_sourcing_flowchart.png - Hand-drawn flowchart of the strategy

---

## Summary

We successfully found 25 qualified companies through careful research and scoring. We also created a realistic plan to scale this to 1000 companies in 4 weeks. The key insight is: don't score everything deeply, screen first then focus on the best ones.

