# PCA-and-Clustering-on-Survey-Data

# Personality Archetype Analysis using PCA and k-Means

This repository contains a university project focused on leveraging dimensionality reduction and clustering techniques to analyze a survey dataset of young adults. The primary goal is to uncover "personality archetypes" distinct groups of individuals sharing similar traits, interests, and habits from a high-dimensional dataset.

## Project Overview

The analysis employs **Principal Component Analysis (PCA)** to distill numerous correlated variables (related to interests, phobias, spending habits, etc.) into a smaller set of meaningful, interpretable components. Subsequently, the **k-Means clustering algorithm** is applied to these components to segment the individuals into homogeneous groups, each representing a different personality archetype.

A key aspect of the project is a comparative analysis of two data preprocessing techniques, **StandardScaler** and **MinMaxScaler**, to assess their impact on the final clustering outcomes.

### Core Methodologies

*   **Data Cleaning and Preprocessing:** Handling missing values (NaNs) and encoding categorical features to prepare the data for analysis.
*   **Dimensionality Reduction:** Using PCA to extract the most significant latent features from the dataset.
*   **Clustering:** Applying the k-Means algorithm to identify distinct groups of individuals based on the principal components.
*   **Model Optimization:** Leveraging the **Silhouette Score** to determine the optimal number of clusters (`k`).
*   **Interpretation and Evaluation:** Analyzing cluster centroids to define archetypes and performing an external evaluation using original demographic labels (e.g., education level) to validate the findings.

## Key Findings

The analysis successfully identified several distinct personality archetypes within the dataset. The primary clusters identified include:

*   **The Pragmatists:** Individuals focused on the concrete aspects of life, with lower scores in spirituality and creativity.
*   **The Social Activists:** Highly extroverted and socially active individuals, often goal-oriented and engaged with their community.
*   **The Spiritual Seekers:** An introspective group interested in beauty, art, and spirituality over scientific knowledge.
*   **The Philosopher-Artists:** Creative and reflective individuals who are not materialistic or driven by conventional goals.

The comparison between `StandardScaler` and `MinMaxScaler` revealed that the choice of preprocessing technique can influence the optimal number of clusters and their final composition, underscoring the importance of this step in the analysis pipeline.


## Dataset

The dataset used, `responses_hw.csv`, it contains anonymized survey responses on a wide range of topics, including interests, habits, and personality traits.
