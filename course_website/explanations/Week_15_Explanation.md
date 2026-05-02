# Week 15: Deployment & Serving Models

## Overview
A model is only valuable when it is used. This week focuses on the transition from training models to deploying them as scalable services that other applications can consume.

## Key Concepts
### 1. Serving Models with FastAPI
- **Production APIs**: `FastAPI` is a high-performance web framework designed for building modern, production-ready APIs. It is ideal for serving machine learning models due to its speed, support for asynchronous code, and automatic API documentation.
- **Model Serialization**: Packaging and loading pre-trained models using `pickle` or `joblib` is the standard way to deploy them into a live production environment.
