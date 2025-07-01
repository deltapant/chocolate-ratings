# chocolate-ratings
6-1
*Source:*
The Chocolate Bar Ratings dataset, sourced from Kaggle, contains 1,795 sensory reviews
of 440 unique chocolate bars contributed by a community of chocolate enthusiasts from
2006 to 2017.
*Key Features:*
• Company: Chocolate manufacturer (416 unique)
• BarName: Bean origin or bar variant (1,039 unique)
• REF: Unique bar identifier
• ReviewDate: Year reviewed
• CocoaPercent: Cocoa content (%)
• Location: Country of production (60 total)
• Rating: Sensory score (1.0 to 5.0)
• BeanType: Cacao variety / blend (41 types; ~50% missing)
• BroadOrigin: Country of bean origin (100 total)
Reviews were submitted by professional and amateur tasters who entered bar details and
scores after sampling. Metadata (origin, maker location, cocoa %) came from tasters or
manufacturer information. Data is voluntary and not sampled.
*Data Limitations*
1. Scope: No reviews after 2017.
2. Bias: Reviewers are likely chocolate enthusiasts instead of general consumers.
3. Missing Data: About 50% of BeanType entries are blank, limiting varietal analysis.
4. Licensing: Open for educational use but not commercial.
*Why I Chose It*
I chose this dataset for its relevance to my interest in specialty foods and flavor profiling. Its
geographic and variable diversity enables spatial and statistical analysis of how origin,
formulation, and time affect chocolate quality.
*Ethical Considerations*
1. Attribution: Requires citation.
2. Privacy: No personal data here.
3. Bias: Submissions may overrepresent niche bars.
*Questions*
• How does CocoaPercent relate to Rating?
• What are rating trends from 2006–2017?
• Which BroadOrigin countries have the highest average ratings?
• Do ratings vary by Company Location (eg: U.S. vs. Europe)?
• How do BeanType categories compare in average rating?
• Can a bar’s Rating be predicted from CocoaPercent, Origin, and Company?
• Do trends show shifting preferences for dark vs. lower-percentage chocolate?
*Data Cleaning Steps*
• Column Names: Removed line breaks/extra spaces and standardized names (e.g.,
Company, BarName, CocoaPercent).
• Data Types: Converted CocoaPercent from string (e.g., “70%”) to float (70.0);
ensured ReviewDate and Rating are numeric.
• Missing Values: Replaced 887 missing BeanType entries with “Unknown”; retained
1 missing BroadOrigin for transparency.
• Duplicates: No exact duplicates; multiple entries per REF are expected due to
multiple reviews.
• Integrity Checks: All key fields were validated; no out-of-range values found in
CocoaPercent.
