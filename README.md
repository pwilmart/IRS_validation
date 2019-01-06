# IRS_validation

## Phil Wilmarth
### January 6, 2019

This repository looks at some data from a 77-channel TMT experiment. It was done in **seven** TMT experiments (plexes) using 11-plex TMT reagents. There were two pooled reference channels used in each plex so that Internal Reference Scaling (**IRS**) could be done to combine the data.

Three of the plexes had an a third reference channel and those extra channels can be used to test and validate the IRS method. There are two notebooks present. One notebook (auto_finder_BIND-473.ipynb) double checks which channels in each plex are the reference channels. The other notebook (IRS_validation.ipynb) does the testing and validation.
