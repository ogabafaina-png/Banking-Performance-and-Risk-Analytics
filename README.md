# Banking Performance & Risk Analytics Dashboard

**Author:** Ogaba Faina Ogenyi  
**Date:** 2026-09-15

## Project Background

The banking platform is experiencing a critical increase in transaction failures, customer complaints, and concerns around financial discrepancies. Management needs to understand whether failed transactions are primarily associated with banking or network-related performance issues.

The Risk Department has also raised concerns about whether transactions identified as potentially fraudulent are actually being stopped. At the same time, management needs to assess whether investment in 5G network slicing is improving transaction performance and determine whether future application development resources should focus on Desktop or Mobile users.

This project analyzes transaction and network performance data and presents the findings through an interactive Excel dashboard to support evidence-based, board-level decision-making.

## Project Objectives

- Analyze transaction success and failure rates.
- Investigate transaction failure patterns across latency, transaction type, and network slices.
- Assess whether transactions flagged as potentially fraudulent are being successfully prevented.
- Evaluate network slice performance using latency and bandwidth.
- Compare transaction success and failure performance across Desktop and Mobile devices.
- Build an interactive Excel dashboard to support management reporting and decision-making.
- Identify areas requiring operational, network, security, or application-development attention.

## Dataset

The project dataset contains transaction-level banking records and network performance information.

The dataset includes:

- Transaction ID
- Sender Account ID
- Receiver Account ID
- Transaction Account
- Transaction Type
- Timestamp
- Transaction Status
- Fraud Flag
- Geolocation
- Device Used
- Network Slice ID
- Latency
- Slice Bandwidth
- PIN Code

**Transaction Status** identifies whether a transaction was **Success** or **Failed**, while **Fraud Flag** identifies transactions flagged as potentially suspicious or fraudulent.

Network-related fields include **Network Slice ID, Latency, and Slice Bandwidth**.

## Dashboard Features

### Key Performance Indicators

- **Total Transactions — 40,000**
- **Transaction Success Rate — 80.08%**
- **Transaction Failure Rate — 19.92%**

### Dashboard Analyses

- Transaction Failure Rate by Latency
- Transaction Failure Rate by Transaction Type
- Transaction Failure Rate by Network Slice
- Fraud Flag but NOT Blocked Rate
- Network Slice Performance — Average Latency & Average Slice Bandwidth
- Transaction Success/Failure Rate by Device

The dashboard is designed around the main business questions concerning transaction failures and network performance, fraud flagging versus transaction outcomes, network slicing performance, and Desktop versus Mobile transaction performance.

## Interactive Filters

The dashboard includes three slicers:

- Device Used
- Network Slice ID
- Transaction Type

## Key Findings

### Transaction Performance

The dataset contains **40,000 transactions**, with a transaction success rate of **80.08%** and a transaction failure rate of **19.92%**.

This provides management with a direct view of overall transaction performance and establishes the scale of failed transactions requiring further investigation.

### Transaction Failures and Network Latency

Transaction failure rate is analyzed across latency ranges to examine whether network delay is associated with transaction failures.

The dashboard uses latency ranges from **5–14 ms through 135+ ms**, allowing management to compare failure rates across different network-delay levels.

The overall transaction failure rate is **19.92%**, while individual latency groups show variation around this overall level.

This analysis helps address whether network performance may be contributing to transaction failures.

### Transaction Failures by Transaction Type

Transaction failure rate is compared across:

- Deposit
- Transfer
- Withdrawal

The failure rates are approximately:

- **Deposit — 19.96%**
- **Transfer — 19.85%**
- **Withdrawal — 19.96%**

The comparison helps determine whether transaction failures are concentrated in a particular transaction type or are relatively consistent across transaction activities.

### Transaction Failures by Network Slice

Transaction failure rate is compared across the three network slices.

The dashboard records approximately:

- **Slice 1 — 20.12%**
- **Slice 2 — 19.77%**
- **Slice 3 — 19.88%**

This analysis provides a basis for assessing whether transaction performance differs across network slices.

### Fraud Flag but NOT Blocked Rate

The dashboard separately analyzes transactions that were flagged by the fraud-detection system and their transaction outcomes.

The dataset identifies potentially suspicious transactions through the **Fraud Flag** field, while **Transaction Status** identifies whether the transaction ultimately succeeded or failed.

This analysis is designed to investigate management's concern about potentially fraudulent transactions that may have been flagged but still completed successfully.

### Network Slice Performance

Network Slice Performance is assessed using:

- **Average Latency**
- **Average Slice Bandwidth**

The dashboard records approximately:

- **Slice 1:** Average latency of **76.35 ms** and average bandwidth of **1,526.47 Mbps**
- **Slice 2:** Average latency of **77.26 ms** and average bandwidth of **1,525.41 Mbps**
- **Slice 3:** Average latency of **76.63 ms** and average bandwidth of **1,531.87 Mbps**

The overall averages are approximately **76.75 ms latency** and **1,527.91 Mbps bandwidth**.

These measures provide management with evidence for evaluating network-slice performance and the performance of the network-slicing investment.

### Device Performance

Transaction success and failure rates are compared between **Desktop** and **Mobile** devices.

The dashboard records approximately:

- **Desktop:** 19.97% failure rate and 80.03% success rate
- **Mobile:** 19.87% failure rate and 80.13% success rate

The difference between the two devices is relatively small in the available data. The comparison provides evidence for evaluating future application-development priorities alongside ongoing transaction-performance monitoring.

## Recommendations

### Transaction and Network Performance

- Monitor transaction failure rates across latency ranges to identify network conditions associated with elevated failures.
- Investigate latency-related failures alongside banking-system processes before attributing failures solely to network connectivity.
- Continue monitoring transaction failure rates by transaction type and network slice to identify emerging performance differences.

### Fraud Controls

- Review transactions that were flagged as potentially fraudulent but were still successful.
- Investigate whether fraud alerts are being converted into real-time transaction blocks where appropriate.
- Monitor the relationship between Fraud Flag and Transaction Status regularly to evaluate fraud-control effectiveness.

### Network Slicing

- Compare network slices using both latency and bandwidth rather than relying on a single network metric.
- Continue monitoring network-slice performance against intended service objectives.
- Use transaction failure performance alongside network metrics when evaluating the value of network-slicing investment.

### Application Development

- Compare Desktop and Mobile transaction performance using success and failure rates.
- Use observed performance differences, together with future transaction-performance monitoring, to guide application-development priorities.
- Avoid allocating development resources based on device volume alone; consider actual transaction performance when prioritizing improvements.

## Tools & Techniques

- **Microsoft Excel**
- **PivotTables**
- **PivotCharts**
- **Slicers**
- **Data cleaning and transformation**
- **Descriptive analytics**
- **KPI development**
- **Dashboard design and visualization**
- **Transaction performance analysis**
- **Network performance analysis**
- **Risk and fraud analysis**

## Project Files

- **Banking Performance & Risk Analytics Dashboard.xlsx** — Interactive Excel dashboard
- **Banking Performance & Risk Analytics Presentation.pptx** — Executive presentation summarizing findings and recommendations
- **README.md** — Project documentation

## How to Run / View

1. Open **Banking Performance & Risk Analytics Dashboard.xlsx** using Microsoft Excel, preferably the desktop version.
2. Enable content if prompted so that PivotTables and slicers can function correctly.
3. Use the dashboard slicers to filter the connected analyses.
4. Review the KPI indicators and charts to investigate transaction performance, network performance, fraud outcomes, and device performance.
5. Refer to the executive presentation for a summarized view of the key findings and recommendations.

## Contact

**Ogaba Faina Ogenyi**

Email: **Ogaba.faina@gmail.com**
