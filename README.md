WebGL Demo Page

This project is a final WebGL demo page created for VK 8.  
It brings together the WebGL, AR, and VR experiments done during the course into a single webpage.

## Features

- **ModelViewer**
  - Displays a GLB 3D model
  - Supports camera controls and auto-rotation
  - Includes AR support on compatible devices

- **three.js Scene**
  - Custom three.js scene rendered inside the page
  - Lighting (Hemisphere + Directional light)
  - Ground plane and animated object
  - GLB model loaded using GLTFLoader
  - OrbitControls for interaction
  - WebXR / VR support using VRButton

## Project Structure

index.html
model-viewer.min.js
models/
mymodel.glb


## How to Run Locally

Because WebGL modules and ModelViewer require an HTTP server, the project should not be opened using `file://`.

### Option 1: VS Code Live Server
1. Open the project folder in Visual Studio Code
2. Right-click `index.html`
3. Select **Open with Live Server**

### Option 2: Python HTTP Server
```bash
python -m http.server 8000

Then open:

http://localhost:8000

Notes

WebXR / VR features require a compatible browser and device.

A VR emulator extension may show informational messages in the console, which is normal.

The project focuses on functionality rather than visual design.