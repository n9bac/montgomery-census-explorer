# Montgomery County Spatial Analysis

A real-time demographic mapping application that dynamically joins US Census Bureau ACS 5-Year estimates with TIGER/Line shapefiles for Montgomery County, Alabama.

## 🚀 Overview

This project demonstrates a seamless integration of spatial geometry and demographic data. It fetches GeoJSON tract boundaries from the TIGERweb REST API and merges them on-the-fly with socioeconomic variables (Income, Age, Population, Education) from the Census ACS API.

## ✨ Features

- **Dynamic Data Joining**: Merges disparate API sources (TIGER/Line + ACS) in the browser using GEOID matching.
- **Interactive Choropleth**: Visualizes Median Household Income across census tracts with custom color scales.
- **Rich Tooltips**: Hover over any tract to see detailed statistics:
  - Median Household Income
  - Median Age
  - Total Population
  - Educational Attainment (% Bachelor's Degree)
- **Responsive UI**: Built with Tailwind CSS for a modern, clean, and professional aesthetic.
- **Optimized Map Rendering**: Uses memoization and stable initialization patterns to ensure a smooth Leaflet experience.

## 🛠️ Tech Stack

- **Frontend**: React 19, TypeScript
- **Mapping**: Leaflet, React-Leaflet
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **Data Sources**: 
  - [US Census Bureau ACS 5-Year API (2022)](https://www.census.gov/data/developers/data-sets/acs-5year.html)
  - [TIGERweb REST Services](https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_restmapservice.html)

## 🚦 Getting Started

### Prerequisites

- Node.js (v18+)
- npm

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## 📝 Note for Mentors

The application features two "Load Data" buttons to optimize the user experience:
- **The Central CTA**: Provides a clear starting point for first-time users when the map is empty.
- **The Header Button**: Offers a persistent utility access point that remains visible throughout the session.

---
*Developed for the Hackathon - March 2026*
