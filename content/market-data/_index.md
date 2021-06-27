---
weight: 10
bookFlatSection: true
title: Market Data
summary: Open brokerage accounts, enable commission-free trading, and manage the ongoing user experience with Alpaca Broker API
---

# Market Data

Access Alpaca's historical and real-time US stock market data through REST API and WebSocket.

## Data sources

Alpaca provides market data from two data sources:

**1. IEX (Investors Exchange LLC) which accounts for ~2.5% market volume**

* IEX is optimal to start testing out your app and utilize it where visualizing accurate price information may not take precedence.

**2. All US exchanges which account for 100% market volume**

* This Alpaca data feed is coming as direct feed from exchanges consolidated by the Securities Information Processors (SIPs). These link the U.S. markets by processing and consolidating all bid/ask quotes and trades from every trading venue into a single, easily consumed data feed.


* We provide ultra low latency and high reliability as the data comes directly into Alpaca's bare metal servers located in New Jersey sitting next to most of the market participants. 


* SIP data is great for creating your trading app where accurate price information is essential for traders and internal use. 


## Sandbox access

You can access the IEX market data with your Broker API key. This is free of charge and you can redistribute it to your end user without any additional agreement.

### Base URL

`https://data.sandbox.alpaca.markets/v2`

### URL

`wss://stream.data.sandbox.alpaca.markets/v2/{source}`

Where source is `iex` or `sip`.

To enable market data on a production environment please reach out to our sales team.

Accessing Alpaca's SIP data requires additional agreements and entails charges with corresponding exchanges. If you need this integration, please contact us.

Explore our [historical](https://alpaca.markets/docs/broker/docs/market-data/historical/) and [real-time](https://alpaca.markets/docs/broker/docs/market-data/realtime/) data APIs.