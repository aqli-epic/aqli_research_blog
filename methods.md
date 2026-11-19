---
layout: page
title: "Methods"
section: "Documentation"
permalink: /methods/
standfirst: "The equation, the coefficient, and the seven things every post has to declare before it goes up."
math: true
---

AQLI-style communication links long-term PM<sub>2.5</sub> exposure to life expectancy through one clear, linear relationship. This simplicity is deliberate: it makes the results easy to understand, compare, and check.

## The calculation

$$
\Delta LE = \left( PM_{2.5}^{\text{baseline}} - PM_{2.5}^{\text{target}} \right) \times \beta
$$

| Symbol | Meaning | Units |
|---|---|---|
| $$PM_{2.5}^{\text{baseline}}$$ | Baseline annual average concentration | µg/m³ |
| $$PM_{2.5}^{\text{target}}$$ | WHO guideline, national standard, or policy target | µg/m³ |
| $$\beta$$ | Life-expectancy gain per 1 µg/m³ reduction | years per µg/m³ |
| $$\Delta LE$$ | Estimated life-expectancy gain | years |

This site uses $$\beta = {{ site.aqli_coefficient }}$$ and a WHO guideline of
{{ site.who_guideline }} µg/m³ throughout. Both are set once, in `_config.yml`, so a single edit
propagates to every page rather than leaving stale numbers behind in prose.

<div class="note" markdown="1">
**What the equation does not do**

The equation is linear. It assumes the effect is the same at every concentration, that exposure is sustained, and that the population is comparable to the one the coefficient was estimated on. If a story leans heavily on any of these assumptions, it should say so.
</div>

## Minimum reporting checklist

Every post must state its:

1. Baseline year
2. Pollution target (WHO guideline, national standard, or policy commitment)
3. Geographic unit (such as district, state, or country)
4. Population-weighting method
5. PM<sub>2.5</sub> data source
6. Life expectancy coefficient
7. Uncertainty and caveats

A post that is missing any of these is a draft, not a finished piece.
