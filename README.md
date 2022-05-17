# GIRFT_DataQuality
Assessment of the data quality from the national Hospital Episode Statistics healthcare dataset.

## Background
Large administrative healthcare datasets are a valuable source of information that can help inform clinical and operational decision making to improve outcomes for patients. However, to gain maximum insight, it is important to understand their strengths and weaknesses. We aimed to identify inconsistencies in the recording of mandatory International Statistical Classification of Diseases and Related Health Problems, tenth revision (ICD-10) codes within the Hospital Episodes Statistics (HES) dataset in England. 

## Methods
Three exemplar medical conditions were chosen: autism, type II diabetes mellitus and Parkinson’s disease dementia. Recording of all three are mandatory and once diagnosed should appear in the record of every subsequent hospital admission. We identified the first occurrence of the condition ICD-10 code for a patient during the period April 2013 to March 2021 and then looked for the code in subsequent hospital spells. We designed and trained random forest classifiers to identify variables strongly associated with inconsistencies in recording of these conditions.

## Results
For autism, type II diabetes and Parkinson's disease dementia respectively, 43.7%, 8.6% and 31.2% of subsequent spells did not have a relevant code recorded for the condition. Coding inconsistencies were highly correlated with non-coding of an underlying condition, a change in hospital trust and the time difference between the spell with the first coded diagnosis and the subsequent spell. For patients with diabetes or Parkinson’s disease dementia, the code recording for spells without an overnight stay were found to have a higher rate of inconsistencies.

## Conclusions
Data inconsistencies are relatively common for the three conditions considered. Where these mandatory diagnoses are not recorded there is potential for this to impact on the care provided.
