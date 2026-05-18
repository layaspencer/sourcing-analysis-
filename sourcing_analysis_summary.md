# Sourcing Funnel Analysis with AI-Assisted Candidate Prioritization

## Objective
Analyze a fictional sourcing/recruitment dataset to identify which sourcing strategies convert best, which candidate signals indicate higher probability of advancement, where conversion drops, and how recruiters can prioritize follow-up.

## Strategic Framing
This project was approached as a recruiter decision-support analysis.
Instead of only reporting funnel metrics, the analysis focuses on how recruiters can use sourcing data to prioritize candidates, identify risks earlier, and reduce time spent on low-probability profiles.
The central question guiding the analysis was:
> How can recruiters spend more time on candidates with stronger advancement signals and less time on candidates with recurring low-conversion patterns?
This framing supports a more practical use of the data by connecting funnel performance, candidate signals, recruiter activity, and AI-assisted qualitative analysis.

## Dataset Overview
- Total candidates: 601
- Total fields: 35
- Main dimensions analyzed: source channel, recruiter, seniority, role, department, work mode, scores, funnel stage, rejection reason, and recruiter notes.
- Candidate-level PII was not used in the analysis outputs; insights are presented at aggregate level.

## Methodology
1. Reviewed the dataset structure and key recruitment fields.
2. Built a sourcing funnel from sourced to hired.
3. Calculated conversion by source channel, recruiter, seniority, role, department, and work mode.
4. Compared average candidate signals for hired vs. non-hired candidates.
5. Categorized rejection/drop-off reasons.
6. Used AI to create a recruiter-note taxonomy and convert qualitative notes into consistent signal categories.

## Key Funnel Finding
The strongest bottleneck appears between **Test Taken** and **Offer Sent**. 201 candidates took the test, but only 62 received an offer, a test-to-offer conversion of 30.8%.

## Key Insights
1. **GitHub, Inbound, and Hunting showed the strongest hired rates.** GitHub led with 11.0%, followed by Inbound at 10.1% and Hunting at 9.3%.
2. **Senior and Staff candidates converted better than Junior candidates.** Staff profiles had a 13.3% hired rate, while Junior profiles had 4.6%.
3. **Hired candidates showed stronger average technical, behavior, and manager scores.** Technical score averaged 82.4 for hired candidates vs. 72.9 for non-hired candidates.
4. **No response was the most common rejection/drop-off reason.** It represented 210 records, making engagement a clear process risk.
5. **Recruiter performance varies, but should be interpreted carefully.** Bruno and Ana showed the strongest hired rates, but differences may also reflect role mix, candidate quality, channel strategy, and follow-up practices.

## AI Usage
AI was used to support the qualitative part of the analysis by creating a consistent taxonomy for recruiter notes. The taxonomy grouped unstructured notes into practical categories such as **Salary risk**, **Low engagement**, **Follow-up/timing risk**, **Strong technical fit**, and **Potential**. A reproducible tagging function was included in the notebook so the analysis can be reviewed and repeated without exposing candidate-level personal information.

## Practical Recommendations for Recruiters
- Prioritize high-converting channels such as GitHub, Inbound, and Hunting for similar roles.
- Review the test-to-offer stage to understand whether candidates are failing the assessment, dropping due to timing, or being filtered by compensation/fit issues.
- Persist with candidates who show strong technical and manager scores, reach the test stage, and have timing-related concerns rather than capability gaps.
- Deprioritize candidates with repeated no-response patterns, low engagement, or clear salary mismatch unless the role has flexibility.
- Compare follow-up and qualification practices from stronger-performing recruiter funnels to identify replicable behaviors.

## Recruiter Action Framework

The analysis supports a four-category recruiter action model:

| Category | Candidate Pattern | Recommended Action |
|---|---|---|
| High Priority | Strong scores, good engagement, advanced funnel progress | Prioritize follow-up and keep process moving |
| Nurture | Strong potential but timing or availability issue | Keep warm for future opportunities |
| Risk / Validate Early | Salary concern, unclear motivation, mixed signals | Clarify risk before investing more time |
| Low Probability | No response, failed assessment, low fit, repeated low engagement | Deprioritize unless new information appears |

## Limitations
- This is a fictional dataset, so recommendations should be interpreted as analytical patterns rather than definitive business rules.
- Candidate names and emails were not analyzed because the project focuses on process-level decisions.
- Recruiter conversion should not be interpreted as individual performance without controlling for role difficulty, candidate pool, requisition urgency, and hiring manager behavior.
