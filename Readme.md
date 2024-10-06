Exosky - Exoplanets and Stars Visualization

Exosky is a 3D interactive visualization of exoplanets and stars using Three.js. The project maps the real coordinates of stars and exoplanets into a virtual 3D space, allowing users to explore astronomical data in an immersive environment. You can zoom, rotate, and navigate through the stars and planets, and retrieve detailed information about individual celestial bodies by clicking on them or selecting them from the sidebar.
Features

    Interactive 3D visualization of stars and exoplanets.
    Displays real-world astronomical data (e.g., right ascension, declination, distance).
    Allows users to click on planets or stars to view detailed information.
    Sidebar to quickly select and focus on specific exoplanets.
    Smooth camera controls using WASD keys, mouse, and zoom capabilities.
    Supports centering the camera on specific celestial objects.

Installation

    Clone the repository to your local machine:

    bash

git clone https://github.com/yourusername/exosky.git
cd exosky

Install a simple HTTP server if you don't have one installed. If you have Python installed, run:

bash

python -m http.server 8080

Run the server in the root folder of the project:

bash

    python -m http.server 8080

    Open your browser and navigate to http://localhost:8080/. The visualization should load in the browser window.

Usage

    Navigation: Use your mouse to rotate around the scene. Zoom in and out using your scroll wheel. Hold the left mouse button to rotate the camera.
    Movement: You can use W (forward), A (left), S (backward), and D (right) to move around the scene.
    Sidebar: The sidebar contains a list of exoplanets. Clicking on a planet name will automatically move the camera to its position in the scene.
    Info Panel: When clicking on a star or planet in the scene, the information panel will display details like right ascension (RA), declination (DEC), and distance (if available).

Project Structure

bash

exosky/
├── index.html          # Main HTML file to load the app
├── style.css           # Styling for the UI and elements
├── exoplanets.json     # JSON file with exoplanet data
├── stars.json          # JSON file with star data
├── js/                 # Directory for JavaScript modules
│   ├── three.module.js # Three.js main library
│   └── controls.js     # Orbit controls for camera navigation
└── README.md           # This README file

Technologies

    Three.js: A cross-browser JavaScript library used to create and display animated 3D graphics.
    JavaScript/ES6 Modules: Used for structuring the app and handling logic.
    HTML5 & CSS3: Basic styling and structure for the project.
    Python (optional): Used to run a simple HTTP server for local development.

How to Build

No build process is required since the project is purely front-end. Simply run the project in a browser using a local server (e.g., python -m http.server) as shown in the installation steps.

If you'd like to extend the project or change data files:

    Data Update: Replace the exoplanets.json or stars.json files with updated datasets that follow the same structure (right ascension, declination, magnitude, distance, etc.).
    Customization: Modify the index.html and js/controls.js files if you want to add custom features such as UI improvements or new camera controls.

Data Sources

    Exoplanets Data: The exoplanet data is sourced from the NASA Exoplanet Archive.
    Stars Data: The star data is sourced from the Gaia Archive.

Feel free to explore, contribute, and suggest improvements for Exosky!