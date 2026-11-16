# Biochar research portfolio — Prof. Meththika Vithanage

A quantitative assessment of Prof. Meththika Vithanage's biochar research, built from the public
[Google Scholar profile](https://scholar.google.com/citations?user=jcCDYcIAAAAJ&hl=en) (read 16 November 2026).

**View it:** https://sasikaa073.github.io/vithanage-biochar-portfolio/

## What it shows

- How many biochar outputs there are, their citations and a biochar-only h-index
- The feedstocks the biochars were made from, grouped by source
- Pristine versus modified (engineered) biochars, and the modification methods used
- Target contaminants by class, organic versus inorganic
- Soil versus water focus, and output over time
- A searchable table of every classified output

## How it was made

Every item on the profile was collected and joined with abstracts from OpenAlex and Semantic Scholar.
Biochar-related items were kept, duplicates removed, and each title and abstract was classified with
Claude (Anthropic) for output type, medium, feedstock, modification and contaminants. Limitations are
listed at the bottom of the page.

## Data

| File | Contents |
| --- | --- |
| `data/biochar_outputs.csv` / `.json` | One row per biochar output with its classification |
| `data/biochar_tags.csv` / `.json` | One row per feedstock, modification or contaminant tag |
| `data/scholar_profile.json` | Whole-profile totals from Google Scholar |

The site is a single static `index.html` with the data embedded; it uses d3 from cdnjs.
