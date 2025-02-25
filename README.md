# AI Pathfinding

## Overview
This repository contains the implementation of an Artificial and Computational Intelligence assignment focused on problem-solving through search algorithms. The project features two primary search strategies: **Uninformed Search** and **Informed Search**, specifically utilizing **Uniform Cost Search (UCS)** and **Recursive Best First Search (RBFS)** algorithms. The goal is to navigate a grid-based environment, accounting for dynamic costs and obstacles, while providing performance metrics and path visualization.

## Table of Contents
- [Project Description](#project-description)
- [Installation](#installation)
- [Usage](#usage)
- [Algorithms Implemented](#algorithms-implemented)
- [Performance Metrics](#performance-metrics)
- [Contributors](#contributors)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Description
The project aims to design a **Problem Solving Agent (PSA)** that can effectively navigate a grid environment. The agent is tasked with finding the optimal path from a starting point to a goal point while considering various obstacles, such as buildings and blocked paths. The implementation includes:

- **Dynamic Cost Calculations**: The agent evaluates the cost of movement based on the current state of the environment.
- **Path Visualization**: The project provides visual feedback on the paths taken by the agent, allowing for better understanding and analysis of the search algorithms.
- **Performance Metrics**: The project tracks and displays various performance metrics, including total cost, expanded nodes, and execution time for each algorithm.

## Installation
To run the code in this repository, ensure you have Python installed on your machine. Follow these steps to set up the environment:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/SaurabhJalendra/AI-Pathfinding.git
   ```

2. **Install Required Packages**:
   It is recommended to use a virtual environment. You can create one using `venv` or `conda`. After activating your environment, install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Jupyter Notebook**:
   Ensure you have Jupyter Notebook installed. If not, you can install it using:
   ```bash
   pip install notebook
   ```

## Usage
1. **Open the Jupyter Notebook**:
   Launch Jupyter Notebook from the command line:
   ```bash
   jupyter notebook "PS1_Group1_ACI_Assignment.ipynb"
   ```

2. **Run the Notebook**:
   Follow the instructions in the notebook to execute the code cells. The notebook is structured to guide you through the process of setting up the environment, defining the grid, and invoking the search algorithms.

3. **Dynamic Input Handling**:
   The code is designed to handle dynamic inputs for the starting and goal positions, allowing for flexible testing of different scenarios.

4. **Visual Output**:
   The notebook will display the grid, the paths taken by the agent, and the performance metrics for each algorithm.

## Algorithms Implemented
### 1. Recursive Best First Search (RBFS)
- **Description**: RBFS is an informed search algorithm that uses recursion to explore paths. It maintains a limited memory footprint by discarding paths that are not promising based on heuristic evaluations.
- **Key Features**:
  - Utilizes a heuristic function to guide the search.
  - Backtracks when a path exceeds the cost of the best alternative path.
  - Efficient for smaller grids but may struggle with larger, more complex environments.

### 2. Uniform Cost Search (UCS)
- **Description**: UCS is an uninformed search algorithm that expands the least costly node first. It guarantees finding the optimal path by evaluating all possible paths based on cumulative costs.
- **Key Features**:
  - Maintains a priority queue to manage nodes based on their cost.
  - Consistently provides the shortest path but may require more memory to store expanded nodes.
  - Effective in densely populated grids with numerous obstacles.

## Performance Metrics
The project tracks and displays the following performance metrics for each algorithm:
- **Total Cost**: The cumulative cost of the path taken by the agent.
- **Expanded Nodes**: The number of nodes that were expanded during the search process.
- **Execution Time**: The time taken to find the solution, measured in seconds.

These metrics are printed at the end of each algorithm's execution, providing insights into the efficiency and effectiveness of the search strategies.

## Contributors
- **Reddy Balaji .C** (BITS ID: 2023AC05862; Email: 2023ac05862@wilp.bits-pilani.ac.in)
- **Saurabh Jalendra** (BITS ID: 2023AC05912; Email: 2023ac05912@wilp.bits-pilani.ac.in)
- **Tushar Shandilya** (BITS ID: 2023AC05573; Email: 2023ac05573@wilp.bits-pilani.ac.in)
- **Bandana Kumari** (BITS ID: 2023AC05879; Email: 2023ac05879@wilp.bits-pilani.ac.in)
- **Monica Malik** (BITS ID: 2023AC05875; Email: 2023ac05875@wilp.bits-pilani.ac.in)

## Acknowledgments
- Special thanks to the instructors and peers for their support and guidance throughout this assignment.
- Acknowledgment to the authors of the libraries and resources utilized in this project.

---

Feel free to modify any sections to better fit your project's specifics or to add any additional information that may be relevant! This README aims to provide a comprehensive understanding of the project, making it easier for users to navigate and utilize the repository effectively.
