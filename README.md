# An R package with real-time data from 4 sources + an Shiny app

## Data Sources (updated daily)
* API to [Tencent SARS-COV-2 website](https://news.qq.com/zt2020/page/feiyan.htm). Updated several times a day, the Tencent website relies on official data obtained from the Chinese provincial health agencies, China National Health Commission (CNHC), the World Health Organization (WHO), and public health agencies in other countries. 
* CNHC, which is official historical statistics for the 34 Chinese provinces and special districts. 
* [Dingxiangyuan](https://ncov.dxy.cn/ncovh5/view/pneumonia)  which has been continuously aggregating official data from provincial and city health agencies and the CNHC. 
* [Wuhan-2019-nCoV GitHub repository](https://github.com/canghailan/Wuhan-2019-nCoV). It derives data from the [literature](https://doi.org/10.1016/S0140-6736(20)30183-5) for December 1, 2019, to January 10, 2020, after which it relies on the Chinese news aggregator Toutiao API. This GitHub repository includes historical data for Chinese cities as well as 43 countries. 

For more details see our [vignette](https://guangchuangyu.github.io/nCov2019/), [Preprint](https://www.medrxiv.org/content/10.1101/2020.02.25.20027433v2), and [Shiny app](http://www.bcloud.org/e/).


## :writing\_hand: Authors

Guangchuang YU

School of Basic Medical Sciences, Southern Medical University

<https://guangchuangyu.github.io>

Xijin Ge (Shiny app)

Department of Mathematics and Statistics, South Dakota State University

<https://www.sdstate.edu/directory/xijin-ge>


If you use `nCov2019`, please cite the following preprint:

Tianzhi Wu, Erqiang Hu, Xijin Ge<sup>\*</sup>, Guangchuang Yu<sup>\*</sup>. [An R package and a website with real-time data on the COVID-19 coronavirus outbreak](https://www.medrxiv.org/content/10.1101/2020.02.25.20027433v2). **medRxiv**, 2020.02.25.20027433. doi: <https://doi.org/10.1101/2020.02.25.20027433> 


## :arrow\_double\_down: Installation

Get the development version from github:

``` r
## install.packages("remotes")
remotes::install_github("GuangchuangYu/nCov2019")
```

+ `get_nCov2019()` to query online latest information
+ `load_nCov2019()` to get historical data
+ `summary` and `[` to access data
+ `plot` to present data on map
+ `dashboard(lang = 'en', remote = TRUE)` to open Shiny app dashboard

## :art: Example

Run the script [example.R](example.R) in R using `source("example.R")`, will produce the following figure:

![](nCov2019.jpg)

## :book: Documents

+ **online vignette**: [nCov2019 for studying COVID-19 coronavirus outbreak](https://guangchuangyu.github.io/nCov2019/)
+ [An R Package to Explore the Novel Coronavirus](https://towardsdatascience.com/an-r-package-to-explore-the-novel-coronavirus-590055738ad6)
+ [检索疫情数据的R包来了](https://mp.weixin.qq.com/s/_0D8ENb-4lGm4UV16Ok28A)
+ [各省市的疫情历史数据来了！](https://mp.weixin.qq.com/s/lrQWGKj-mReWrxfi_4Sw9A)
+ [一次搞定所有的疫情地图](https://mp.weixin.qq.com/s/iWyOvOoLDl2q9VCUEDY52A)
+ [nCov2019：历史数据实现自动更新](https://mp.weixin.qq.com/s/wTqeSVWZCH3YP8YzAj20EQ)


## :chart\_with\_upwards\_trend: Shiny Apps that use `nCov2019`

+ [Coronavirus Tracking dashboard](https://coronavirus.john-coene.com/)
+ [Novel Coronavirus Pneumonia (NCP-2019) Dashboard](https://github.com/gaospecial/NCPdashboard)
+ [Coronavirus COVID-19 outbreak statistics and forecast](http://www.bcloud.org/e/)
+ [新冠状病毒统计和预测](http://www.bcloud.org/v/)
+ [新冠肺炎疫情分析平台](http://14.215.135.56:3838/COVID-19-public/)

## :sparkling\_heart: Collected in resource list

+ [Open-Source-COVID-19](https://weileizeng.github.io/Open-Source-COVID-19/)
+ [Top 7 R resources on COVID-19 Coronavirus](https://www.statsandr.com/blog/top-r-resources-on-covid-19-coronavirus/)
