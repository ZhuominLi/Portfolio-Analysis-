# Portfolio-Analysis-
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

### Market Efficient Frontier 










