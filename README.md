# What Was Really Driving Revenue Growth in Fashion Retail?

## A Business Analysis of Sales, Products and Customer Behaviour from 2015 to 2024

Revenue growth is usually associated with selling more products. While exploring this dataset, I noticed that the business followed a different pattern.

Revenue continued to rise, but the annual number of orders barely changed.

This raised the question that shaped the entire project:

**If the company was not processing more orders, what was actually driving its growth?**

To investigate this, I combined sales, product and recorded inventory data covering ten years of business activity. Instead of beginning with a fixed assumption, I followed the result through transaction value, units sold, product prices, discounts, seasonality, markets, product groups and customer behaviour.

The analysis is based on **256,506 sales records**, **2,500 products** and **3,741 recorded inventory rows**. Before calculating the main metrics, I separated valid sales activity from orders for which net revenue could be assessed. This allowed customer activity to remain visible even when a missing discount prevented the calculation of net order value.

## The first clue: revenue was growing without more orders

The first step was to compare annual revenue with the number of analysed orders.

<p align="center">
  <img src="assets/01_revenue_orders_aov.png" width="900" alt="Annual revenue growth despite stable order volume">
</p>

<p align="center">
  <i><b>Figure 1.</b> Nominal revenue increased while annual order volume remained almost unchanged.</i>
</p>

Between 2015 and 2024, nominal net revenue increased by **36.8%**, while the number of analysed orders increased by only **1.1%**.

The business was therefore not growing by completing substantially more transactions. It was generating more revenue from almost the same number of orders.

Average Order Value provided the first explanation. It increased from **436 to 590**, which represented growth of **35.3%**.

But an increase in the average still did not explain what was happening inside each transaction. Customers could have been buying more units, choosing more expensive products, receiving smaller discounts or combining these behaviours.

The next step was to separate these effects.

## Customers were not buying substantially more units

I compared the annual number of units sold with the quantity-weighted gross unit price.

<p align="center">
  <img src="assets/02_weighted_price_units.png" width="900" alt="Weighted unit price growth compared with units sold">
</p>

<p align="center">
  <i><b>Figure 2.</b> Units sold remained stable while the weighted unit price increased.</i>
</p>

Units sold increased by only **0.5%**, while the quantity-weighted gross unit price increased by approximately **36.0%**.

This narrowed the explanation considerably. The increase in order value did not come from customers adding substantially more items to their baskets. It was associated mainly with the recorded value of the products being purchased.

There was still one important question left.

Was the company selling a different mix of products, or were the same products becoming more expensive?

To separate these effects, I compared products that appeared in both 2015 and 2024. Within this common-product population, product-level price changes explained **99.5%** of the weighted-price increase, while changes in product unit shares explained only **0.5%**.

The result showed that the higher weighted price was not explained mainly by customers switching towards a different combination of products. The recorded prices of individual products played the dominant role.

This is a numerical decomposition rather than proof of causality. Without inflation, product cost, competitor prices and margin, the analysis cannot determine why those prices changed or whether the pricing strategy was profitable.

## The structure of sales was changing as well

Although product-level price changes explained most of the weighted-price increase, the distribution of sold units across nominal price ranges also changed.

<p align="center">
  <img src="assets/03_price_segment_mix.png" width="900" alt="Share of units sold by nominal price range">
</p>

<p align="center">
  <i><b>Figure 3.</b> Premium and High-End products represented a growing share of units sold.</i>
</p>

The Premium share of sold units increased by **14.4 percentage points**, while the High-End share increased by **11.3 points**. At the same time, the Budget share fell by **14.8 points**.

At first glance, this could suggest that customers were increasingly choosing more expensive products. However, the price ranges are nominal. A product could move into a higher segment because its own recorded price changed, even when customer preference remained the same.

For that reason, I did not treat the changing sales mix as a separate explanation of growth. I interpreted it together with the common-product decomposition.

The combined result was more precise: the business increasingly generated sales in higher nominal price ranges, but this movement was driven mainly by changes in product prices rather than a major change in the number or type of products purchased.

## Was the increase visible across ordinary orders?

Average Order Value can be influenced by a relatively small number of large transactions. Before treating its increase as representative of the wider customer base, the updated analysis also compares the median and upper percentiles of order value.

<p align="center">
  <img src="assets/05_order_value_distribution.png" width="900" alt="Order value distribution between 2015 and 2024">
</p>

<p align="center">
  <i><b>Figure 4.</b> Change in the median and upper percentiles of order value.</i>
</p>

Between 2015 and 2024, the median order value changed by **[MEDIAN_CHANGE]%**, while the 75th and 90th percentiles changed by **[P75_CHANGE]%** and **[P90_CHANGE]%**.

The top 10% of orders generated **[TOP_10_REVENUE_SHARE]%** of analysed revenue in 2024.

These results show whether higher transaction value was visible across the order distribution or concentrated mainly among the largest purchases. They should be completed only after the updated analysis has been run.

## Growth followed a remarkably consistent calendar

Once the main revenue driver had been identified, I examined whether the increase was distributed evenly throughout the year.

It was not.

<p align="center">
  <img src="assets/04_monthly_seasonality.png" width="900" alt="Cumulative monthly revenue pattern">
</p>

<p align="center">
  <i><b>Figure 5.</b> December consistently generated the highest revenue, while February generated the lowest.</i>
</p>

December was the strongest month and February the weakest in every analysed year.

The pattern remained visible after accounting for the different number of days in each month. Average daily revenue in December was **2.03 times** the February level.

This consistency makes the year-end peak relevant for commercial and operational planning. It does not automatically justify higher campaign spending. Before making that recommendation, the company would need campaign costs, contribution margin, fulfilment capacity and evidence that additional promotion generates incremental sales.

## Markets reached similar scale through different paths

Total ten-year revenue was relatively evenly distributed across the analysed markets. Looking only at the final totals could therefore suggest that their performance was similar.

The yearly development showed a more complicated picture.

France recorded the strongest increase between 2015 and 2024 at **40.4%**, while the Czech Republic recorded **32.8%**. Across the complete market-year series, I identified **13 year-over-year declines**.

This means that long-term growth should not be described as uninterrupted expansion. Markets reached a similar aggregate scale despite following different yearly paths.

The product structure was more stable. Shoes remained the largest category in every market and generated approximately **28–29%** of country revenue. Women contributed around **24%**.

At subcategory level, Bags, Scarves and Jewelry recorded the strongest growth. The weakest increases were concentrated in Men's Outerwear, Kids' Shoes and Men's Jeans.

These results show where further investigation would be most useful, but they do not show which areas were most profitable. Revenue alone does not include product cost, returns or cost-to-serve.

## Discounts supported sales, but they did not explain the growth

Most analysed orders and revenue were generated using discounts of no more than 20%.

Orders with discounts at or below this level represented **78.9% of orders** and **82.0% of analysed revenue**.

Discounting was therefore part of normal commercial activity, but the available results did not indicate that increasingly aggressive promotions were the main driver of long-term revenue growth.

A full promotional analysis would require information about campaign exposure, offer type, margin, customer eligibility and the incremental sales generated by each promotion.

## The customer base did not follow the expected 80/20 pattern

The next part of the analysis examined whether revenue growth depended on a small group of high-value customers.

<p align="center">
  <img src="assets/06_customer_revenue_concentration.png" width="900" alt="Customer revenue concentration in 2024">
</p>

<p align="center">
  <i><b>Figure 6.</b> More than half of active customers were required to generate 80% of revenue.</i>
</p>

In 2024, **55.2% of active customers** were required to generate 80% of analysed revenue.

The top 10% generated **25.9%**, while the bottom half generated **24.0%**. Revenue was therefore distributed across a relatively broad customer base rather than concentrated in a small group following a classic 80/20 structure.

This changed the customer question.

The most useful next step was no longer simply identifying the highest-spending customers. It was understanding which customers were likely to remain active.

## Only part of the customer base returned from one year to the next

Among customers active in 2024, **32.5% had also purchased in 2023**. They generated **33.2% of analysed 2024 revenue**.

I describe this as consecutive-year activity rather than formal customer retention. The dataset does not contain a confirmed acquisition date or an expected purchase cycle, so the absence of a purchase in the following year cannot be treated as permanent customer churn.

The historical result raised a forward-looking question:

**Could customer behaviour in one year help identify who was most likely to purchase in the next?**

## Moving from explanation to prediction

To answer this question, I transformed the transaction data into annual customer snapshots. Each row represents one customer in one feature year, while the target indicates whether that customer made an observed purchase in the following calendar year.

The features are calculated only from information available by the end of the feature year. They include purchase recency, order frequency, assessable revenue, order-value statistics, active months, recent activity, product diversity, discount behaviour, previous-year activity and observed customer tenure.

Raw customer and order identifiers are retained only as keys and are not supplied to the models.

A random train-test split would mix earlier and later customer periods, so the models are evaluated chronologically. Customer behaviour from 2016–2021 forms the training period, 2022 is used to validate purchases in 2023, and 2023 behaviour forms the final test for purchases recorded in 2024.

Regularised Logistic Regression and Random Forest are compared with a constant-probability baseline and a simple rule based on previous-year activity. The more complex model is selected only when it provides a meaningful improvement over the simpler alternative.

<p align="center">
  <img src="assets/07_model_lift.png" width="900" alt="Repeat-purchase model lift by customer score group">
</p>

<p align="center">
  <i><b>Figure 7.</b> Observed next-year purchase activity across customer propensity groups.</i>
</p>

On the final temporal test, **[SELECTED_MODEL]** achieved a ROC-AUC of **[ROC_AUC]** and Average Precision of **[AVERAGE_PRECISION]**.

The 20% of customers with the highest predicted scores contained **[CAPTURE_RATE]%** of customers who actually purchased in the following year. Their purchase rate was **[LIFT] times** the average test-population rate.

These fields should be completed only after the model has been evaluated on the untouched final test period.

## From a probability score to a business decision

A high probability of purchasing again does not automatically mean that a customer should receive the highest marketing priority.

Customers with a high natural probability may return without an additional incentive. At the same time, a high-value customer with a lower probability of returning may deserve closer attention.

For that reason, the final score is combined with observed customer revenue. This creates four practical groups: high-value customers likely to return, high-value customers with lower natural purchase probability, lower-value customers with development potential and a lower-priority group.

The result supports customer review and campaign testing. It should not be interpreted as an automatic instruction to contact or exclude a particular customer.

## What marketing data would allow us to do next

The current model answers:

**Who is likely to purchase again?**

It cannot answer:

**Whose decision would change because of a campaign?**

To make that distinction, the company would need campaign exposure, contact date, communication channel, offer type and a treatment-control indicator. These variables would make uplift modelling possible.

A standard propensity model may rank customers who were already likely to purchase. Uplift modelling would instead focus on customers whose purchase probability increased because they received the campaign.

Acquisition source and marketing spend would add another missing part of the story. The business could compare repeat-purchase rate, margin, Customer Acquisition Cost, payback period and LTV-to-CAC across channels rather than analysing customer value without the cost of acquiring it.

Campaign cost, discount cost, gross margin, fulfilment cost and returns would also allow customers to be ranked by expected incremental profit:

```text
expected incremental profit
= incremental response probability
× expected contribution margin
− contact and incentive cost
```

The strongest next step would be a randomised campaign with a control group.

The current data helps identify **who is likely to return**. Marketing-response data would help identify **who should be contacted**. Experimental and cost data would show **which action creates additional profit**.

## Why the inventory analysis stops before optimisation

The inventory file initially appeared to offer an opportunity to compare stock allocation with product demand.

The update history changed what could be concluded.

Approximately **85.0% of inventory rows were more than 90 days old**, while the median recorded age was **303 days**. These records cannot support reliable conclusions about current shortages, excess stock or replenishment needs.

The recorded category structure was close to the structure of 2024 unit sales, with the largest difference equal to **1.3 percentage points**. This is a useful structural comparison, but it is not evidence that stock was sufficient or correctly allocated at a particular moment.

Rather than force an operational recommendation from outdated records, I kept the inventory section as an example of how data quality can limit the scope of a business conclusion.

## What the analysis revealed

The business generated substantially more nominal revenue without processing substantially more orders or selling many more units.

The main numerical change was the increase in recorded product prices. The sales structure consequently moved towards higher nominal price ranges, while discounts remained concentrated at moderate levels.

Growth was not distributed evenly across the calendar, markets or products. December remained consistently dominant, market paths included several annual declines, and subcategory performance varied considerably.

Revenue was also less concentrated among customers than an 80/20 assumption would suggest. This made customer continuity and next-year purchase probability more useful than focusing only on a small group of top spenders.

The predictive extension turns the historical analysis into a customer-prioritisation framework, while clearly separating natural purchase probability from campaign response.

## Business implications

Future revenue growth should be evaluated using more than revenue and Average Order Value. Orders, units, the median and upper percentiles of order value, quantity-weighted price, margin and returns should be monitored together.

Product-level price changes should be compared with unit response and profitability before further pricing decisions are made. Higher nominal revenue does not necessarily mean that the business created more real or profitable value.

The repeated year-end peak should be included in commercial and fulfilment planning, but additional promotional spending should be tested rather than assumed to be effective.

The customer model should be used to prioritise further analysis and controlled experiments. It predicts observed next-year activity, not customer profitability, campaign responsiveness or causal impact.

## Limitations

Revenue is analysed in nominal terms because inflation-adjusted values are unavailable. Orders with missing discounts remain available for activity analysis but do not contribute to net-revenue calculations.

Records containing the unresolved `quantity = 608` value are excluded from the main analysis. The recorded product launch date is not reliable enough to support conclusions about new-product performance.

The dataset begins in 2015, so the first observed customer purchase may not represent the true beginning of the relationship. The target uses a calendar-year horizon and should not be interpreted as permanent churn.

Product cost, margin, returns, campaign exposure, acquisition source and communication history are unavailable. The model therefore predicts natural next-year purchase activity rather than campaign response or incremental profit.

Predictions produced from 2024 customer behaviour for 2025 cannot be evaluated until later activity becomes available.

## Repository structure

```text
retail-revenue-repeat-purchase/
├── assets/
│   ├── 01_revenue_orders_aov.png
│   ├── 02_weighted_price_units.png
│   ├── 03_price_segment_mix.png
│   ├── 04_monthly_seasonality.png
│   ├── 05_order_value_distribution.png
│   ├── 06_customer_revenue_concentration.png
│   └── 07_model_lift.png
├── notebooks/
│   └── Retail_Sales_Business_Analysis.ipynb
├── README.md
├── requirements.txt
└── LICENSE
```

The project was created in Python using Pandas, NumPy, Matplotlib and Scikit-learn.

## Author

**Oliwia Małkus**

Aspiring Data Analyst focused on business analysis, data quality, interpretable modelling and presenting analytical results as a clear business story.
