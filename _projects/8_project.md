---
layout: page
title: Significant Champions League Metrics
description: 
img: assets/img/new_uefa.jpg
importance: 2
category: work
giscus_comments: false
---

Using Champions League Data to Analyze Key Metrics for Tournament Success 


<!-- PROJECT OVERVIEW -->
<details open>
  <summary><strong>Project Overview</strong></summary>
  <p>
    This project examines team performance in the <span style="color: #b509ac;">UEFA Champions League</span> over the past five years using a <span style="color: #b509ac;">data-driven approach</span> to identify which metrics most strongly correlate with tournament success. With football tactics constantly evolving, the study seeks to provide insight into which modern play styles and team characteristics most reliably predict progress in the competition. Success is evaluated at three levels: <span style="color: #b509ac;">qualifying</span> for the tournament, <span style="color: #b509ac;">reaching the Round of 16</span>, and <span style="color: #b509ac;">reaching the Final</span>.
  </p>
</details>

<!-- OBJECTIVES -->
<details>
  <summary><strong>Objectives</strong></summary>
  <ul>
    <li>To determine which <span style="color: #b509ac;">performance metrics</span> correlate most strongly with success in the UEFA Champions League</li>
    <li>To test hypotheses regarding the importance of <span style="color: #b509ac;">offensive metrics</span> such as expected goals (xG), possession, and progression</li>
    <li>To evaluate whether <span style="color: #b509ac;">average team age</span> has a measurable effect on tournament outcomes</li>
    <li>To apply <span style="color: #b509ac;">statistical and predictive models</span> (e.g., bootstrapping and logistic regression) for deeper analysis</li>
  </ul>
</details>

<!-- METHODOLOGY -->
<details>
  <summary><strong>Methodology</strong></summary>
  <p>
    To explore which metrics contribute most to success in the UEFA Champions League, we began by collecting and merging five years' worth of team-level data from <span style="color: #b509ac;">FBref.com</span>. This dataset included over 35 variables such as <span style="color: #b509ac;">possession percentage</span>, <span style="color: #b509ac;">expected goals (xG)</span>, <span style="color: #b509ac;">progressive actions</span>, and <span style="color: #b509ac;">average team age</span> for each participating team.
  </p>
  <p>
    We defined three levels of tournament success: qualifying for the Champions League, advancing to the Round of 16, and reaching the Final. Our analysis focused on four key metrics:
  </p>
  <ul>
    <li><span style="color: #b509ac;">Expected Goals (xG)</span></li>
    <li><span style="color: #b509ac;">Possession (%)</span></li>
    <li><span style="color: #b509ac;">Progressive Carries and Passes</span></li>
    <li><span style="color: #b509ac;">Average Team Age</span></li>
  </ul>
  <p>For each of these metrics, we performed the following steps:</p>
  <ol>
    <li><span style="color: #b509ac;">Descriptive Analysis</span> – We calculated means, variances, and distributions.</li>
    <li><span style="color: #b509ac;">Bootstrapping</span> – We generated 1,000 bootstrap samples to estimate confidence intervals.</li>
    <li><span style="color: #b509ac;">Correlation Analysis</span> – We computed correlation coefficients to assess associations.</li>
    <li><span style="color: #b509ac;">Logistic Regression</span> – We modeled how each metric influenced tournament progression.</li>
  </ol>
</details>

<!-- FINDINGS -->
<details>
  <summary><strong>Findings</strong></summary>

  <!-- xG -->
  <details>
    <summary><strong>Expected Goals (xG)</strong></summary>
    <ul>
      <li>Strong indicator of success, especially for <span style="color: #b509ac;">reaching the Round of 16</span> (correlation ≈ 0.57)</li>
      <li>Finalist teams averaged over <span style="color: #b509ac;">2 xG per game</span></li>
      <li>Logistic regression: finalists had ~<span style="color: #b509ac;">2.31 xG/game</span></li>
    </ul>
  </details>

  <!-- Possession -->
  <details>
    <summary><strong>Possession</strong></summary>
    <ul>
      <li>Average tournament possession: <span style="color: #b509ac;">49.2%</span></li>
      <li>Positive correlation between possession and xG (<span style="color: #b509ac;">r ≈ 0.65</span>)</li>
      <li>Each 1% increase in possession raised odds of Round of 16 by <span style="color: #b509ac;">15%</span>, Final by <span style="color: #b509ac;">5%</span></li>
    </ul>
    <div class="row">
      <div class="col-sm mt-3 mt-md-0" style="max-width: 500px; margin: 0 auto;">
        {% include figure.liquid loading="eager" path="assets/img/poss.png" title="Possession vs Expected Goals" class="img-fluid rounded z-depth-1" %}
      </div>
    </div>
    <div class="caption text-center">
      Teams with higher possession tended to generate more expected goals and achieve deeper tournament runs.
    </div>
  </details>

  <!-- Progressive Carries and Passes -->
  <details>
    <summary><strong>Progressive Carries and Passes</strong></summary>
    <ul>
      <li>Finalist teams: >250 progressive carries, >500 progressive passes</li>
      <li>Higher progression rates associated with xG between <span style="color: #b509ac;">1.5–2.5</span></li>
      <li>Regression confirmed positive impact on progression</li>
    </ul>
    <div class="row">
      <div class="col-sm mt-3 mt-md-0" style="max-width: 500px; margin: 0 auto;">
        {% include figure.liquid loading="eager" path="assets/img/prgc.png" title="Progressive Carries" class="img-fluid rounded z-depth-1" %}
      </div>
    </div>
    <div class="caption text-center">
      Progressive carries (PrgC) were significantly higher among top-performing teams.
    </div>

    <div class="row">
      <div class="col-sm mt-3 mt-md-0" style="max-width: 500px; margin: 0 auto;">
        {% include figure.liquid loading="eager" path="assets/img/prgp.png" title="Progressive Passes" class="img-fluid rounded z-depth-1" %}
      </div>
    </div>
    <div class="caption text-center">
      Teams reaching the finals completed more than 500 progressive passes on average.
    </div>
  </details>

  <!-- Average Team Age -->
  <details>
    <summary><strong>Average Team Age</strong></summary>
    <ul>
      <li>Mean age: ~<span style="color: #b509ac;">26 years</span></li>
      <li>Slight positive correlation with xG (r ≈ 0.2), but not statistically significant</li>
      <li>Confidence interval for age coefficient included zero</li>
    </ul>
    <div class="row">
      <div class="col-sm mt-3 mt-md-0" style="max-width: 500px; margin: 0 auto;">
        {% include figure.liquid loading="eager" path="assets/img/age.png" title="Team Age Distribution" class="img-fluid rounded z-depth-1" %}
      </div>
    </div>
    <div class="caption text-center">
      While most finalists had players aged 26–28, age was not a strong predictor of tournament success.
    </div>
  </details>
</details>

<!-- CONCLUSION -->
<details>
  <summary><strong>Conclusion</strong></summary>
  <p>
    <span style="color: #b509ac;">Expected goals</span>, <span style="color: #b509ac;">possession</span>, and <span style="color: #b509ac;">progressive actions</span> are meaningful indicators of success in the Champions League. <span style="color: #b509ac;">Age</span> appears less predictive, emphasizing the value of <span style="color: #b509ac;">tactical execution</span> over demographic factors. The combination of <span style="color: #b509ac;">bootstrapping</span> and <span style="color: #b509ac;">regression modeling</span> provided robust insights, showing that <span style="color: #b509ac;">high-quality offensive output</span> and <span style="color: #b509ac;">ball control</span> are vital for tournament success.
  </p>
</details>
