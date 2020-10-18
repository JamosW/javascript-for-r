--- 
title: "JavaScript for R"
author: "John Coene"
date: "2020-10-18"
documentclass: krantz
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
colorlinks: yes
lot: yes
lof: yes
site: bookdown::bookdown_site
description: "Invite JavaScript into your Data Science workflow."
github-repo: JohnCoene/javascript-for-r
graphics: yes
---



# Preface {-}

_This is the online version of JavaScript for R, a book currently under development and intended for release as part of the [R series by CRC Press](https://www.routledge.com/Chapman--HallCRC-The-R-Series/book-series/CRCTHERSER)._

<div style = "float:left; width:400px; max-width:100%; margin-right:1em;">
<img src="images/cover.jpg" width = "100%">
<small><span>Photo by <a href="https://unsplash.com/@davisuko?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">davisuko</a> on <a href="https://unsplash.com/s/photos/paint?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a></span></small>
</div>

The R programming language has seen the integration of many languages; C, C++, Python, to name a few, can be seamlessly embedded into R so one can easily call code written in other languages from the R console. Little known to many, R works just as well with JavaScript---this book delves into the various ways both languages can work together.

The ultimate aim of this work is to demonstrate to the reader the many great benefits one can reap by inviting JavaScript into their data science workflow. In that respect the book is not teaching one JavaScript but rather demonstrates how little JavaScript can greatly support and enhance R code. Therefore focus is on integrating external JavaScript libraries and only limited knowledge of JavaScript is required in order to learn from the book. Moreover, the book focuses on generalisable learnings so the reader can transfer takeaways from the book to solve real-world problems.

Throughout the book several shiny applications and R packages are put together as examples, all of these, along with the code for the entire book can be found on the Github repository: [github.com/JohnCoene/javascript-for-r](https://github.com/JohnCoene/javascript-for-r).

## Premise {-}

The R programming language has been propelled into web browsers with the introduction of packages such as [shiny](https://shiny.rstudio.com/) [@R-shiny] and [rmarkdown](https://rmarkdown.rstudio.com/) [@R-rmarkdown] which have greatly improved how R users can communicate complex insights by building interactive web applications and interactive documents. Yet most R developers are not familiar with one of web browsers' core technology: JavaScript. This books aims to remedy to that by revealing how much JavaScript can greatly enhance various stages of data science pipelines from the analysis to the communication of results.

Importantly, the focus of the book truly is the integration of JavaScript with R where both languages either actively interact with one another, or where JavaScript enables doing things otherwise not accessible to R users---it is not merely about including JavaScript code that works alongside R.

## Book Structure {-}

1. The book opens with an introduction to better illustrate its premise, it provides rationales for using JavaScript in conjunction with R which it supports with existing R packages that make use of JavaScript and are available on CRAN. Then it briefly describes concepts essential to understand the rest of the book to ensure the reader can follow along. Finally, this part closes by listing the various methods with which one might make JavaScript work with R.

2. We explore existing integrations of JavaScript and R namely by exploring packages to grasp how these tend to work and the interface to JavaScript they provide.

3. A sizeable part of the book concerns data visualisation, it plunges into creating interactive outputs with the htmlwidgets package. This opens with a brief overview of how it works and libraries that make great candidates to integrate with the htmlwidgets package. Then a first, admittedly unimpressive, widget is built to look under the hood and observe the inner-workings of such outputs in order to grasp a better understanding of how htmlwidgets work. Next, we tackle a more substantial library that allows drawing arcs between countries on a 3D globe. Then, to demonstrate that such packages are not limited to visualisation and more broadly applies to interactive outputs, a second package is built, one that allows to mimic text being typed on the screen. The last two chapter go into more advanced topics such as security and resizing.

4. The fourth part of the book details how JavaScript can work with Shiny. Once the basics out of the way, the second chapter builds the first utility to programmatically display notifications. Then we create a functionality to notify the user when the shiny server is busy running computations. This part of the book ends with an example of custom shiny output for a library that applies filters to images. Finally, shiny and htmlwidgets are (literally) connected by including additional functionalities in interactive visualisations when used with the shiny framework.

5. Finally, we look at how one can use some of the more modern JavaScript technologies such as Vue, React, and webpack with R---these can make the use of JavaScript more agile and robust.

6. Then the book delves into using JavaScript for computations, namely via the V8 engine and node.js. After a short introduction, chapters will walk the reader through various examples: a fuzzy search, a time format converter, and some basic natural language operations.

7. Next the book closes with examples of all the integrations explored previously. This involves recreating (a part of) the plotly package, building an image classifier, adding progress bars to a shiny application, building an app with HTTP cookies and running basic machine learning operations in JavaScript.

8. Finally, the book concludes with some noteworthy remarks on where to go next. 

## Acknowledgement {-}

Many people in the R community have inspired me and provided the knowledge to ultimately write this book, amongst them are [Ramnath Vaidyanathan](https://github.com/ramnathv/) for his amazing work on the htmlwidgets [@R-htmlwidgets] package, [Kent Russel](https://github.com/timelyportfolio) from whom I have learned a lot via his work on making Vue and React accessible in R, and [Carson Sievert](https://github.com/cpsievert) for pioneering probably the most popular integration of R and JavaScript with the plotly [@R-plotly] package.

Early reviewers also shared precious feedback that help make the book dramatically better, thanks to [Maya Gans](@mayacelium), [
Felipe Mattioni Maturana](@felipe_mattioni), and [Wei Su](@Wei_Su) for thoroughly going through every line of the book.