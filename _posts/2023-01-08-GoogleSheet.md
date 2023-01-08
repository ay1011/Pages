---
toc: true
layout: post
description: GoogleSheet Formula for Malaysian Stock Prices
categories: [markdown]
title: GoogleSheet Formula for Malaysian Stock Prices
---

# GoogleSheet Formula for Malaysian Stock Prices[^1]

Replace the stock code 5014 with your stock ticker
```
=index(ImportXML("https://klse.i3investor.com/web/stock/overview/5014?randomstring", "//*[@id='stock-price-info']/div[1]/p[2]/strong"), 1, 1)
```
Formula for referring to  stock ticker in A1 cell 
```
=index(ImportXML("https://klse.i3investor.com/web/stock/overview/"&A1&"?randomstring", "//*[@id='stock-price-info']/div[1]/p[2]/strong"), 1, 1)
```
## Footnotes

[^1]: Extracted from [klse.i3investor](https://klse.i3investor.com/web/stock/overview/5014)

