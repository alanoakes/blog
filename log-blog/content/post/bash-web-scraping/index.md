---
date: 2023-07-12T01:01:00
title: "Linux Web-Scraping"
tags: [Bash, DataAnalysis, WebScraping]
toc: false
---

Here is web scraping tip to put in your toolbox.

### Problem

I ran into this headache when building a web scraper for extracting some
personal data sets and I found such a simple solution I had to share!!

When looping over an array of variables with page numbers I ran into a problem
since web scraping does not use a browser and the variables don't have the same
amount of pages. The problem is called redirection. Redirection happens when
a website host points a user to a new page from a 400-500 response code.

### Solution

The way around this is to set your `wget` call with `--max-redirect` to 0. If
you do not set it to 0, then your data set duplicates rows since the host will
redirect you to a previous connection each time you loop over the non-existent
page numbers.

{{< figureCupper 
img="bashWebScraping.jpg"
caption="Note: the above code example is not active, but kept simple for explanation purposes."
command="Resize"
options="700x" >}}

What are your thoughts about dealing with redirection in web scraping?
