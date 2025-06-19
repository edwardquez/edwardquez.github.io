---
layout: page
title: Sustainable Website Emissions Optimization
description:
img: assets/img/green.png
importance: 2
category: work
giscus_comments: false
---

<details open>
  <summary><strong>Project Overview</strong></summary>
  <p>In this project, we partnered with <span style="color:#b509ac;">Wagtail</span> to investigate the <span style="color:#b509ac;">environmental impact</span> of websites and identify actionable ways to reduce their <span style="color:#b509ac;">carbon footprint</span>. Our focus was on understanding <span style="color:#b509ac;">internet-related CO₂ emissions</span>, evaluating <span style="color:#b509ac;">key drivers</span> of those emissions, and proposing <span style="color:#b509ac;">sustainable web development practices</span>. The client, <span style="color:#b509ac;">Wagtail</span> (a <span style="color:#b509ac;">CMS platform</span>), sought to understand how <span style="color:#b509ac;">design choices</span> and <span style="color:#b509ac;">hosting decisions</span> influence <span style="color:#b509ac;">sustainability</span>.</p>
</details>

<details>
  <summary><strong>The Problem</strong></summary>
  <ul>
    <li>The <span style="color:#b509ac;">internet</span> contributes <span style="color:#b509ac;">3.7%</span> of global <span style="color:#b509ac;">CO₂ emissions</span>, projected to grow to <span style="color:#b509ac;">14%</span> by 2040.</li>
    <li>Each <span style="color:#b509ac;">web page load</span> can produce between <span style="color:#b509ac;">2.79g</span> and <span style="color:#b509ac;">7.26g</span> of <span style="color:#b509ac;">CO₂</span> depending on <span style="color:#b509ac;">infrastructure</span> and <span style="color:#b509ac;">design</span>.</li>
    <li><span style="color:#b509ac;">WordPress</span>, which powers over <span style="color:#b509ac;">60%</span> of websites, has massive potential for <span style="color:#b509ac;">carbon reduction</span> through <span style="color:#b509ac;">sustainable practices</span>.</li>
  </ul>
</details>

<details>
  <summary><strong>Objectives</strong></summary>
  <ul>
    <li>Quantify the <span style="color:#b509ac;">carbon emissions</span> produced by websites.</li>
    <li>Identify which <span style="color:#b509ac;">website features</span> most significantly contribute to emissions.</li>
    <li>Model how emissions could be reduced through <span style="color:#b509ac;">design</span> and <span style="color:#b509ac;">infrastructure improvements</span>.</li>
    <li>Evaluate <span style="color:#b509ac;">economic</span> and <span style="color:#b509ac;">societal benefits</span> from these improvements.</li>
  </ul>
</details>

<details>
  <summary><strong>Methodology</strong></summary>
  <ul>
    <li>Used <span style="color:#b509ac;">Ecograder</span>, an industry-standard tool, to score websites based on <span style="color:#b509ac;">sustainability metrics</span> (e.g., file size, green hosting, caching, image optimization).</li>
    <li>Collected data across <span style="color:#b509ac;">100 websites</span> representing <span style="color:#b509ac;">21 major industries</span> to ensure a representative sample.</li>
    <li>Built a <span style="color:#b509ac;">multiple linear regression model</span> to assess which features most strongly predicted <span style="color:#b509ac;">Ecograder scores</span> and emissions.</li>
  </ul>
</details>

<details>
  <summary><strong>Findings & Impact</strong></summary>

  <p><u>Top predictors of emissions:</u></p>
  <ul>
    <li><span style="color:#b509ac;">File Size (0.47)</span> – image size, unused code</li>
    <li><span style="color:#b509ac;">Green Hosting (18)</span> – renewable-powered servers</li>
    <li><span style="color:#b509ac;">Web Design (0.23)</span> – cache policy, rendering</li>
  </ul>

  <p><u>Impact per 1-point Ecograder score increase:</u></p>
  <ul>
    <li><span style="color:#b509ac;">1.114g CO₂</span> per page load</li>
  </ul>

  <p><u>If applied across all WordPress sites:</u></p>
  <ul>
    <li><span style="color:#b509ac;">368.4 million tons</span> of CO₂ could be eliminated</li>
    <li>Equivalent to a <span style="color:#b509ac;">27.1%</span> cut in total internet emissions</li>
    <li>Results in a <span style="color:#b509ac;">1%</span> reduction in global emissions</li>
    <li>Estimated <span style="color:#b509ac;">$18.79 billion</span> in societal cost savings (based on U.S. government's <span style="color:#b509ac;">$51/ton</span> social cost of carbon).</li>
  </ul>
</details>







--- 
<div class="embed-responsive embed-responsive-16by9" style="margin-top: 2rem; margin-bottom: 2rem;">
  <iframe class="embed-responsive-item" src="https://docs.google.com/presentation/d/e/2PACX-1vSuXjgUUThDGwaSD-WoqvxrI0w-OEPHrj0y6RRxCG2JQdnnOmG0gaOYxLyuSusYWlAVGpaWFZINHuY9/pubembed?start=false&loop=false&delayms=3000" frameborder="0" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
</div>
