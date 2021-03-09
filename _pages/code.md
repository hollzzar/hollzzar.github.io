---
layout: archive
permalink: /code/
title: "Code"
author_profile: true
---

## From EEG to ERP: My processing pipeline with MATLAB and R

[My lab](https://sites.psu.edu/bildlab/) uses a combined NeuroScan and Brain Vision system with 31 active Ag/AgCl electrodes and two bipolar channels. I developed the processing pipeline presented here for my first EEG/ERP experiment on dialectal variation in syntax (double modal [DM] versus single modal [SM] constructions) in two groups of participants (Unmarked [MAE] and Southern [SUSE]).

1. I pre-processed the CNT files for each participant with [this MATLAB script](https://github.com/hollzzar/eeg-data-scripts/blob/master/DM_process.m). After a reviewer asked about adaptation effects during the experiment, I pre-processed again in the first and second halves of the experiment separately with [this MATLAB script](https://github.com/hollzzar/eeg-data-scripts/blob/master/DM_process_half.m).
2. I used [this MATLAB script](https://github.com/hollzzar/eeg-data-scripts/blob/master/DM_analysis.m) to calculate average ERPs in each time window (2) for each subject, both for the main analysis and first/second half analysis, and calculate grand averages for plotting. The script exports the processed data as TXT files for use in R.