**🔹 Data Cleaning and Analysis**
This project involved a structured approach to data cleaning and analysis, using both SQL and Python to ensure the dataset was reliable and ready for insight generation.

**Initial steps included:**

Handling missing values and ensuring consistency in date formats

Validating data types and identifying duplicate or irrelevant records

Using Pandas for efficient manipulation in Python, and SQL window functions to detect potential duplicate transactions to showcase skillset.

An example of this approach is included in the project/notebook.

During review, inconsistencies were identified in the Price Per Unit field, particularly due to unclear currency context. To explore this, I ran a deeper investigation on Solana, comparing its highest and median prices. The findings raised questions about data validity, especially around value-related fields, and highlighted the importance of understanding currency reference points in transaction data.

While proceeding with the assumption that the dataset reflected intended values, this scenario demonstrates the importance of validation - ideally through internal data documentation or trusted sources like CoinGecko or CoinMarketCap for a guide.

**🔹 Key Insights and Recommendations**
1. **Low Completion Rate Across Transactions**

Only 33.22% of transactions were marked as completed, with the rest nearly evenly split between failed and pending.

**Recommendation:** Investigate root causes of transaction failures — e.g. wallet compatibility, network latency, or platform-specific issues. Improving success rate could have a direct impact on retention and trust.

2. **Higher fees on hardware wallets**

Average fees for Trezor and Ledger exceeded $38K per transaction, compared to lower fees on hot and exchange wallets.

**Recommendation:** Consider introducing fee transparency tools or caps for hardware wallet users, or reward systems to offset friction while preserving security benefits.

**3. High-value transactions clustered around key cryptos**

Bitcoin, Cardano, BNB, and Ethereum had the highest average transaction values — suggesting institutional or high-net-worth engagement.

**Recommendation:** Explore tailored services for these user segments (e.g. faster processing, custom support, lower fees) to retain high-value users.

**4. Coinbase, KuCoin, and Huobi lead in platform volume**

These three platforms dominate transaction volume (all transactions), collectively representing a major share of user activity. Kraken is 3rd when it is completed transaction.

**Recommendation:** Prioritise partnerships and integrations with these platforms. Consider co-branded user journeys or promotional campaigns to deepen engagement.

**5. Clarity needed on value fields**

The lack of defined currency context for pricing fields affects data interpretation and undermines trust in value-based metrics.

**Recommendation:** Ensure critical financial fields (like price per unit price and total value) are clearly defined in future datasets, ideally with standardised currency formats or metadata documentation on confluence.

**✅ Final thoughts**
This project aimed to highlight how data quality, platform strategy, and user experience intersect in crypto transaction analysis from 10,000 rows of data. Future improvements could include:

Validating external price data sources
Conducting user journey analysis

**✏️ Note for reviewers**
Feel free to explore the accompanying Python scripts and Tableau dashboards included in the repo. The dashboard tab is called Top Line Overview Dashboard and it has filters that should change the relevant visuals.
