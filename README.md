# Portfolio Analysis

## 1 Build Your own Portfolio

###  Select Any stock as you want and take the S&P500 as benchmark
![image](https://user-images.githubusercontent.com/73721315/162109690-40ebcd8d-ec27-4708-b4dd-83f9f1eec71f.png)
- Choose initial 31 stocks from utility sectors as example
- Take an overview on their perfoimaces in the past 5 years (too many overlaps here)

###  Breakdown to Individual Stock
![image](https://user-images.githubusercontent.com/73721315/162101856-ef71aec2-4f6e-46ba-815f-8d093829ed63.png)
- S&P500 as becnhmark only has increaeed by 1.8 times in the past 5 years 
- AMRC has tenfold in the past 5 years.
- MSEX has triple in the past 5 years.
- TTEK has quadrupled. 
- AWR,AWK,GWRS and MYRG all have doubled than 5 years before

###  Pay Attention to Stocks outperforamced Benchmark 
![image](https://user-images.githubusercontent.com/73721315/162112346-bb7e8e74-c596-42d4-90fb-d32f2c42dcb4.png)
- You should really take AMRC consideration
![image](https://user-images.githubusercontent.com/73721315/162112706-af0f1ad6-53bf-4a08-b1c6-758c714362a6.png)
- After removing the AMRC and amplifing the trends of other stocks
- we found those stocks seem are good to be included in portfolio, which could provide profibility factors

### Dig into Monthly Returns of Selected Factors
![image](https://user-images.githubusercontent.com/73721315/162261534-43e93c0e-b8cc-4ab2-b09e-06115a8a95d5.png)
- seems all are  **stationary time serises**

### Augmented Dickey-Fuller Test (ADF)
<img width="296" alt="image" src="https://user-images.githubusercontent.com/73721315/162262061-7f8852cc-ebce-498e-b171-293b467b0e81.png">

- The results of p-value prove that they are all strong stationary
- means you can regard its average monthly return as a expected monlthy return in a long-term aspect

### Overview of Expected Monthly Return for individual Stock
![image](https://user-images.githubusercontent.com/73721315/162265763-a10efeec-e30f-4670-8311-4805fe054e6b.png)

- **AQUA** and **MTZ** has a high expected return but has been ignored before 
- Drop those stocks have negative expected returns

### Estimated Risk (Standard Deviation) 
![image](https://user-images.githubusercontent.com/73721315/162330812-ec7eb2ca-fad7-407a-a22d-56f8b7811951.png)
- **ARTNA** has a trait on stability that could lower the risk for the portfolio

### Sharpe Ratios for Selected Stocks
![image](https://user-images.githubusercontent.com/73721315/162330186-40bca660-ee31-47cc-8edd-b6cbdd425553.png)
#### Based on all analysises above, I will pick out stocks into my profolio as belows :
- AMRC,TTEK,MYRG,AQUA,MSEX,MTZ,AWK,GWRS,AWR(Profibility factors)
- ARTNA (low risk factor)

## 2 Optimize Portfolio

### Correlation Matrix of Portfolio
![image](https://user-images.githubusercontent.com/73721315/162336443-ccedcdfe-dbe1-4e6b-b1ba-3b76c9891667.png)
- Highlighting the weak correlations (<= 0.2)
- The portfolio looks well diversified 

### Using Monte Carlo to Simulate Market Efficient Frontier 
![image](https://user-images.githubusercontent.com/73721315/162338974-72e87005-4ba4-443c-a0f2-cef1ca73d4a1.png)
- Efficient Frontier helps in giving optimal weights to each stocks in your portfolio
- For the convenience of calculation, I setted a minimum weight for each stock, which is 0.1% (tiny but useful)
- By running the simulations for 500k times, the result shows the **red star** represnting the optimal point has the maximum sharpe ratio, which is 0.406, and **yellow star** representing the optimal point has the minimum risk,which the standard deviation is only 0.03

### Visualizing the Optimiztions 

![image](https://user-images.githubusercontent.com/73721315/162346610-f9f8ff49-8d49-41f2-ad4f-c805a5239b51.png)  ![image](https://user-images.githubusercontent.com/73721315/162346801-f12c0e86-8724-43ee-91e8-1ba80d1f2b63.png)

- The model of maximum sharpe ratio suggests to invest on **TTEK**(29%),**AMRC**(21.4%),**AWR**(12.8%),**MSEX**(28.2%) and **MYRG**(8%) respectively
- The recent price indexs of big holdings
- AMRC(21.4%) looks like the factor generating most profit, while the rests for lowering the volatility


![image](https://user-images.githubusercontent.com/73721315/162347422-daa27999-b068-4582-88cd-53ddc8c5c9f1.png) ![image](https://user-images.githubusercontent.com/73721315/162347461-a40c5526-25ed-4f85-9762-532757c08418.png)

- The model of minimum volatility suggests to invest on **TTEK**(29%),**AMRC**(21.4%),**AWR**(12.8%),**MSEX**(28.2%) and **MYRG**(8%) respectively
- The recent price indexs of big holdings


## 3 Test the profibility of Portfolio with Benchmark

![image](https://user-images.githubusercontent.com/73721315/162347577-1f21eacc-f39a-4834-984d-c3f485f0055f.png)
- The portfolio of max sharpe ratio did apparently outperform S&P500 and it has a similar pattern as **AMRC**, which implys **AMRC** did contribute a lot to the whold portfolio even with the holdings of 21.4%.
- The portflio of minmum volatility barely outperform the benckmark but stabler than each individual stock of portfolio. 













