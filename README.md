

# Elevation Profile and Electric Motor Analysis

## Overview

This code analyzes elevation data for a route between municipalities near Cochabamba, Bolivia. It calculates the elevation profile, identifies steep uphill sections, curve points, and determines where an electric motor would require additional assistance. The output includes plots and a map visualization.

## How it Works

- Imports necessary Python libraries like matplotlib, numpy, scipy, geopy
- Loads elevation JSON data for the route 
- Converts GPS coordinates to meter units for distance calculation
- Computes elevation gain, distances between points and slope at each point
- Smooths the slope data using a Savitzky-Golay filter
- Identifies steep uphill sections based on smoothed slope and distance thresholds
- Suggests relay points every 10km along the route
- Calculates curvature at each point to find sharp curve points
- Generates plots for elevation profile, slope, steep sections and relay points
- Creates a Folium map with route, steep section, relay and curve points marked
- Provides functions to locate assistance points based on battery range limits 
- Helper functions for distance and curvature calculations

## Key Outputs

- Elevation profile plot with major towns labeled
- Slope plot showing raw and smoothed slope 
- Marked steep uphill segments needing motor assistance
- Suggested relay points for swapping batteries
- High curvature points identified
- Interactive Folium map with all route and points marked

## Usage

The code can be run as a Python script after installing the required libraries. JSON data for any route can be loaded and analyzed. The slope and distance thresholds for steep sections and relay points can be customized as needed.

