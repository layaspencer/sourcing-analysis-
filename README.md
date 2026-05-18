# Sourcing Analysis with AI

This project analyzes a fictional sourcing and recruitment dataset to identify funnel conversion patterns, candidate advancement signals, and practical recommendations for recruiters.

The goal is not only to describe what happened in the process, but to support better recruiting decisions through funnel analysis, candidate prioritization, and AI-assisted interpretation of qualitative notes.

## Business Question

How can a recruiting team use sourcing funnel data and AI-assisted qualitative analysis to identify stronger conversion patterns, reduce time spent on low-probability candidates, and improve recruiter follow-up decisions?

## Objective

This analysis aims to answer:

- Which sourcing channels convert best
- Where candidates drop in the funnel
- Which candidate signals indicate a higher chance of advancing
- When recruiters should persist with a candidate
- When there is a low probability of conversion
- How AI can support recruiter decision-making

## Project Structure

- `sourcing_analysis.ipynb` — main analysis notebook and technical solution demonstration
- `sourcing_analysis_presentation.pptx` — short visual presentation used as an additional solution walkthrough
- `sourcing_analysis_report.pdf` — short report explaining the approach, AI usage, key insights, and recommendations
- `sourcing_analysis_summary.md` — written summary of the analysis
- `mock_sourcing_dataset.csv` — dataset used by the notebook
- `mock_sourcing_dataset.xlsx` — original dataset file
- `requirements.txt` — Python dependencies

## Methodology

The analysis includes:

1. Funnel conversion analysis across recruitment stages
2. Conversion comparison by sourcing channel
3. Conversion comparison by recruiter
4. Candidate signal analysis using scores, seniority, response behavior, and rejection reasons
5. AI-assisted classification of qualitative recruitment notes into structured insight categories
6. Practical recommendations for recruiter prioritization and process improvement

## AI Usage

AI was used as a qualitative structuring layer, not as an automated decision-maker.

The AI-assisted workflow classifies unstructured recruiter notes into consistent categories such as:

- Salary risk
- Low engagement
- Timing issue
- Technical mismatch
- Strong technical fit
- High-potential candidate

These categories support pattern recognition and recruiter prioritization. Final recommendations remain based on structured funnel data, business context, and human interpretation.

## Recruiter Action Framework

Based on the funnel and candidate signal analysis, candidates can be grouped into four practical action categories.

### 1. High Priority

Candidates with strong technical or manager scores, good engagement, advanced funnel progress, and no major salary or timing concern.

**Recommended action:** prioritize follow-up and keep the process moving quickly.

### 2. Nurture

Candidates with positive signals but current timing, availability, or readiness limitations.

**Recommended action:** keep warm for future opportunities.

### 3. Risk / Validate Early

Candidates with mixed signals, salary concerns, unclear motivation, or weak engagement.

**Recommended action:** clarify risks early before investing additional process time.

### 4. Low Probability

Candidates with no response, low fit, failed technical assessment, or repeated low engagement.

**Recommended action:** deprioritize unless new information changes the assessment.

## Key Recommendations

- Prioritize high-converting sourcing channels with stronger hired-stage outcomes.
- Investigate the test-to-offer bottleneck to understand whether the issue is technical readiness, process timing, compensation, or hiring manager alignment.
- Use AI-assisted note classification to identify recurring candidate risks earlier.
- Apply a candidate prioritization framework to separate high-priority, nurture, risk-validation, and low-probability profiles.
- Compare recruiter funnel patterns carefully, considering role difficulty, seniority mix, assigned requisitions, and channel strategy.

## Limitations

- The dataset is fictional and should be interpreted as a sample scenario.
- Recruiter conversion may be influenced by role difficulty, candidate seniority, channel mix, and assigned requisitions.
- AI-generated categories should support recruiter review, not replace human judgment.
- Additional data such as time-in-stage, compensation expectations, hiring manager feedback, and candidate availability would improve the analysis.

## Future Improvements

If expanded, this project could become a recruiter decision-support dashboard with:

- Candidate prioritization scoring
- Channel performance monitoring
- Bottleneck alerts
- AI-assisted note tagging
- Follow-up recommendations
- Recruiter coaching insights based on funnel patterns
