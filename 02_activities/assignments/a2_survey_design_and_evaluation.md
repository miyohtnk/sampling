# Assignment: Questionnaire Design and Sample Evaluation

## Requirements

The goal of this assignment is to practice developing and evaluating sampling materials.

### Part A - Survey Design:

Select one of the scenarios below and design a survey to meet the need(s) outlined in the prompt.

1.	In two to three sentences, describe the purpose of your survey
2.	Describe your target population, sampling frame, sampling units, and overall sampling strategy.
3.	Write a 5-10 question survey to address your chosen scenario below.

##### Scenarios
1.	You work in the Human Resources Department at a large tech company. Over the past few months, the company has been experiencing a high turnover rate across many of its departments, specifically within the entry- and lower-level positions. The company wishes to understand why this turnover is happening, and what changes need to occur to improve employee satisfaction.
2.	You work for a Canadian national political party during a federal election. Throughout the campaign period, your party has seen relatively high approval ratings, but an opposing party is also polling favorably and may still have a chance to win the election. You are one month away from the election and you want to understand what voters want from your party and its leader in order to maintain your lead and eventually win the election.
3.	You are a student researcher in the sociology department at the University of Toronto. You are working on a research project that concerns the relationship between music taste and age. This involves both comparisons between different people of different ages and comparisons of the same individual at different ages during their lifetime. You wish to understand to what extent age influences music taste, specifically as it relates to perceptions of popular music. Your results will be written into an academic paper that you hope to publish.

### Part B - Survey Evaluation:

For the **Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33)**, conducted by Statistics Canada find any and all available documentation for the data gathered and identify and describe the survey features indicated below.

1. Sample type
2. Sample size
3. Target population
4. Sampling frame
5. Survey mode(s) 
6. Timeline
7. Response rate
8. Weights
9. Data processing
10. Cleaning, imputation, etc
11. Sources of error
12. Limitations, known biases, etc
13. Link to documentation and any additional sources used


# Your Changes

## Part A - Survey Design: 

The number of your chosen topic: `#3`

Describe the purpose of your survey:
```
The survey aims to understand the relationship between music taste, age, and how it changes through time. With this survey, we hope to elucidate the extent of influence that age places on music preference, specifically as it relates to perceptions of popular music.
```

Describe your target population, sampling frame, sampling units, and observational units:
```
Our target population is men, women and non-binary folks from ages 18-70 living in the Toronto municipality.

Our sampling frame people in Toronto that are registered to vote (for example for the April 28th elections) as well as people with address and postal code information from Canada Post.

Our sampling units are neighborhoods. Since the population of Toronto is about 3 million, we will stratify the people based on neighborhood and use purposive sampling (non-probability sampling) to find 20 people from each age (52 x 20 = 1,040 people)

Our observational units are people in our age of interest.
```

Your 5-10 question survey:
```
1. In what year were you born? (input year)
2. How often do you listen to music? (Never, Rarely, Weekly, Daily)
3. If YES, how often do you currently listen to the following music genres: Pop, Rock, Metal, Jazz, Hip-Hop, Rap, R&B, Electronic/Dance, Soul, Classical, Folk, Blues, Indie, Country, Other(input music type)- (Never, Rarely, Sometimes, Often, Always)
4. Do you feel like you listen to the same music as your peers? (Yes/No),If no, why not? (Open-ended)
5. Do you like finding new artists in different music genres than what you normally listen to? (Yes/No)
6. What motivates you to explore new genres? (Friends, Curiosity, Peer pressure, Internet algorithms)
7. Do you think that your music taste has changed over the years? (Yes/No)
8. If YES, compared to 5-10 years ago, how has your music taste changed? (No change, Slightly different, Somewhat different, Very different)
9. If YES, what other music genres did you use to listen to? (Yes/No answers for every genre)
Pop, Rock, Metal, Jazz, Hip-Hop, Rap, R&B, Electronic/Dance, Soul, Classical, Folk, Blues, Indie, Country, Other(input music type)
10. If YES, how often would you say your music taste changed? (Never, Rarely, Sometimes, Often, Always)
11. Do you believe that your music taste follows what is currently popular? Why or why not? (Open-ended)
```

## Part B - Survey Evaluation:

Identify and describe survey features:

```
1. Sample type: Stratified random sampling (probablity sampling). Stratification happened at the province/census metropolitan area level, and information was collected from one randomly selected household member aged 15 or older. 27 strata were created in total. Proxy responses were not permitted. Rejective sampling was also used.

2. Sample size: 40,000 invitation letters were sent and 24,000 questionnaires were expected to be completed.

3. Target population: All Canadians and permanent residents 15 years of age or older that live in the 10 Canadian provinces

4. Sampling frame: households with telephone numbers that were part of the Census and other known sources with Statistics Canada's dwelling frame and that responded to the survey. (record number is 4430)

5. Survey mode(s) :Phone calls (both landline and cellular) from the Census and other sources with Statistics Canada's dwelling frame.

6. Timeline: Data collection period- 2018-09-04 to 2018-12-28., collection period is every 5 years from September to December.

7. Response rate: 41.9%

8. Weights: A weighting factor was created because each person represented 50 persons in the population. In addition, bootstrap weights were created for design-based variance estimation. Estimates based on the survey data were also adjusted by weights so that they are representative of the target population with regard to certain characteristics.

9. Data processing: Data was collected from survey respondents through an electronic questionnaire or through a computer assisted telephone inteviewing (either French or English), and this information was linked to the personal tax records (T1, T1FF, T4) of the respondents and the tax records of the household members. Key variables included: household information such as address, postal code and telephone number, respondent's information such as social insurance number, surname, name, data of birth, age and sex, and household members' information such as surname, name, age, sex and relationship to respondent. Use of SSPE set of generalized processing steps, with a structured environment to monitor the processing fo data. Edits were performed- family relationships (for integrity of matrix data), consistency of survey data (eg. respondent date against their birth date) and flow edits (to ensure correct path taken and fix off-path situations). Errors were detected and fixed.

10. Cleaning, imputation, etc: The CATI system was used to "clean" up the data by editing the flow of the questionnaire and editing out of range values. In addition, with data linkage, better quality data was hoped to be obtained. Imputations were carried out in nine steps using donor records (donors were the cases from where the information could be copied and imputed into another case) selected through a score function. Characteristics on each record with item or partial non-response were compared with the characteristics on all the donor records, and when the donor score was highest, it was chosen to fill the missing information of the non-respondent. When donor imputation could not be used, mean imputation was used.
Some data was also linked because income data was not available for the 2018 cases. Validation measures were also implemented, and included: analysis of changes over time, verification of estimates through cross-tabulations and confrontation with other similar sources of data.

11. Sources of error: Human processing  and response error, sampling and non-sampling errors. Sampling error: estimates based on a sample will vary from sample to sample and typically they will be different from the results that would have been obtained from a complete census. For the non-sampling error, we had non-response at the household and individual level and imperfect coverage. Households without telephones and those with telephone services not covered by the frame were excluded, thus bias is introduced.

12. Limitations, known biases, etc: Due to the type of sampling method, sampling error is possible, as well as exclusion of cases where telephones were not available. non-response bias, in particular for 2018 was noted. Questions regarding income showed a high non-response rate perhaps due to the sensitivity of the question. Another limitation was the fact that the survey was a bit long, at 44 minutes.

13. Link to documentation and any additional sources used: https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&Id=796234
```

## Rubric

-	All required components are present and complete **Complete / Incomplete**
-	Choice of sampling strategy for Part A is justified and related to survey purpose **Complete / Incomplete**
-	Information for Part B is complete and correct **Complete / Incomplete**

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 18/04/2025`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (a2_survey_design_and_evaluation.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-2`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via the help channel in Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
