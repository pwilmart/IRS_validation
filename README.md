# IRS_validation

## Phil Wilmarth
### January 6, 2019
#### some additions September 22, 2019

This repository looks at some data from a 77-channel TMT experiment. It was done in **seven** TMT experiments (plexes) using 11-plex TMT reagents. There were two pooled reference channels used in each plex so that Internal Reference Scaling (**IRS**) could be done to combine the data.

Three of the plexes had an a third reference channel and those extra channels can be used to test and validate the IRS method. There are two notebooks present. One notebook [auto_finder_BIND-473.ipynb](https://pwilmart.github.io/TMT_analysis_examples/auto_finder_BIND-473.html) double checks which channels in each plex are the reference channels. The mathematical steps in IRS do not know if the channels being made identical are the correct pooled standard channels or mis-labeled channels. The pooled channels should be more similar to each other than any of the other biological samples in the TMT plex. This notebook runs an R function to find the two most similar channels in each plex. It is critical that the pooled standards in each plex are correctly identified.  

The other notebook [IRS_validation.ipynb](https://pwilmart.github.io/TMT_analysis_examples/IRS_validation.html) does the testing and validation. This compares pooled standards within single plexs to pooled standard channels between plexes. Various metric are used to show that IRS data between plexes very similar to data from within single plexes.
