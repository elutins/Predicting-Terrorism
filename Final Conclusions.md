## Final Report

> For the Bayesian Inference portion of the project, the dataset was divided into two populations; pre-2003 and post-2003 bombings in the Middle East.  The intention of this timeline was to test the hypothesis that the American Government's decision in the early 21st century to disban the Iraqi military ultimately led to more violence and turmoil in the Middle East.  In 2003, the Bush administration issued an order to wipe away the Iraqi military in hopes of terminating any ties with Saddam Hussein's regime. Rather than gradually diffusing to peace and civil cooperation, the decision led to societal unrest, growing insurgency, and a U.S. military occupation of Iraq that would last roughly eight years. The American government has come under much scrutiny for this decision for many reasons. Firstly, many believe the American government had the opportunity of scrubbing the Iraqi military of Hussein loyalists and keeping the rest of the army intact. Secondly, the decision to disban the Iraqi military left thousands of Sunni soldiers -- formerly loyal to Saddam Hussein -- without a job and looking for a movement to join. Unfortunately, the popular movement to join turned out to be Al-Qaida. Al-Qaida established Al-Qaida in Iraq (AQI) to wage insurgency against the US troops. During the Iraq war, AQI moved into Syria and renamed itself the Islamic State of Iraq & Syria, better known as ISIS.

> The goal of the Bayesian inference was to calculate the posterior distribution of the mean bombings to occur in the Middle East pre and post 2003. For prior to 2003, after calculating the likelihood, it was derived that the mean annual bombings followed a normal distribution with a mean of 139 bombings per year. It can be stated with 95% confidence interval that the mean fell between 110 - 167 bombings per year. The standard deviation for pre-2003 also followed a normal distribution with a mean of 81 bombings (that is on average a standard deviation of 81 bombings/year).

> Similarly, the posterior distribution for mean bombings post-2003 followed a normal distribution with a mean of 1,821 bombings per year. It can be stated with a 95% confidence interval that the mean falls between 971 - 2700 bombings per year. The standard deviation of the mean bombings post-2003 also followed a normal distribution with a mean of 1620 bombings per year.

> While the American Goverment's decision to disban the Iraqi military may very well not be the only factor that led to a the increase in annual Mid-East bombings after 2003, the conducted Bayesian inference proves of the drastic leap in mean bombings between the two time periods. In future studies, the immediate years leading up to and following 2003 will be measured and used for Bayesian inference to make more definitive conclusions about this 2003 decision by the American government. Visualizations for the posterior distribution for each population can be found below this write-up.

> Regarding the second portion of the project which entailed predicting the number of bombings in 1993, Autoregressive-Moving Average temperalspatial models were built. The dataset was divided into the designated regions, with an ARMA/ARIMA model built for each region (there were 12 regions in total).  The temperalspatial models were built to strictly predict the number of bombings that occured in each region in 2003.  In order to improve accuracy of the predictions, the dates of each attack were broken down and grouped by year and the corresponding month. This was done to test if there were any seasonal trends in the regional data, hoping to gain interpretability as well. The first step of building the ARMA/ARIMA model was to test the data for stationarity. Utilizing a built-in function that plotted the data and brought back results of the Dickey-Fuller test, the number of bombings per month was tested for stationarity. If the data was stationary, a simple ARMA model was built to predict 1993 bombings. However, if the data was not already stationary, and a "first difference" or "seasonal first difference" was calculated to gain stationary, a more complex ARIMA model was built.

#### Based on the results of the twelve ARIMA models that were built, one for each region, the predictions for 1993 bombings are as followed:
- Australasia & Oceania: 30
- North America: 24
- Central America and Caribbean: 39
- South America: 39
- East Asia: 4
- Southeast Asia: 8
- Central Asia: 3
- Western Europe: 47
- Eastern Europe: 12
- Middle East & North Africa: 89
- South Asia: 13
- Sub-Saharan Africa: 11
- Total: 319 Bombings
