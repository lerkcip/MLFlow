# MLFlow for GenAI Observability

## Overview

This project demonstrates how to implement MLFlow for monitoring and tracking the performance of GenAI applications, specifically those using OpenAI's GPT models. MLFlow provides a comprehensive framework for tracking experiments, logging metrics, and visualizing performance data, which is essential for understanding and optimizing AI-powered systems.

## Purpose

The primary goal of this project is to showcase how MLFlow can be used to:

1. Set up tracking for a GenAI application
2. Log important metrics like token counts, latency, and model parameters
3. Create an interactive chat application with the OpenAI API
4. Monitor the application's performance in real-time

## Features

- **Comprehensive Metric Tracking**: Monitors token usage, request latency, and model parameters
- **Dual Observability**: Uses both MLFlow for experiment tracking and Prometheus for real-time operational monitoring
- **Interactive Chat Interface**: Demonstrates MLFlow integration in a functional application
- **Visualization Tools**: Includes code for visualizing token usage and latency distributions

## Key Metrics Monitored

- **Request Latency**: Measures response time of the API
- **Token Usage**: Tracks prompt tokens, completion tokens, and total tokens
- **Request Count**: Monitors API call frequency
- **Model Parameters**: Logs configuration settings like temperature and top_p

## Implementation Details

The project uses:

- **OpenAI API**: For accessing GPT models
- **MLFlow**: For experiment tracking and metric logging
- **tiktoken**: For accurate token counting using OpenAI's tokenization algorithm
- **Prometheus Client**: For exposing metrics via HTTP endpoint for real-time monitoring
- **Pandas & Matplotlib**: For data analysis and visualization

## Benefits of MLFlow for GenAI

- **Centralized Monitoring**: All metrics stored in one accessible location
- **Experiment Tracking**: Systematic comparison of different configurations
- **Cost Management**: Detailed token usage tracking for API cost estimation
- **Performance Optimization**: Visualization of metrics to identify bottlenecks
- **Reproducibility**: All parameters and metrics systematically logged

## Getting Started

### Prerequisites

- Python 3.x
- OpenAI API key
- MLFlow server running locally or remotely

### Setup

1. Clone this repository
2. Install required dependencies: `pip install -r requirements.txt` (if available)
3. Set up your OpenAI API key in a `.env` file
4. Start the MLFlow server: `mlflow server`
5. Run the Jupyter notebook: `jupyter notebook "MLFlow Example.ipynb"`

## Usage

The main functionality is demonstrated in the Jupyter notebook `MLFlow Example.ipynb`. The notebook contains:

1. Setup code for MLFlow tracking and OpenAI API
2. An interactive chat application that logs metrics to MLFlow
3. Visualization code for analyzing token usage and latency
4. Detailed explanations of the implementation and benefits

## Conclusion

This project demonstrates a comprehensive approach to implementing MLFlow observability for GenAI applications. By tracking metrics such as token usage, request latency, and model parameters, it establishes a data-driven foundation for understanding and enhancing the performance, cost-efficiency, and reliability of language model deployments.

The integration of MLFlow with OpenAI's API represents a significant advancement in GenAI operational excellence, enabling teams to move beyond ad-hoc monitoring approaches toward systematic experimentation and continuous improvement.