# CEO-Strategic-Intelligence-Report-
Retail Chain Turnaround — 18-Month Sales Dataset Analysis  A 30-store retail chain is under financial pressure with declining performance across multiple locations. Leadership needs a clear, data-driven framework to make three irreversible decisions — store closures, product investment, and customer recovery.
🔑 Three Key Business Questions Driving This Analysis
PriorityStrategic QuestionDecision It Unlocks1Which stores are structurally failing vs. temporarily struggling?Close or save2Which products are driving real cash flow vs. draining shelf space?Push or discontinue3Which lost customers are worth the cost of winning back?Target or abandon

📊 Description of Available Data
ColumnWhat It Tells Usstore_idWhich of the 30 stores the transaction happened intransaction_dateWhen the sale occurred — enables trend and time-series analysisproduct_id / product_nameExactly what was soldcategoryProduct grouping — enables range and mix decisionsrevenueDollar value generated per transactionunits_soldVolume of items sold — separates price effect from demand effectcustomer_idWho bought — enables loyalty, retention, and win-back analysisloyalty_pointsEngagement depth — identifies committed vs. casual buyersregionGeographic grouping of stores — enables market-level decisions

5 SMART Business Questions

1. Which stores have had monthly revenue below the chain average for 9 or more of the last 12 months — and does any store in that group show at least two consecutive months of revenue growth anywhere in that window?
(a) The Question: Calculate each store's monthly revenue for the most recent 12 months. Flag every store that falls below the chain-wide monthly average in 9 or more of those months. Within that flagged group, check whether any store produced two back-to-back months of revenue increase at any point during the same period.
(b) Why it matters to the CEO: Chronic underperformance over 9 of 12 months is not a slump — it is a structural failure. However, two consecutive months of growth inside that failure window is a recovery signal that changes the closure calculus entirely. This question gives the CEO two clean lists: stores to close without further debate, and stores to place on a short-term recovery watch before the final decision is made.
(c) Columns to use: store_id, revenue, transaction_date

2. Which stores have lost more than 25% of their distinct buying customers when comparing months 1–9 to months 10–18?
(a) The Question: Count the number of unique customers who made at least one purchase per store in months 1–9. Repeat the count for months 10–18. Calculate the percentage drop per store and rank all 30 stores from largest to smallest customer loss.
(b) Why it matters to the CEO: Revenue figures can be temporarily inflated by price changes or bulk orders, masking the real picture. Customer count loss cannot be disguised. A store that has shed 25% or more of its buying base in nine months is not experiencing a revenue problem — it is experiencing a customer abandonment problem, which is significantly harder and more expensive to reverse. This is the CEO's clearest early-warning metric for stores beyond saving.
(c) Columns to use: store_id, customer_id, transaction_date

3. Which 5 products have the highest revenue-per-unit-sold AND have grown in units sold for at least 4 of the last 6 months across the majority of stores?
(a) The Question: Calculate revenue-per-unit for every product using the full 18-month dataset. Then filter to only products whose monthly units sold increased in at least 4 of the last 6 months, in at least 60% of the stores that carry them. Rank the top 5 by revenue-per-unit within that filtered group.
(b) Why it matters to the CEO: In a cash-constrained turnaround, the CEO cannot afford to promote products based on instinct or supplier pressure. These 5 products meet two non-negotiable criteria simultaneously — customers are actively choosing them more often, and each unit sold generates above-average cash. They are the chain's natural revenue engines and deserve priority shelf position, promotional spend, and guaranteed stock levels across all 30 stores immediately.
(c) Columns to use: product_id, product_name, category, revenue, units_sold, transaction_date, store_id

4. Which customers were in the top 25% of spenders in months 1–12 but made zero purchases in months 13–18 — and what was their total spend before they went silent?
(a) The Question: Rank all customers by total revenue generated in months 1–12. Isolate the top 25% of spenders. From that group, identify every customer with no transaction recorded in months 13–18. Calculate their total 12-month spend and sort the list from highest to lowest. Group them by their most frequently visited store.
(b) Why it matters to the CEO: These customers already demonstrated above-average willingness to spend at this chain. Their silence in the last 6 months is recent enough that the relationship is not dead — it is dormant. Reactivating the top 500 customers on this list through a direct loyalty offer or personalised outreach will generate faster and cheaper revenue than any new customer acquisition campaign. The CEO can attach a specific dollar figure to this win-back opportunity before spending a single rand on marketing.
(c) Columns to use: customer_id, revenue, transaction_date, store_id, loyalty_points

5. In stores flagged for potential closure, which product categories have grown their revenue share by more than 10 percentage points over the last 6 months relative to the store's total revenue?
(a) The Question: For every store already identified as a closure candidate, calculate each product category's share of total store revenue in months 13–15 versus months 16–18. Flag any category whose revenue share increased by more than 10 percentage points between those two periods within the same struggling store.
(b) Why it matters to the CEO: A store earmarked for shutdown may contain a category that customers in that location are actively gravitating toward — even as the store overall declines. This category-level signal tells the CEO one of three things: the store could be saved by stripping it down to only what is working; the growing demand in that category could be transferred to a nearby store before closure; or the store's lease could be renegotiated at a smaller footprint around that category alone. Closing without running this check is leaving a recoverable asset on the table.
(c) Columns to use: store_id, category, revenue, transaction_date

✅ Decisions These Questions Will Inform
QuestionDecision EnabledQ1 — Store revenue trendBuild the closure shortlist vs. recovery watchlistQ2 — Customer count lossConfirm which stores are beyond recoveryQ3 — High-value growing productsAllocate promotional budget and shelf priorityQ4 — Lapsed high spendersSize and target the win-back campaignQ5 — Category bright spots in failing storesFinal closure vs. restructure vs. downsize decision.
