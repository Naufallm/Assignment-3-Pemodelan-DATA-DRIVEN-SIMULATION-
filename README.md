# Airline Queuing System Analysis Report

## Overview
This repository contains the analysis and simulation of a hypothetical airline queuing system based on customer data derived from an airline service satisfaction survey. The project aims to optimize waiting times, queue performance, and customer satisfaction using Python and data visualization techniques.

## Date
- **Generated On:** March 18, 2025

## Purpose
The primary objective is to analyze the queuing system by simulating customer arrival and service processes, focusing on the following key metrics:
- Waiting times
- Queue length over time
- Server utilization
- Customer satisfaction correlation with waiting times
- Departure delays categorized by travel class (Business, Eco, Eco Plus)

## Data
The dataset consists of 25,976 customer records with the following variables:
- **Arrival Delay in Minutes**: Used as inter-arrival times for customers.
- **Departure Delay in Minutes**: Used as service times for processing customers.
- **Satisfaction**: Binary classification (1 for "satisfied", 0 for "neutral or dissatisfied").
- **Class**: Travel class categories (Business, Eco, Eco Plus).

## Methodology
### Tools and Libraries
- **Python 3.11.9**: Programming language for data analysis and simulation.
- **Matplotlib**: Used for generating visualizations such as boxplots and scatter plots.
- **Pandas**: Utilized for data manipulation and analysis.

### Simulation Approach
- The analysis employs an M/M/c queuing model, initially with a single server and later extended to a two-server model (M/M/2).
- Data is processed to simulate customer arrivals and service times, with performance metrics calculated and visualized.

## Key Findings
1. **Efficiency**: The system handles 25,976 customers with minimal waiting times and queue lengths, supported by a 60% server utilization rate.
2. **Class Disparity**: Business class exhibits the lowest median departure delay (near 0) with outliers up to 1,000 minutes, while Eco and Eco Plus classes show higher median delays and wider spreads.
3. **Satisfaction Analysis**: The correlation between waiting time and satisfaction is unclear due to a lack of discernible data distribution in the scatter plot, suggesting a need for further investigation into additional variables.
4. **Optimization**: Adding a second server reduces the average waiting time to approximately 0.05 minutes, significantly enhancing system efficiency.

## Visualizations
- **Boxplot (Departure Delay by Class)**: Displays the distribution of departure delays across Business, Eco, and Eco Plus classes, highlighting priority service for Business class.
- **Scatter Plot (Satisfaction vs. Waiting Time)**: Intended to show the relationship between waiting times and satisfaction, but currently lacks clear data distribution (potential visualization error).

## Recommendations
1. **Multi-Server Implementation**: Deploy a two-server system during peak hours to maintain waiting times below 0.05 minutes.
2. **Priority Queue**: Continue prioritizing Business class and consider extending benefits to frequent flyers in other classes.
3. **Enhanced Satisfaction Analysis**: Re-evaluate satisfaction data with additional variables (e.g., service quality) to identify key drivers.
4. **Dynamic Management**: Monitor queue length and utilization to adjust server allocation dynamically.

## Conclusion
The queuing system demonstrates high efficiency with low waiting times and queue lengths, further improved by a two-server model. Business class benefits from reduced delays, while satisfaction analysis requires deeper exploration. Implementing the recommendations will enhance operational efficiency and customer satisfaction.

## Usage
To replicate the analysis:
1. Ensure Python 3.11.9 and required libraries (Pandas, Matplotlib) are installed.
2. Run the provided Jupyter Notebook cell to generate the boxplot visualization.
3. Adjust the dataset or code as needed to regenerate the scatter plot for satisfaction vs. waiting time.
