# UFO-Sighting
This project is a silly project made in data science I course. I have a thing for UFOs.

UFO Sightings Analysis and Prediction
Author: Nhu Nguyen Course: Data 133

This notebook/project explores the CORGIS UFO sightings dataset and performs simple data analysis and machine learning predictions on UFO locations.

Summary of what I did for this notebook:
Clean and flatten the dataset for easier analysis.
Perform exploratory data analysis (EDA) using statistics, unique values, and visualizations.
Generate interactive maps of UFO sightings in the US and specific regions
Build and evaluate a Random Forest Regressor to predict UFO latitude and longitude based on features like date, time, location, shape, and duration.
Visualize predicted UFO locations and trajectories with interactive Folium maps.
Compare predicted vs. actual sightings and explore intersections and hotspots.
Brief report:
Data cleaning & Cleaning

Flattened nested dictionaries into simple columns like shape, duration, city, state, country, and sighted/documented dates.
Checked for missing values and unique entries per column.
Data analysis -Find the most frequent value for each column -Found patterns using heatmap in different dataset attributes in the US in general and CA for specific

ML Prediction

Trained a Random Forest Regressor to predict latitude and longitude using features such as date, time, UFO shape, state, city, and duration.
Evaluated model performance:
RMSE ≈ 0.93° (~100 km)
R² = 0.988, meaning the model explains almost all patterns in the data.
Added predicted coordinates to the dataset for mapping and trajectory analysis.
Interactive mapping

Visualized actual sightings using Folium maps with clustering for dense areas.
Added interactive layers to toggle visibility of actual sightings, predicted locations, and connecting lines.
Interesting findings:

Most sightings occur in California, but Seattle is a notable city hotspot.
Latitude and longitude correlations are different across states, with California showing strong negative correlation not seen in the US as a whole.
