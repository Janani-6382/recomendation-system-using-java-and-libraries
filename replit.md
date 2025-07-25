# Java Recommendation System with Apache Mahout

## Overview

This is a Java-based recommendation system built using Apache Mahout that implements collaborative filtering algorithms. The system provides both user-based and item-based recommendation capabilities with built-in data generation, evaluation metrics, and an interactive console interface.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

The application follows a modular Java architecture centered around Apache Mahout's machine learning capabilities:

- **Core Language**: Java 11+
- **Build System**: Maven for dependency management and project building
- **ML Framework**: Apache Mahout for recommendation algorithms
- **Data Format**: CSV files for data input/output
- **Interface**: Command-line interactive console

## Key Components

### Recommendation Algorithms
- **User-Based Collaborative Filtering**: Finds users with similar preferences and recommends items they liked
- **Item-Based Collaborative Filtering**: Recommends items similar to those the user has previously rated highly
- Both algorithms use Mahout's built-in implementations for efficiency and reliability

### Data Management
- **Sample Data Generator**: Creates realistic test datasets for development and testing
- **CSV Data Loader**: Handles loading user ratings, item metadata, and user profiles from CSV files
- **Data Statistics Module**: Provides comprehensive analysis of dataset characteristics

### Evaluation System
- **Cross-Validation**: Splits data into training and test sets for algorithm validation
- **RMSE Calculation**: Root Mean Square Error metrics for measuring recommendation accuracy
- **Performance Benchmarking**: Built-in evaluation framework for comparing algorithm effectiveness

### User Interface
- **Interactive Console**: Command-line interface for real-time recommendation testing
- **Batch Processing**: Support for processing multiple recommendation requests

## Data Flow

1. **Data Ingestion**: CSV files containing user-item ratings are loaded into the system
2. **Data Preprocessing**: Raw data is transformed into Mahout-compatible format
3. **Model Training**: Collaborative filtering models are built using training data
4. **Recommendation Generation**: Trained models generate personalized recommendations
5. **Evaluation**: System validates recommendations using test data and RMSE metrics
6. **Output**: Recommendations are presented through the console interface

## External Dependencies

### Core Dependencies
- **Apache Mahout**: Primary machine learning library for recommendation algorithms
- **Maven**: Build automation and dependency management
- **Java Standard Library**: Core Java functionality

### Data Dependencies
- **CSV File Support**: Standard Java CSV parsing capabilities
- **File I/O**: Java NIO for efficient file operations

## Deployment Strategy

### Development Environment
- **Local Development**: Maven-based build system for local development
- **Command Line Execution**: Direct execution via Maven exec plugin
- **IDE Integration**: Standard Maven project structure for IDE compatibility

### Build and Run Process
1. **Compilation**: `mvn clean compile` to build the project
2. **Execution**: `mvn exec:java -Dexec.mainClass="com.recommendation.RecommendationApp"` to run
3. **Testing**: Built-in evaluation system for algorithm validation

### Scalability Considerations
- **Memory Management**: Mahout's efficient sparse matrix implementations for large datasets
- **Algorithm Selection**: Choice between user-based and item-based filtering based on data characteristics
- **Data Loading**: CSV-based approach allows for easy data updates and management

The system is designed for educational and prototype use, with a focus on demonstrating collaborative filtering concepts while maintaining code clarity and ease of use.