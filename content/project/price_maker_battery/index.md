---
title: Capacity expansion of storage over nodal wholesale market
summary: A guide to optimizing battery placement and size to maximize revenue over a nodal wholesale market.
tags:
  - Optimization
  - Electricity Markets
date: '2023-11-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by Karsten Würth on Unsplash
  focal_point: Smart

---

This blog post builds upon the insights from our [detailed article](publication/goujard-2021-optimal/) and an accompanying Jupyter notebook, which can be found at [this GitHub repository](https://github.com/GuillaumeGoujard/LMP_NZ/blob/master/jupyter_notebook/notebook.ipynb). The purpose of this overview is to present the main results and highlights of our project, which focuses on the strategic placement and operation of battery storage systems in nodal wholesale electricity markets.

In this blog post, we're exploring the smart way to choose where and how big a transmission scale battery should be. Finding the perfect spot and size that can help alleviate congestion while benefiting from high electricity prices. I'll guide you through the factors that make a location ideal for battery placement and the right battery size to maximize revenues.

Hopefully, you'll come away with an understanding of how these decisions impact the energy market and grid congestion. Whether you're in the energy industry, a student, or just curious about how power markets work, you'll find some neat insights on making the grid smarter. Let's dive in!

## Battery storages make prices in congested markets

The fundamental rule in power grid balancing is that generation must equal consumption at every moment in time. It's a delicate game where every kilowatt consumed must be precisely matched by a kilowatt produced. Wholesale electricity markets exist to organize this temporal matching between multiple agents. They ensure that for every time step—usually measured in hours or even minutes—the supply meets the demand.

Participants in these markets, ranging from large-scale utility companies to smaller independent producers, submit bids. Demand bids represent the maximum price consumers are willing to pay for power, while supply offers indicate the lowest price at which producers are willing to sell their generated electricity. These bids are plotted on a graph: the demand curve slopes downwards, reflecting the willingness to purchase less at higher prices; the supply curve, conversely, slopes upwards, indicating a readiness to sell more at higher prices.

![Alternative Text for Image 1](supply_demand.png)
*Discharge (1) and charge (2) effects on prices on single node market*

In the wholesale electricity market, the role of a battery as either a 'price-taker' or 'price-maker' hinges on its influence over the market clearing price. A price-taker is an agent whose bids are too small to sway the overall market prices—like a single drop in an ocean. However, when the bid volumes are significant, the agent wields enough power to impact the prices, thus becoming a price-maker. For instance, in congested areas of the grid, where there's a bottleneck in power supply, even small bids from a battery can significantly affect the local prices, elevating the battery's role to that of a price-maker. This is because it can adjust the supply-demand balance by either injecting or withdrawing energy, which, respectively, lowers or raises the market clearing price. The figure you referred to illustrates this effect: a battery discharging lowers the price, while charging increases it, underscoring the battery’s capability to tilt the scale of market prices in either direction.

### Research Focus
Examining the profitability of battery storage at the transmission level in a nodal wholesale market, considering the battery as a price-maker during congestion periods.

## 2. Problem Formulation
### Battery Storage Problem
We consider a standalone battery at the transmission level in a nodal market. The goals are to identify optimal siting, capacity, and bidding strategy.

### Key Constraints
Storage charge level (SCL) constraints, charging rate limits, and a linear model for charge profile.

## 3. Nodal Wholesale Market Model
### Key Components
Describes the network topology, demand characteristics, generator specifications, and the economic dispatch process.

### Economic Dispatch
Outlines how market operators dispatch generation and storage to meet demand while minimizing costs.

## 4. Optimization Framework
### Price-Maker vs Price-Taker Framework
Differentiates between the two approaches in terms of market influence and bidding strategy.

### Mathematical Program under Equilibrium Constraints
Presents a mixed-integer linear program formulation for profit maximization under the price-maker assumption.

## 5. Case Study: New Zealand Energy Market
### Scenario Setup
Uses data and network characteristics from the New Zealand Energy Market for simulation.

### Results & Discussion
Presents findings on optimal battery siting and capacity under price-maker conditions. Highlights the influence of battery operation on market prices and profitability.

## 6. Conclusion
### Significance of Findings
Emphasizes the importance of market-aware approaches in battery storage optimization, especially in nodal wholesale markets.

### Future Research Directions
Suggests further exploration into the impact of large-scale battery storage on market dynamics and social welfare.

## Plots
[Include main plots from the LaTeX file, focusing on market price variations, battery operation strategies, and profitability comparisons.]



