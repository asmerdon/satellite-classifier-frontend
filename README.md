# Satellite Classifier Frontend

This is the frontend for the Satellite Image Classifier — a web app that uses satellite imagery and a deep learning model to classify land types (e.g., forest, crops, sea, industrial, etc).

## How It Works
- A semi-transparent mask highlights the region being classified.
- When you click “Classify This Area,” the bounding box coordinates are sent to a backend API.
- The backend returns classification probabilities via a deep learning model trained on satellite imagery.
- Results are displayed as a bar chart on screen.

Note: The first request may take up to 50 seconds due to free-tier cold starts on Render.com.

## Mapbox Token
This project uses Mapbox’s satellite tiles. The API key is exposed in `index.html`, as it is only used for rendering tiles and does not provide access to any sensitive permissions.

## Backend
The classification model API is hosted separately at:
`https://earth-observation.onrender.com/predict/`

## Live Version


## Example Screenshot
(Optional: include a screenshot of the app in use if desired)
