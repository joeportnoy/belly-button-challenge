# Belly Button Biodiversity Dashboard

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [D3 + Plotly Visualizations](#d3--plotly-visualizations)

## Overview

This interactive dashboard explores the *Belly Button Biodiversity* dataset, cataloging the microbial species that inhabit human navels. The project utilizes JavaScript, D3, and Plotly to visualize the data and dynamically update the charts and demographic information based on user input.

Explore the live dashboard on [GitHub Pages](https://joeportnoy.github.io/belly-button-challenge/).

---

## Project Structure

```
belly-button-challenge/
│
├── static/
│   ├── css/
│   └── js/
│       └── app.js        # Main JavaScript logic
│
├── index.html            # Dashboard HTML layout
├── samples.json          # Provided sample dataset (not accessed locally)
├── README.md             # Project documentation
```

---

## D3 + Plotly Visualizations

- **Bar Chart**: Displays the top 10 OTUs found in a selected individual's navel.
  - X-axis: `sample_values`
  - Y-axis: `otu_ids` (formatted as `OTU <id>`)
  - Hover Text: `otu_labels`

- **Bubble Chart**: Visualizes all OTUs for a selected sample.
  - X-axis: `otu_ids`
  - Y-axis: `sample_values`
  - Marker size: `sample_values`
  - Marker color: `otu_ids`
  - Hover Text: `otu_labels`

- **Demographic Panel**: Displays metadata for the selected individual.
  - Uses key-value pairs from the metadata object to populate HTML elements dynamically.

---

## Deployment

The website is deployed via GitHub Pages and is accessible here:  
[https://joeportnoy.github.io/belly-button-challenge/](https://joeportnoy.github.io/belly-button-challenge/)