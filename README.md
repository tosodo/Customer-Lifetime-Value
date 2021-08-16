
**Customer Lifetime Value (CLV)**

[[Still subject to future changes]] 

------------------------------------------------------------------------
------------------------------------------------------------------------


Working out Customer Lifetime Value (CLV) with Recency, Frequency, and Monetary (RFM)
------------------------------------------------------------------------

CLV, "the present value of future cash flow attributed to a customer's tenure with a company", can be determined by variety of approaches.  Based on a simple [equation](http://www.r-bloggers.com/calculating-customer-lifetime-value-with-recency-frequency-and-monetary-rfm/), one can calculate the cumulative profit (value) from a customer based on assumptions such as retention rate and historical profit margin from customers.  However, a customer's retention can be influenced by factors such as demographics (age, geography, education background), behavior (Recency, Purchase Frequency, Monetary Contribution), competitions, peer influences, etc..  As a result, a dynamic approach should be taken to account for such variations.

In this repo, I calculated CLV by predicting the retention rate (r) of customers' future purchasing cycle using Logistic Regression based on his/her Recency of purchase, purchase Frequency, and Monetary contribution from past purchases.

------
### RFM
By definition, RFM represents:

 - R(ecency): how recently did a customer make a purchase?
 - F(rquency): how often does the customer make purchases?
 - M(onetary Value): how much do they purchase each time on average?


------
### Data
The CDNow data set ([DOWNLOAD](http://brucehardie.com/datasets/)) has 69,659 transaction records by 23,570 different customers. The purchase records between Jan 1997 and June 1998 are also captured.

------
### Code

 - Source code ([R](/2_Code/RFM_v0.2.R))

------
### References
This project was mainly inspired by the work done by Jack Han at [Data Apple](http://www.dataapple.net/?p=84).  However, new libraries/functions are used to update data transformation and visualization of data such as dplyr and ggviz.

Other references used:

 - [Customer Lifetime Value (CLV) – A Methodology for Quantifying and Managing Future Cash Flows, David C. Ogden](http://www.sas.com/content/dam/SAS/en_ca/User%20Group%20Presentations/Montreal-Business-Analytics-Forum/DavidOgden-CustomerLifetimeValue-Nov2009.pdf)




