# Exosky - Exoplanets and Stars Visualization

**Exosky** is a 3D interactive visualization of exoplanets and stars built using [Three.js](https://threejs.org/). This project maps real astronomical data, such as the coordinates of stars and exoplanets, into a virtual 3D space, allowing users to explore these celestial bodies in an immersive environment. You can zoom, rotate, and navigate through the stars and planets, and retrieve detailed information about individual celestial objects by clicking on them or selecting them from the sidebar.

## Features

- **Interactive 3D visualization** of stars and exoplanets.
- Displays **real-world astronomical data** (e.g., right ascension, declination, distance).
- Allows users to **click on planets or stars** to view detailed information.
- **Sidebar** for quick selection and focus on specific exoplanets.
- Supports **centering the camera** on specific celestial objects.

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/yourusername/exosky.git
    cd exosky
    npm install
    ```

2. Install a simple HTTP server if you don't have one installed. If you have Python installed, run:
   
   ```bash
    # $ python -m http.server 8080
    ```
   OR
    ```bash
    # npx vite
    ```

5. Open your browser and navigate to `http://localhost:8080/`. The visualization should load in the browser window.

## Usage

- **Navigation:** Use your mouse to rotate around the scene. Zoom in and out using your scroll wheel. Hold the left mouse button to rotate the camera.
- **Sidebar:** The sidebar contains a list of exoplanets. Clicking on a planet name will automatically move the camera to its position in the scene.
- **Info Panel:** Clicking on a star or planet in the scene will display details such as right ascension (RA), declination (DEC), and distance (if available).

## Technologies

- **Three.js**: A cross-browser JavaScript library used to create and display animated 3D graphics.
- **JavaScript/ES6 Modules**: Used for structuring the app and handling logic.
- **HTML5 & CSS3**: For basic styling and structure.
- **Python (optional)**: Used to run a simple HTTP server for local development.

## How to build

No build process is required since the project is purely front-end. Simply run the project in a browser using a local server (e.g., python -m http.server) as shown in the installation steps.

If you'd like to extend the project or update data files:

- **Data Update**: Replace the exoplanets.json or stars.json files with updated datasets that follow the same structure (right ascension, declination, magnitude, distance, etc.).

## Data Sources

- **Exoplanet Data**: The exoplanet data is sourced from the NASA Exoplanet Archive.
- **Star Data**: The star data is sourced from the Gaia Archive.
