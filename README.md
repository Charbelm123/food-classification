# Food Recommendation System

A machine learning-based food recommendation system that uses image classification and recipe analysis.

## Project Structure

- `data/` - Directory containing project data
- `Food Images/` - Directory containing food images for classification
- `Food Ingredients and Recipe Dataset with Image Name Mapping.csv` - Dataset mapping ingredients to recipes
- `food_classification.ipynb` - Jupyter notebook containing the classification model
- `docker-compose.yml` - Docker configuration for Weaviate vector database

## Setup

### Prerequisites

- Docker and Docker Compose
- Python with Jupyter Notebook
- Required Python packages (requirements.txt to be added)

### Vector Database Setup

The project uses Weaviate as a vector database with image recognition capabilities. To start the Weaviate services:

docker-compose up -d

This will start:

Weaviate server on port 8070
Image inference API using ResNet50 model

Environment Variables
The Weaviate configuration includes:
  Image inference API
  Anonymous access enabled
  img2vec-neural module for image vectorization
  CUDA disabled by default
Features
  Image-based food classification
  Recipe and ingredient mapping
  Vector similarity search
Usage
  1-Start the Weaviate services using Docker Compose
  2-Open food_classification.ipynb in Jupyter Notebook
  3-Follow the notebook instructions for classification and recommendations

API Endpoints
Weaviate API is available at:
  Main API: http://localhost:8070
  Image Inference API: http://localhost:8070
