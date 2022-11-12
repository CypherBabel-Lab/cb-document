---
description: Basic information about CypherBabel Index products.
---

# CBI Indices

## Resolutions and Timestamps

### Time Window Resolutions

CBI indices' time windows are available in the following resolutions:

* **All**
* **1 year** (1Y)
* **1 month** (1M)
* **1 week** (1W)
* **1 day** (1D)
* **1 hour** (1H)

Time window resolution means the **time window** over which a metric is being aggregated.

### Data Point Resolutions

CBI indices' data points are available in the following resolutions:

* **1 day** (for "All" and "1 year" time windows)
* **2 hours** (for "1 month" time window)
* **30 minutes** (for "1 week" time window)
* **5 minutes** (for "1 day" time window)
* **1 minute** (for "1 hour" time window)

Data point resolution means the **frequency** at which the data is being updated.

For instance, the CIC55 on a 1D time window resolution shows the index level over 24 hours with a data point resolution of 5 minutes. The same mechanism is applied analogously to all other resolutions.

## Timestamps

All metric timestamps are in UTC and always refer to the start of an interval.

For examples:

* **Monthly** time window resolution: `2022-10-01` : Includes data from`2022-10-01 00:00 UTC` to `2022-10-31 23:59 UTC` (i.e. Oct 2022)
* **Weekly** time window resolution: `2022-10-10` : Includes data from `2022-10-10 00:00 UTC` to `2019-05-19 23:59 UTC` (i.e. Week 20)
* **Daily** resolution: `2019-05-13`--> Includes data from`2019-05-13 00:00 UTC` to `2019-05-13 23:59 UTC`
* **Hourly** resolution: `2019-05-13 10:00 UTC` --> Includes data from`2019-05-13 10:00 UTC` to `2019-05-13 10:59 UTC`
* **10 Min** resolution: `2019-05-13 10:20 UTC` --> Includes data from `2019-05-13 10:20 UTC` to `2019-05-13 10:29 UTC`
