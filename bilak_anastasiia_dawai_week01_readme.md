
# Trust and Institutions – A World Values Survey Analysis

## Overview
This project uses a random subset from the World Values Survey (Wave 7, 2017–2022) to explore the relationship between interpersonal trust and institutional trust across individuals. The dataset includes 2,007 respondents and 168 variables, focusing on social, political, and demographic indicators.

## Research Question
**Are people who trust others more likely to trust institutions?**

This analysis investigates whether individuals who express greater trust in others (e.g., family, neighbors, strangers) also tend to report higher confidence in political and social institutions (e.g., government, parliament, police).

## Dataset Information
- **File name**: `WVS_random_subset2000.csv`
- **Observations**: 2,007 respondents
- **Variables**: 168
- **Source**: [World Values Survey](https://www.worldvaluessurvey.org), Wave 7
- **Weighting**: Use `W_WEIGHT * S018` for weighted analyses

## Key Variables

| Variable | Description                            | Type     | Scale                            |
|----------|----------------------------------------|----------|----------------------------------|
| Q57      | Most people can be trusted             | Categorical | 1 = Trust, 2 = Must be careful   |
| Q58–Q63  | Trust in social groups (e.g., family, strangers, other religions) | Ordinal | 1 = Completely trust → 4 = Not at all |
| Q64–Q73  | Confidence in institutions (e.g., courts, gov, parliament) | Ordinal | 1 = A great deal → 4 = None at all |

## Descriptive Statistics (Key Variables)

Below are the summary stats for selected trust variables (see attached data table for full details):

- **Q57**: Mean = 1.69 (on 1–2 scale)
- **Q58 (Family Trust)**: Mean = 1.26
- **Q61 (Strangers)**: Mean = 2.96
- **Q71 (Trust in Government)**: Mean = 2.49
- **Q72 (Political Parties)**: Mean = 2.86

## Methodology
- Descriptive statistics were computed to understand distributions
- Missing values coded as -1, -2, -4, -5 were treated as missing (`NaN`)
- Planned next step: correlation or regression analysis between interpersonal trust and institutional trust

## Missing Data Handling
The following codes were treated as missing values and excluded from analysis:
- `-1`: Don’t know
- `-2`: No answer
- `-4`: Not asked in country
- `-5`: Missing / Unknown

## Notes
- This subset contains only one country: **Andorra**
- Not all political participation variables are available, which informed a pivot in the research question
- Institutional trust questions are well-represented

## File Naming
- Dataset: `WVS_random_subset2000.csv`
- Final README: `bilak_anastasiia_dawai_week01_readme.md`
