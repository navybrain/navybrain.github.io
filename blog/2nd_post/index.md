---
layout: post
title:  "소셜데이터 분석을 통한 트렌드 리포트"
subtitle: "상반기 고객 평판 분석"
type: "소셜분석"
blog: true
text: true
author: "Hojae Han"
post-header: true
order: 2
---

# big data analytics with R
## 소셜 빅데이터 분석

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

엠포스에서 빅데이터 분석을 해봤습니다<sub>~</sub><http://http://www.emforce.co.kr>

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

Including Plots
---------------

You can also embed plots, for example:

<img src="index_files/figure-markdown_github/pressure-1.png" style="display: block; margin: auto;" />

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.

``` r
require(ggplot2)
```

    ## Loading required package: ggplot2

``` r
require(plotly)
```

    ## Loading required package: plotly

    ## 
    ## Attaching package: 'plotly'

    ## The following object is masked from 'package:ggplot2':
    ## 
    ##     last_plot

    ## The following object is masked from 'package:stats':
    ## 
    ##     filter

    ## The following object is masked from 'package:graphics':
    ## 
    ##     layout

``` r
hhj_theme <- theme_classic(base_family="NanumGothic") +
  theme(#axis.text.x = element_text(angle = 45),
    strip.background = element_rect(colour = "white", fill = "white"), 
    axis.line = element_line(colour = "#EBEBEB"), 
    panel.spacing = unit(1, "lines")
  )

theme_set(hhj_theme)
```

------------------------------------------------------------------------

> plot result

``` r
p <- ggplot(pressure, aes(temperature, pressure, color = "")) +
  geom_point()

p
```

<img src="index_files/figure-markdown_github/unnamed-chunk-3-1.png" style="display: block; margin: auto;" />

Conclusion
----------

엠포스의 빅데이터 분석을 통해 마케팅 분야의 ...
