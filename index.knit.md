---
title: "Introduction to ggplot"
author:
- name: Eugene Hickey
  url: https://www.fizzics.ie
  affiliation: Technological University Dublin
  affiliation_url: https://www.tudublin.ie
date: "2022-02-24"
description: |
  An Introduction to ggplot for TU Dublin GRS 2022
site: distill::distill_website
---



<div class="layout-chunk" data-layout="l-body">


</div>


# Welcome

This is the course site for the _Introduction to ggplot_ workshop created by Eugene Hickey for [TU Dublin](https://tudublin.ie).

<aside>
<div class="layout-chunk" data-layout="l-body">
<img src="https://nhsrcommunity.com/wp-content/uploads/2018/02/logo.png" height="43" />

</div>

</aside>

This six-hour hands-on workshop will be a gentle introduction to  [ggplot](https://ggplot2.tidyverse.org/reference/ggplot.html) package as a tool to create impressive graphics and data visualisations.

- **The Morning** will discuss the overall structure of [ggplot](https://ggplot2.tidyverse.org/reference/ggplot.html) and we'll start doing some initial plots; barcharts, boxplots, histograms, point/line plots.....

<aside>
Wednesday, March 8th<br/>10-1pm BST ([check your time zone](https://www.worldtimebuddy.com/?qm=1&lid=2964574,360630,524901&h=2964574&date=2022-3-8&sln=10-13&hf=1
))
</aside>

<div class="layout-chunk" data-layout="l-body">

```{=html}
<div class="shareagain" style="min-width:300px;margin:1em auto;">
<iframe src="https://intro-ggplot-nhs.netlify.app/slides/01-why-ggplot.html" width="1600" height="900" style="border:2px solid currentColor;" loading="lazy" allowfullscreen></iframe>
<script>fitvids('.shareagain', {players: 'iframe'});</script>
</div>
```

</div>



<div class="layout-chunk" data-layout="l-body">

```{=html}
<div class="shareagain" style="min-width:300px;margin:1em auto;">
<iframe src="https://intro-ggplot-nhs.netlify.app/slides/02-proportions.html" width="1600" height="900" style="border:2px solid currentColor;" loading="lazy" allowfullscreen></iframe>
<script>fitvids('.shareagain', {players: 'iframe'});</script>
</div>
```

</div>



<div class="layout-chunk" data-layout="l-body">

```{=html}
<div class="shareagain" style="min-width:300px;margin:1em auto;">
<iframe src="https://intro-ggplot-nhs.netlify.app/slides/03-distributions-relationships.html" width="1600" height="900" style="border:2px solid currentColor;" loading="lazy" allowfullscreen></iframe>
<script>fitvids('.shareagain', {players: 'iframe'});</script>
</div>
```

</div>


- **The Afternoon** will cover colours, themes, facets, and fonts.

<aside>
Wednesday, March 8th<br/>1-4pm BST ([check your time zone](https://www.worldtimebuddy.com/?qm=1&lid=2964574,360630,524901&h=2964574&date=2022-3-8&sln=14-16&hf=1))
</aside>

This workshop is designed for people with previous experience of R but have yet to take the plunge to working with ggplot.

# Prework

## Essential

We'll be using the software listed below.

- Install [R](https://cloud.r-project.org/) and [RStudio Desktop](https://rstudio.com/products/rstudio/download/) on your computer. 

You can find step-by-step instructions for installing these here: [macOS](https://www.youtube.com/watch?v=GM88tYlEy_g), [Windows](https://www.youtube.com/watch?v=JRKmZK5-6aE).


- Install the following packages:

<div class="layout-chunk" data-layout="l-body">
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r"><span class='co'># From CRAN</span>
<span class='va'>list_of_packages</span> <span class='op'>&lt;-</span> <span class='fu'><a href='https://rdrr.io/r/base/c.html'>c</a></span><span class='op'>(</span><span class='st'>"tidyverse"</span><span class='op'>)</span>

<span class='co'># run the following line of code to install the packages you currently do not have</span>
<span class='va'>new_pkgs</span> <span class='op'>&lt;-</span> <span class='va'>list_of_pkgs</span><span class='op'>[</span><span class='op'>!</span><span class='op'>(</span><span class='va'>list_of_pkgs</span> <span class='op'><a href='https://rdrr.io/r/base/match.html'>%in%</a></span> <span class='fu'><a href='https://rdrr.io/r/utils/installed.packages.html'>installed.packages</a></span><span class='op'>(</span><span class='op'>)</span><span class='op'>[</span>,<span class='st'>"Package"</span><span class='op'>]</span><span class='op'>)</span><span class='op'>]</span>
<span class='kw'>if</span><span class='op'>(</span><span class='fu'><a href='https://rdrr.io/r/base/length.html'>length</a></span><span class='op'>(</span><span class='va'>new_pkgs</span><span class='op'>)</span><span class='op'>)</span> <span class='fu'><a href='https://rdrr.io/r/utils/install.packages.html'>install.packages</a></span><span class='op'>(</span><span class='va'>new_pkgs</span><span class='op'>)</span>

<span class='co'># From GitHub</span>
<span class='fu'>devtools</span><span class='fu'>::</span><span class='fu'><a href='https://devtools.r-lib.org/reference/remote-reexports.html'>install_github</a></span><span class='op'>(</span><span class='st'>"nhs-r-community/NHSRdatasets"</span><span class='op'>)</span>
</code></pre></div>

</div>


# Links

- Link to this website:

# Acknowledgments {.appendix}

This workshop draws from various sources, most notably the books by [Kieran Healy](https://socviz.co/) and [Claus Wilkie](https://clauswilke.com/dataviz/). I'd also like to mention the webpage of [The Top 50 ggplot2 Visualisations](http://r-statistics.co/Top50-Ggplot2-Visualizations-MasterList-R-Code.html). This workshop ran smoothly with the help of [Raffaella Salvante](raffaella.salvante@tudublin.ie) as co-pilot.

This website was made with the [distill package](https://rstudio.github.io/distill/) and a custom theme designed by Silvia Canelón.
```{.r .distill-force-highlighting-css}
```
