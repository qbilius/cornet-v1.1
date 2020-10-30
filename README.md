# CORnet v1.1

CORnet v1.1 wrapped for Brain-Score testing.

This is a fully recurrent version of [CORnet-S](https://github.com/dicarlolab/cornet), meaning that each layer is now recurrent such that data is processed at each layer at each time step. In contrast, in CORnet-S data is processed at a single layer at each time step; once the data is processed for several time steps in a given layer, it is passed to the next layer, while the previous layer sits idle.


# Scoring results

| Benchmark                 | Score | CORnet-S score  |
|---------------------------|-------|-----------------|
| FreemanZiemba2013.V1-pls  | 0.249 | .294            |
| FreemanZiemba2013.V2-pls  | 0.304 | .242            |
| MajajHong2015.V4-pls      | 0.567 | .58             |
| MajajHong2015.IT-pls      | 0.511 | .54             |
| Rajalingham2018-i2n       | 0.338 | .55             |
| Kar2019-ost               | N/A   | .305            |

Notes:

- The model has not been prepared for testing on `Kar2019-ost` so the score is unknown.
- The score on `Rajalingham2018-i2n` is suspiciously low. I'm pretty sure it's incorrect.
- Other scores match my expectations. The model was not developed sufficiently to reach the level of CORnet-S but should be very close.


# Current Status

I am not actively developing this model and have no plans to do so. Feel free to use this model for your needs.