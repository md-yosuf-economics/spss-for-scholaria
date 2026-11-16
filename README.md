# AI use, academic productivity and performance: SPSS practice data (n = 999)

Synthetic practice data for the book *SPSS for Scholaria* (YS Scholaria, Md. Yosuf). Every record is synthetic and describes no real person.

## Files

- `AI_Productivity_Synthetic_999.xlsx`
  - `Synthetic_Data`: coded data, one row per respondent (59 variables). Unknown answers are coded 99.
  - `Raw_Data`: the answers in words, as collected (43 columns). Blanks mean no answer.
  - `SPSS_Codebook`: variable labels, codes, measurement levels, the 99 rule and each derivation.
  - `SPSS_Analysis_Map`: the SPSS procedure for each analysis.
- `AI_Productivity_Synthetic_999.sav`: the coded data as an SPSS data file, with variable labels, value labels, and 99 declared as a user-missing value where it means unknown.
- `AI_Productivity_Project_Questionnaire_YS_Scholaria.docx`: the questionnaire and project framework, including item F9.

## Notes

- The file holds 999 respondents (AIAP20260001 to AIAP20260999). Unknown answers are coded 99 and declared missing in the `.sav` file. F1, F2 and F9 contain real answers of 99 minutes, so 99 is not declared missing for those variables.
- The survival fields are included: `F6_completion_days`, `F7_under_observation_end`, `event` and `time_to_completion_days`. Cases with `event` = 99 (completed, date missing; 140 cases) are excluded from survival analysis, which leaves 859 cases.
- Derived variables: `ai_group` (1 non-user, 2 low or moderate user, 3 frequent user); the contrasts `ai_group_user` and `ai_group_frequent` (non-users are the reference group); `study_hours_band`; and `performance_high`.
- `Raw_Data` is decoded from the coded data with the codebook labels, so it is not an original form export. The nine B4 activity options are combined into `B4_activities`, and `None selected` means no activity was chosen.
- Known inconsistencies are kept for practice: 70 respondents answered No to AI use but Rarely to frequency, and 52 AI users answered Never. The stored `productivity` (30 respondents) and `responsible_ai` (29 respondents) scores differ from the mean of the answered items; all of these respondents have missing items. Recompute the scores as described in Section 6.5 of the book.
- In the `.sav` file, `participant_code` is the last variable.

## Opening the data in SPSS

- `.sav`: File > Open > Data, then choose the file.
- Excel: File > Open > Data, choose Excel, tick "Read variable names from the first row of data", and select `Synthetic_Data` or `Raw_Data`.
