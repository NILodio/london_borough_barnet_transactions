## Executive Summary

In response to a simulated request from an auditor, we reviewed corporate credit card transactions for the London borough of Barnet for the period 2014-2016. We performed several kinds of analysis: summary, trend analysis, classification review, clustering, and anomaly identification. Data quality was reasonble, so we were able to fulfill all of the analysis requests. The rest of this report will review the analysis in detail. The analysis requests and key findings are summarized below.

#### Analysis Requests
1. The Auditor would like to get a summary view of the transactions for each Service Area. The summary view would include at least one visual representation of the transactions in such a way that they could compare them by quarter. Quarters are defined based on the calendar year (Q1 is January to March, Q2 April to June, etc.). The Auditor would also like a summary table with some relevant statistics (The Auditor says something along the lines of “transaction counts and averages”, but welcomes ideas).

2. The Auditor would like to get a view if there are any significant changes in spending behavior by Service Area and by Account. Changes in behavior could be spikes, but could also be permanent increases in the transaction amounts. Please identify instances of both or show that they do not exist in the data. 

3. The Auditor would like to get an understanding of how Creditors are classified into accounts. In particular, they are worried about transaction misclassification. Are you able to identify instances in which Creditors are not consistently classified into Accounts (e.g., most of the time Creditor “AirTickets.com” is classified into “Travelling Expenses”, but on some occasions it is also found in “Miscellaneous”)?

4.	In terms of spending behavior (defined by the number and the typical size of transactions), are there Service Areas that behave similarly and can be grouped together? How?

5.	The auditor has heard that you may know anomaly detection techniques. They would like to ask you for a sample of a few hundred transactions that are anomalous, different or worthwhile inquiring about.  The sample should include at least five transactions for each Service Area. Please provide this sample and explain why they are special or different.

#### Key Findings
* 76% of creditors are classified consistently, but 24% are classified inconsistently.
* 18 spikes occurred in quarterly spending by the 15 service areas, as well as 53 such spikes for the 67 accounts.
* 13 permanent increases occurred in quarterly spending by service area, as well as 25 such increases by account.
* Service areas cluster naturally into four groups, on the basis of transaction count and average transaction amount.
* Approximately 400 or 4.5% of transactions are anomalous for high transaction amounts (above the 98th percentile for their service areas)
* Approximately 140 or 1.6% of transactions are anomalous as one-time charges to an account within a given service area (which might represent misconduct or misclassification)