---
title: Capacity expansion of storage over nodal wholesale market
summary: I show here how to carefully select a battery's site and size with respect to its influence on prices and congestion.
tags:
  - Optimization
  - Electricity Markets
date: '2023-11-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by Karsten Würth on Unsplash
  focal_point: Smart

links:
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

This blog post builds upon the insights from our [detailed article](content/publication/goujard-2021-optimal/index.md) and an accompanying Jupyter notebook, which can be found at [this GitHub repository](https://github.com/GuillaumeGoujard/LMP_NZ/blob/master/jupyter_notebook/notebook.ipynb). The purpose of this overview is to present the main results and highlights of our project, which focuses on the strategic placement and operation of battery storage systems in nodal wholesale electricity markets.

## Abstract
The market for battery storage is rapidly expanding due to factors such as falling battery costs and the need for flexible renewable energy generation. This study presents a new approach for maximizing the profitability of a battery storage system in a nodal wholesale market by optimizing its siting, size, and bidding schedule. We introduce a price-maker mixed-integer optimization framework and compare its effectiveness with traditional price-taker models. Our results, based on simulations using New Zealand's market data, highlight the importance of considering market influence in battery operation strategies.

## 1. Introduction
### Background & Motivation
Growing demand for grid-scale batteries in energy markets, influenced by factors like cost reduction of technology and increased renewable energy penetration.

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


![Alternative Text for Image 1](image1.jpg)
*Caption for Image 1*
