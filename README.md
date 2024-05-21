# Flood Monitoring Android Application
## Table of Contents
1. [Abstract](#abstract)
2. [Introduction](#introduction)
3. [Problem Statement](#problem-statement)
4. [Project Objectives](#project-objectives)
5. [Methodology](#methodology)
6. [System Architecture](#system-architecture)
7. [Implementation](#implementation)
8. [Results and Evaluation](#results-and-evaluation)
9. [Future Work](#future-work)
10. [Conclusion](#conclusion)
11. [References](#references)
12. [Setup and Usage](#setup-and-usage)

## Abstract
This project is an Android application designed to monitor water levels in real-time using an ESP32 sensor connected to an ultrasonic sensor. The app fetches water level data from ThingSpeak, displays various related metrics, and notifies users of potential flood risks. Key features include real-time data visualization, flood risk assessment, and user notifications.

## Introduction
This project demonstrates an application of object-oriented programming in developing an Android application for flood monitoring. By leveraging Java, Android Studio, and various APIs, the project showcases a practical approach to building a real-time monitoring system.

## Problem Statement
Flooding is a significant natural disaster that causes immense damage to property and life. Early warning systems are crucial to mitigate these effects. This project aims to develop a mobile application that provides real-time flood monitoring and alerts to users, helping them take timely action.

## Project Objectives
Monitor water levels using an ESP32 sensor.
Display real-time water level data and trends.
Assess flood risk and notify users of potential dangers.
Show weather information and sensor status.
Ensure the application runs in the background and notifies users even when closed.

## Methodology
The project uses Java and Android Studio for application development. The ESP32 sensor sends data to ThingSpeak, which is then fetched by the app. Various APIs are used for weather information and real-time data updates. The app's architecture follows the principles of modularity and separation of concerns.

## System Architecture
The architecture consists of the following components:

### MainActivity: 
Manages the user interface and fragment transactions.
WaterLevelUpdateReceiver: 
Receives broadcast intents for water level updates.
### Fragments: 
Different fragments handle specific functionalities like weather display, directions, emergency contacts, safety information, and home display.
### ThingSpeakClient: 
Fetches data from ThingSpeak.
### WaterLevelService: 
Monitors water levels in the background and sends notifications.

## Implementation
### MainActivity.java: 
Handles fragment management and UI initialization.
### WaterLevelUpdateReceiver.java: 
Listens for water level update broadcasts.
### ThingSpeakClient.java: 
Manages data fetching from ThingSpeak.
### WaterLevelService.java: 
Runs in the background to monitor water levels and notify users.
### Fragments: 
Individual fragments for different sections of the app.

## Results and Evaluation
The application successfully monitors water levels and alerts users in case of potential flooding. Screenshots of the main modules and error handling mechanisms demonstrate the app's functionality and robustness.

## Future Work
Integrate more sophisticated flood prediction algorithms.
Enhance UI/UX for better user interaction.
Expand support for multiple sensors.
Implement additional notification channels (e.g., SMS, email).
Conclusion
The flood monitoring application provides a practical solution for real-time flood detection and alerting. The project demonstrates effective use of object-oriented programming, API integration, and background services in Android development.

## Clone the repository:
git clone https://github.com/Saahil-Shahzad/FloodEarlyWarningSystem.git
cd flood-monitoring-app
Home Fragment: Displays water levels and sensor status.
Weather Fragment: Shows weather information.
Directions Fragment: Provides navigation directions.
Emergency Fragment: Lists emergency contacts.
Safety Fragment: Displays safety tips and information.
