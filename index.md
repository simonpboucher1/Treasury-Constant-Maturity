## Treasury Constant Maturity 


#### 1-Month Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/1MONTH_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/1MONTH_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/1MONTH_MONTHLY.csv)

#### 3-Month Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/3MONTHS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/3MONTHS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/3MONTHS_MONTHLY.csv)

#### 6-Month Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/6MONTHS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/6MONTHS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/6MONTHS_MONTHLY.csv)



#### 1-Year Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/1YEAR_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/1YEAR_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/1YEAR_MONTHLY.csv)

#### 2-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/2YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/2YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/2YEARS_MONTHLY.csv)


#### 3-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/3YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/3YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/3YEARS_MONTHLY.csv)

#### 5-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/5YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/5YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/5YEARS_MONTHLY.csv)


#### 7-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/7YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/7YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/7YEARS_MONTHLY.csv)


#### 10-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/10YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/10YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/10YEARS_MONTHLY.csv)


#### 20-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/20YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/20YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/20YEARS_MONTHLY.csv)


#### 30-Years Treasury Constant Maturity Rate

* [Daily](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/30YEARS_DAILY.csv) 
* [Weekly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/30YEARS_WEEKLY.csv) 
* [Monthly](https://raw.githubusercontent.com/simonpboucher1/Treasury-Constant-Maturity/main/30YEARS_MONTHLY.csv)


```{R}
install.packages("fredr")
install.packages("ggplot2")
library(fredr)
library(ggplot2)

setwd("~/Dropbox/Mon Mac (MacBook-Pro-de-Simon-Pierre.local)/Documents/GitHub/Treasury-Constant-Maturity")

fredr_set_key("5d6f76382d7d188e9166bb3b96c8f934")

DGS1MO<-fredr_series_observations(series_id = "DGS1MO") 
GS1M<-fredr_series_observations(series_id = "GS1M") 
WGS1MO<-fredr_series_observations(series_id = "WGS1MO") 

DGS3MO<-fredr_series_observations(series_id = "DGS3MO") 
GS3M<-fredr_series_observations(series_id = "GS3M") 
WGS3MO<-fredr_series_observations(series_id = "WGS3MO") 

DGS6MO<-fredr_series_observations(series_id = "DGS6MO") 
GS6M<-fredr_series_observations(series_id = "GS6M") 
WGS6MO<-fredr_series_observations(series_id = "WGS6MO") 

DGS1<-fredr_series_observations(series_id = "DGS1") 
GS1<-fredr_series_observations(series_id = "GS1") 
WGS1YR<-fredr_series_observations(series_id = "WGS1YR") 

DGS2<-fredr_series_observations(series_id = "DGS2") 
GS2<-fredr_series_observations(series_id = "GS2") 
WGS2YR<-fredr_series_observations(series_id = "WGS2YR") 

DGS3<-fredr_series_observations(series_id = "DGS3") 
GS3<-fredr_series_observations(series_id = "GS3") 
WGS3YR<-fredr_series_observations(series_id = "WGS3YR") 

DGS5<-fredr_series_observations(series_id = "DGS5") 
GS5<-fredr_series_observations(series_id = "GS5") 
WGS5YR<-fredr_series_observations(series_id = "WGS5YR") 

DGS7<-fredr_series_observations(series_id = "DGS7") 
GS7<-fredr_series_observations(series_id = "GS7") 
WGS7YR<-fredr_series_observations(series_id = "WGS7YR") 

DGS10<-fredr_series_observations(series_id = "DGS10") 
GS10<-fredr_series_observations(series_id = "GS10") 
WGS10YR<-fredr_series_observations(series_id = "WGS10YR") 

DGS20<-fredr_series_observations(series_id = "DGS20") 
GS20<-fredr_series_observations(series_id = "GS20") 
WGS20YR<-fredr_series_observations(series_id = "WGS20YR") 

DGS30<-fredr_series_observations(series_id = "DGS30") 
GS30<-fredr_series_observations(series_id = "GS30") 
WGS30YR<-fredr_series_observations(series_id = "WGS30YR") 

write.csv(DGS1MO,"1MONTH_DAILY.csv")
write.csv(GS1M,"1MONTH_MONTHLY.csv")
write.csv(WGS1MO,"1MONTH_WEEKLY.csv")
write.csv(DGS3MO,"3MONTHS_DAILY.csv")
write.csv(GS3M,"3MONTHS_MONTHLY.csv")
write.csv(WGS3MO,"3MONTHS_WEEKLY.csv")
write.csv(DGS6MO,"6MONTHS_DAILY.csv")
write.csv(GS6M,"6MONTHS_MONTHLY.csv")
write.csv(WGS6MO,"6MONTHS_WEEKLY.csv")
write.csv(DGS1,"1YEAR_DAILY.csv")
write.csv(GS1,"1YEAR_MONTHLY.csv")
write.csv(WGS1YR,"1YEAR_WEEKLY.csv")
write.csv(DGS2,"2YEARS_DAILY.csv")
write.csv(GS2,"2YEARS_MONTHLY.csv")
write.csv(WGS2YR,"2YEARS_WEEKLY.csv")
write.csv(DGS3,"3YEARS_DAILY.csv")
write.csv(GS3,"3YEARS_MONTHLY.csv")
write.csv(WGS3YR,"3YEARS_WEEKLY.csv")
write.csv(DGS5,"5YEARS_DAILY.csv")
write.csv(GS5,"5YEARS_MONTHLY.csv")
write.csv(WGS5YR,"5YEARS_WEEKLY.csv")
write.csv(DGS7,"7YEARS_DAILY.csv")
write.csv(GS7,"7YEARS_MONTHLY.csv")
write.csv(WGS7YR,"7YEARS_WEEKLY.csv")
write.csv(DGS10,"10YEARS_DAILY.csv")
write.csv(GS10,"10YEARS_MONTHLY.csv")
write.csv(WGS10YR,"10YEARS_WEEKLY.csv")
write.csv(DGS20,"20YEARS_DAILY.csv")
write.csv(GS20,"20YEARS_MONTHLY.csv")
write.csv(WGS20YR,"20YEARS_WEEKLY.csv")
write.csv(DGS30,"30YEARS_DAILY.csv")
write.csv(GS30,"30YEARS_MONTHLY.csv")
write.csv(WGS30YR,"30YEARS_WEEKLY.csv")
```
