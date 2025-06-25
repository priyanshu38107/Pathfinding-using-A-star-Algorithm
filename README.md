# Pathfinding-using-A-star-Algorithm
PATH FINDING ROUTE PLANNER USING OSM A*(STAR) ALGORITHM
🚦 Mumbai Route Planner
An interactive route planning tool for Mumbai using OpenStreetMap data, allowing users to calculate and visualize optimal routes by shortest or fastest path. The planner supports both text-based and interactive map input, and also displays distance, estimated travel time, and elevation profile.

🌍 Features
Interactive Routing: Choose start and end points by typing location names or clicking directly on the map.

Shortest vs Fastest Routes: Select the optimization mode for your route.

POI Integration: Automatically displays nearby Points of Interest (POIs) along your route.

Elevation Profile: Visualize the elevation changes along your route.

Road Type Color Coding: Different road types are shown with distinct colors and estimated speeds.

Google Satellite and Multiple Map Layers: Switch between OpenStreetMap, Stamen Terrain, Google Satellite, and more.

Blocked Roads Detection: Automatically avoids roads marked as “blocked”.

🛣️ Road Type Legend
Road Type	Color	Speed (km/h)
Motorway	Red	60
Trunk	Dark Red	50
Primary	Orange	40
Secondary	Yellow	35
Tertiary	Light Green	30
Residential	Green	25
Unclassified	Gray	20

📌 How to Use
Option 1: Use Location Names
Enter Start and End locations in the input boxes.

Choose either Shortest or Fastest route.

Click Plan Route.

Option 2: Use Interactive Map
Click on the map:

First click sets Start

Second click sets End

Third click resets Start

The route will be updated automatically.

🧱 Technical Stack
Python

OSMnx – for street network data and routing

NetworkX – for graph-based route calculation (A* algorithm)

Folium – for interactive map visualization

Geopy – for location name to coordinate conversion

Matplotlib – for elevation plotting

Shapely – for bounding box geometry

IPython Widgets – for interactive controls in notebooks

📦 Setup Instructions
Clone the repository or copy the code into a Jupyter Notebook.

Install required packages:

bash
Copy
Edit
pip install osmnx networkx folium geopy shapely matplotlib ipywidgets
Run the notebook. If no graph file is found, it will automatically download data for the Mumbai area and save a .graphml file for faster future access.

📁 Files
mumbai_drive.graphml – Cached street network file for Mumbai

README.md – This file

📝 Notes
Make sure you're connected to the internet when geocoding or fetching map tiles.

Elevation data depends on the availability of elevation attributes in the OSM dataset or pre-processed nodes.
