---
layout: post
title: "Stroke Prediction with FastAPI: Deploying My First ML Model 🚀🌐"
date: 2026-05-04
categories: [Machine Learning, Database Systems]
tags: [MLProject, FastAPI, DrBilalAhmad, MLwithDrBilalAhmad, Python, ComputerEngineering, UETLahore, LearningJourney, RandomForest, StrokePrediction]
---

![FastAPI ML](https://images.unsplash.com/photo-1677442135703-1787eea5ce01?w=800)

If someone had told me at the start of my first year at UET Lahore Faisalabad Campus that I would deploy a machine learning model that predicts stroke risk in human beings — I would not have believed them. But that is exactly what happened.

## Introduction 🎯

Building a machine learning model is only part of the journey. A model sitting inside a Jupyter Notebook cannot help anyone. This realization became the starting point of one of the most exciting phases of my learning — deploying my stroke prediction model using FastAPI.

## The Dataset 🏥

The dataset contained genuinely important health attributes:

- **Hypertension** — does the patient have high blood pressure?
- **Heart Disease** — any existing heart conditions?
- **Age and Gender** — basic demographic information
- **Work Type** — government, private, or self-employed?
- **Avg Glucose Level** — blood sugar levels
- **BMI** — body mass index
- **Smoking Status** — current, former, or never smoked?
- **Ever Married** — marital status
- **Residence Type** — urban or rural?

## The NeuroGuard Web Interface 🖥️

We built a complete web application called **NeuroGuard — Stroke Risk Predictor**:

![NeuroGuard Interface](https://images.unsplash.com/photo-1559028012-481c04fa702d?w=800)

The interface allowed users to:
1. Enter patient clinical and demographic details
2. Click **Analyse Risk**
3. Get instant stroke risk prediction

## Building the ML Model 🤖

### The Algorithm — Random Forest

The model we built was a **Random Forest Classification** model. Random Forest works by building multiple decision trees and combining their outputs — making it more accurate than a single decision tree alone.

### Training Process

1. Loading and preprocessing the dataset
2. Splitting data into training and testing sets
3. Training the Random Forest model
4. Evaluating accuracy and performance
5. Saving the model using Joblib

## Deploying with FastAPI ⚡

### What Is FastAPI?

FastAPI is a modern, high-performance Python framework for building APIs. It allowed me to:

- Create API endpoints
- Receive data from the frontend
- Pass data to the ML model
- Return predictions to the user

### The Application Workflow

1. User enters health information on the webpage
2. Frontend collects the data
3. Data is sent to FastAPI via an API call
4. FastAPI passes the data to the trained ML model
5. The model analyzes the features and generates a prediction
6. The prediction is returned as a response
7. The user sees the stroke risk result on screen

## The Database Design 🗄️

We also designed a complete database for the project with proper ER diagram and normalized tables including:

- **Patient** table
- **HealthMetrics** table
- **MedicalHistory** table
- **Lifestyle** table
- **Genders, WorkTypes, SmokingStatuses, ResidenceTypes** lookup tables

## Dr. Bilal Ahmad's Guidance 👨‍🏫

Dr. Bilal Ahmad guided us fully throughout the entire project. He made sure we understood why each step existed, what it was doing, and how it contributed to the final model. That deeper understanding is what separates someone who can follow instructions from someone who can actually think like a data scientist.

## Final Reflection #

When the application finally ran — when I entered health data into the interface and saw the model return a prediction in real time — the happiness I felt was something I cannot fully describe.

Dr. Bilal Ahmad always says that the goal is not just to learn — it is to **build things that matter**. This project was proof that even as first year students, we are capable of building things that matter.

#MLProject #FastAPI #DrBilalAhmad #MLwithDrBilalAhmad #Python #ComputerEngineering #UETLahore #LearningJourney #RandomForest #StrokePrediction
