# Project 1: SAT & ACT Analysis - README.md
#### James Proctor, General Assembly DSI-9-ATL
#### September 20, 2019

## Problem Statement

**What can be learned from ACT & SAT 2017/2018 testing data, and how can we use that information to improve SAT Participation rates?**

## Executive Summary

Through the course of this project, we executed and documented the process of obtaining text-based data, cleaning and organizing in our Python Pandas DataFrames, and plotting data to extract meaningful insights.

Data is displayed both in queried tabular form as well as in Histograms, Scatter Plots, and Box Plots from Python's Seaborn/Matplotlib visualization libraries. Through the use of these displays, assembled with custom-built functions, we identified a strong growth opportunity for the College Board in the state of New Mexico.

## Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|Final|The state in which ACT test data was collected during 2017|
|**act_participation_2017**|*float*|ACT 2017|Percentage of test takers in the state that took ACT during 2017|
|**act_english_2017**|*float*|ACT 2017|Mean score for ACT English tests taken in state during 2017|
|**act_math_2017**|*float*|ACT 2017|Mean score for ACT Math tests taken in state during 2017|
|**act_reading_2017**|*float*|ACT 2017|Mean score for ACT Reading tests taken in state during 2017|
|**act_science_2017**|*float*|ACT 2017|Mean score for ACT Science tests taken in state during 2017|
|**act_composite_2017**|*float*|ACT 2017|Mean composite score for ACT English, Math, Reading, and Science tests taken in state during 2017|
|**sat_participation_2017**|*float*|SAT 2017|Percentage of test takers in the state that took SAT during 2017|
|**sat_erw_2017**|*integer*|SAT 2017|Mean score for SAT Evidence-Based Reading & Writing (ERW) tests taken in state during 2017|
|**sat_math_2017**|*integer*|SAT 2017|Mean score for SAT Math tests taken in state during 2017|
|**sat_total_2017**|*integer*|SAT 2017|Mean composite score for SAT ERW and Math tests taken in state during 2017|
|**act_participation_2018**|*float*|ACT 2018|Percentage of test takers in the state that took ACT during 2018|
|**act_composite_2018**|*float*|ACT 2018|Mean composite score for ACT English, Math, Reading, and Science tests taken in state during 2018|
|**sat_participation_2018**|*float*|SAT 2018|Percentage of test takers in the state that took SAT during 2018|
|**sat_erw_2018**|*integer*|SAT 2018|Mean score for SAT Evidence-Based Reading & Writing (ERW) tests taken in state during 2018|
|**sat_math_2018**|*integer*|SAT 2018|Mean score for SAT Math tests taken in state during 2017|
|**sat_total_2018**|*integer*|SAT 2018|Mean composite score for SAT ERW and Math tests taken in state during 2018|

## Conclusions & Recommendations

In reviewing ACT and SAT participation data from 2017 and 2018, as well as the status of applicable state laws regarding testing subsidies and requirements, we recommend that the College Board prioritize its marketing and lobbying efforts in **New Mexico**.

The College Board should seize the opportunity to invest its marketing and lobbying efforts in New Mexico based on both statistical and environmental factors.  

*Geography*

New Mexico resides in a balanced location in the Southwest US, nestled against the ACT stronghold of the Midwest but adjacent to Texas, which experienced an increase in SAT participation from 62% in 2017 to 66% in 2018. 

It also shares its Northern border with Colorado, which recently passed legislation making the SAT a mandatory as well as a subsidized exam for college-bound students.  This increasing presence of the SAT in the regional culture around New Mexico increases the likelihood that marketing and lobbying efforts will be effective.

*Participation Growth Potential*

New Mexico saw an increase from just 11% SAT participation in 2017 to 16% in 2018, which represents almost 50% growth in a year, yet still leaves major room for growth.  This contrasts with an ACT participation rate that increased slightly from 66% to 67% over the same year, but is relatively low considering how common 100% participation for ACT is in the region.  

*Strategy*

The College Board should undertake the following strategies within the state of New Mexico:

**1. Engage with State and Local Governments**

The SAT can be offered for free or discounted to students at both the state level and the municipal - even if a state doesn't provide for all, individual school districts are able to offer free SAT admission for local citizens.  Currently, none of these programs exist at the state level in New Mexico, and a more compelling case can be made in its favor.

**2. Invest in Marketing Efforts**

New Mexico is a state where students have the freedom to choose the college exam they prefer, or to skip it altogether.  With this, there is a contingent of potential customers still untapped by the ACT exam that may be reached by effective communication.

**3. Leverage Neighbors' Successes**

Lobbying and marketing efforts should make use of trends in Texas and Colorado, where SAT participation rates are increasing significantly.  This momentum can be harnessed to increase SAT participation rates across the wider Southwest.

## Data Sources

2017 SAT Data: https://blog.collegevine.com/here-are-the-average-sat-scores-by-state/
2017 ACT Data: https://blog.prepscholar.com/act-scores-by-state-averages-highs-and-lows
2018 SAT State-by-State: https://reports.collegeboard.org/sat-suite-program-results/state-results
2018 ACT State-by-State: http://www.act.org/content/dam/act/unsecured/documents/cccr2018/Average-Scores-by-State.pdf
States Providing ACT for Free: https://magoosh.com/hs/act/2017/states-provide-act-free/
States Providing SAT for Free: https://magoosh.com/hs/sat/2017/states-provide-sat-free/
States Requiring ACT/SAT/Either: https://magoosh.com/hs/act/2017/states-that-require-the-act-or-sat/