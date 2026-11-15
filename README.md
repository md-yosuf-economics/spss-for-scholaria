# AI use, academic productivity and performance: SPSS practice data (n = 999)

Synthetic practice data for the book *SPSS for Scholaria* (YS Scholaria, Md. Yosuf). Every record is synthetic and does not describe a real person.

## Files

- `AI_Productivity_Synthetic_999.xlsx`
  - `Synthetic_Data`: coded data, one row per respondent, with numeric codes.
  - `Raw_Data`: the same answers written in words, for practice in coding and multiple-response preparation.
  - `SPSS_Codebook`: variable names, labels, codes, measurement levels, and whether each variable is in this file.
  - `SPSS_Analysis_Map`: the suggested SPSS procedure for each analysis.
- `AI_Productivity_Synthetic_999.sav`: the coded data as an SPSS data file, with variable labels and value labels.
- `AI_Productivity_Project_Questionnaire_YS_Scholaria.docx`: the questionnaire and project framework.

## Notes

- The file holds 999 respondents (AIAP20260001 to AIAP20260999) and 50 variables. The survival fields (F7, event, time_to_completion_days) are not included; Section 17.2 of the book shows how to derive them.
- `Raw_Data` is decoded from the coded data with the codebook labels. It is not an original form export. The nine B4 activity columns are combined into `B4_activities`, as respondents selected them. `None selected` means that no activity was chosen.
- For 30 respondents the stored `productivity` score does not match the mean of their answered items, and for 29 the stored `responsible_ai` score does not match. All of these respondents have missing items. Recompute the scores as described in Section 6.5 of the book.
- In the `.sav` file, `participant_code` is the last variable.

## Opening the data in SPSS

- `.sav`: File > Open > Data, then choose the file.
- Excel: File > Open > Data, choose Excel, tick "Read variable names from the first row of data", and select the sheet `Synthetic_Data` or `Raw_Data`.
