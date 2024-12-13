# Pupil Diameter and Emotion Analysis

This repository contains the analysis of the relationship between pupil diameter and emotions, focusing on the effects of emotional stimuli (Happy, Angry, Neutral) on reaction time and pupil diameter. The study comprises two experiments: the Main experiment (emotion detection) and the Control experiment (spatial detection).

## Problem Statement
The objective of this study is to explore how pupil diameter and reaction time vary with emotional stimuli. Specifically, the analysis aims to:
- Examine pupil diameter trends over time.
- Understand reaction time variations for different emotions.

## Dataset
The dataset contains CSV files for two experiments (Main and Control) and includes the following:
- **Stimulus Name**: Identifier for the presented stimulus.
- **Reaction Time**: Time taken by participants to respond.
- **Reaction Key**: Response type.
- **Pupil Diameter**: Time-series data starting from column 4 onwards.

### Preprocessing
- Removed irrelevant columns (e.g., `Stimulus Name`, `t1-t86` for fixation periods).
- Handled missing values (`NULL`) in pupil diameter data.
- Created a cleaned CSV file (`new.csv`) for analysis.

## Data Analysis
### Reaction Time
- Median reaction times were calculated for robustness against outliers.
- Reaction times varied significantly across emotions in the Main experiment:
  - Happy: Shortest reaction time.
  - Angry: Longest reaction time.
  - Neutral: Intermediate reaction time.
- Control experiment showed consistent reaction times across stimuli.

### Pupil Diameter
- Aggregated average pupil diameter values while ignoring rows with `NULL` values.
- Significant trends observed:
  - Pupil constriction around 1450 ms, followed by dilation, forming a "V" shape.
  - Main experiment showed greater variability compared to the Control.

### Supporting Analysis
- Rate of change of pupil diameter indicated sharp constrictions and adjustments due to cognitive load.

## Key Findings
- Emotional stimuli (especially Angry) caused greater pupil constriction and longer reaction times, indicating heightened cognitive and physiological demand.
- Control tasks exhibited stable reaction times and minimal pupil variation, reflecting lower cognitive load.

## Conclusion
Emotional recognition tasks are more cognitively and physiologically demanding than simple visual tasks. Negative emotions, such as anger, amplify these effects, with increased reaction times and significant pupil constrictions.

## References
1. O'Sullivan, T., & Ibbotson, P. (2008). Matplotlib for Python Developers. [Documentation](https://matplotlib.org/stable/contents.html)
2. Pandas API Documentation: [Pandas API](https://pandas.pydata.org/docs/reference/index.html#api)
3. Henderson, R. R., Bradley, M. M., & Lang, P. J. (2018). Emotional imagery and pupil diameter. [Psychophysiology](https://doi.org/10.1111/psyp.13050)

---

Feel free to explore the repository for the code, data, and detailed analysis reports!
