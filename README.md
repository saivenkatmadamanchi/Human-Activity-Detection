# Human-Activity-Detection

This project explores various time series features for human activity monitoring using accelerometer data collected from 15 subjects engaged in four different activities: walking, running, climbing up, and climbing down. The analysis employs Natural Visibility Graph (NVG) and Horizontal Visibility Graph (HVG) methods to compute key metrics and uses permutation entropy and complexity for a detailed examination of the accelerometer data.

## Table of Contents

- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Methods](#methods)
  - [Visibility Graphs](#visibility-graphs)
    - [Natural Visibility Graph (NVG)](#natural-visibility-graph-nvg)
    - [Horizontal Visibility Graph (HVG)](#horizontal-visibility-graph-hvg)
  - [Permutation Entropy and Complexity](#permutation-entropy-and-complexity)
- [Parameters](#parameters)
- [Results](#results)
  - [Scatter Plots](#scatter-plots)
  - [Sample Output Tables](#sample-output-tables)
- [Conclusions](#conclusions)
- [Usage](#usage)
- [License](#license)

## Introduction

This project aims to provide insights into human activity patterns by analyzing accelerometer data through graph-based and entropy-based methods. By leveraging these techniques, we can comprehensively understand the characteristics and complexities of different human activities.

## Data Collection

Accelerometer data were collected from 15 subjects performing the following activities:
- Walking
- Running
- Climbing up
- Climbing down

Each activity's data consist of 1024 data points for analysis.

## Methods

### Visibility Graphs

#### Natural Visibility Graph (NVG)

The Natural Visibility Graph (NVG) method converts time series data into a graph where each data point becomes a node. Edges are created based on the visibility criteria between data points.

#### Horizontal Visibility Graph (HVG)

The Horizontal Visibility Graph (HVG) method is similar to NVG but uses horizontal visibility criteria for creating edges between nodes.

For both NVG and HVG, the following metrics are computed:
- Average degree
- Network diameter
- Average path length

### Permutation Entropy and Complexity

Permutation entropy and complexity provide a measure of the complexity and unpredictability of the time series data. The analysis involves varying parameters such as:
- Embedded dimension
- Embedded delay
- Signal length

## Parameters

The parameters for computing permutation entropy and complexity are:
- **Embedded Dimension**
- **Embedded Delay**
- **Signal Length**: 1024 data points

## Results

### Scatter Plots

Scatter plots are generated to visualize the relationships between:
- Average degree and network diameter, color-coded based on activities and methods (NVG and HVG)
- Permutation entropy and complexity, color-coded based on activities

### Sample Output Tables

The project includes sample output tables summarizing the computed metrics and their relationships for each activity and method.

## Conclusions

The analysis provides valuable insights into the distinguishing features of various human activities. The use of NVG and HVG methods, along with permutation entropy and complexity, allows for a detailed understanding of the underlying patterns in accelerometer data.

## Usage

To run the analysis, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/your-username/human-activity-monitoring.git
   ```
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Execute the main script:
   ```
   python main.py
   ```
4. Visualize the results using the provided scatter plots and output tables.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to the project by submitting issues or pull requests. For any questions, please contact [your-email@example.com](mailto:your-email@example.com).

---

**Note**: Update the parameter ranges, repository URL, and contact information as necessary.
