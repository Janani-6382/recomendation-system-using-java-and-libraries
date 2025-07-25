# Java Recommendation System with Apache Mahout

A comprehensive recommendation system built with Java and Apache Mahout, implementing both user-based and item-based collaborative filtering algorithms.

## Features

- **User-Based Collaborative Filtering**: Recommends items based on similar users' preferences
- **Item-Based Collaborative Filtering**: Recommends items similar to those the user has liked
- **Sample Data Generation**: Automatically generates realistic sample data for testing
- **CSV Data Loading**: Load user, item, and rating data from CSV files
- **Evaluation Metrics**: Built-in evaluation using cross-validation and RMSE
- **Interactive Console**: Command-line interface for testing recommendations
- **Data Statistics**: Comprehensive data analysis and statistics

## Prerequisites

- Java 11 or higher
- Maven 3.6 or higher

## Installation and Setup

1. Clone or download this project
2. Navigate to the project directory
3. Build the project:
   ```bash
   mvn clean compile
   ```

## Running the Application

To run the recommendation system:

```bash
mvn exec:java -Dexec.mainClass="com.recommendation.RecommendationApp"
