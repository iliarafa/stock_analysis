# STOCK_ANALYSIS

## OVERVIEW

The purpose of this project is to help our client in his research of the stock market by producing code 
that processes all stocks listed on the market. To accomplish this we have to refactor the initial code 
we composed for him when his research was focused on an initial number of 12 stocks, making sure the 
code runs as fast as possible.

## RESULTS 

### Refactoring the Original Code.

The key element in our refactored code is the  variable ```tickerIndex```. By declaring this variable 
we can dispose of the nested loop that we had to use in the original script. 

```
Dim tickerIndex As Single
    tickerIndex = 0
```
The ticker index allows us to calculate volumes 
without the need of a conditional within the loop.

```tickerVolumes(tickerIndex) = tickerVolumes(tickerIndex) + Cells(i, 8).Value```

Our refactored loop ran in 0.0703125 seconds for 2018 in contrast to 0.3359375 seconds of the original script runtime. 
Similarly for 2017 the refactored code took  0.078125 seconds to run instead of 0.3203125. **The refactored code ran approximately 25% faster.** 

![](resources/test1.png)
 
 ### Stock Performance
 
 The two stocks that stand out are naturally the stocks that show gains for both 2017 and 2018. ENPH has risen by 211.4% in 24 months and RUN has climbed 89,5%. Both stocks have icreased their daily volumes in 2018. ENPH had in fact the highest daily volume in 2018 rising by 275% compared to the year before .Although there was a slight increase in Total Daily Volumes in 2018 by around 6% compared to the previous year some stocks lost or gained volume disproportionately. This might serve as a forecast of higher volatility for these stocks. 
 
 ![](resources/AllStocksAnalysis2017.png)
 
 
