---
description: Basic information about CypherBabel Index products.
---

# CBI Indices

{% hint style="info" %}
CAUTION

This is a living document and is susceptible to changes.
{% endhint %}

## Introduction

As a financial data service provider, CBI is the core and "genesis block" of CypherBabel. Besides official indices products, CBI offers a DApp for users to build their own crypto assets indices. Valuing the spirit of blockchain and Web3.0, CBI provides tools to give the power of creating financial products back to each participant in Web3.0. CBI encapsulates a set of complex index calculation methodologies so that the users only need to decide the constituents of their indices based on their understanding of the market. CBI expects an increasing number of professional users to participate in the CBI DAO to improve and diversify the index methodologies and tools and build more effective indices for all Web3.0 users. Investors in the CBI community pay attention to CBI indices and make investments accordingly. The best performance index will be favored the most in the community as a sign of the community's involvement.

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

* **Monthly** time window resolution: `2022-10-01` : Includes data from`2022-10-01 00:00 UTC` to `2022-10-31 23:59 UTC` (i.e. Oct 2022).
* **Daily** time window resolution: `2022-10-01` : Includes data from`2022-10-01 00:00 UTC` to `2022-10-01 23:59 UTC`
* **Hourly** resolution: `2022-10-01 08:00 UTC` : Includes data from`2022-10-01 08:00 UTC` to `2022-10-01 08:59 UTC`
