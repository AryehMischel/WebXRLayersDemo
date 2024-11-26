# WebXR Layers Demo

This project demonstrates the use of the WebXR Layer API in an interactive Three.js scene. The demo showcases how to render high-quality stereo images using compressed GPU textures, targeting Meta hardware but with potential for cross-device compatibility using the Basis Universal intermediate file format. If interested in seeing how this developed here is my main [repo](https://github.com/AryehMischel/WebXRLayers-Playground) for experimenting with the WebXR Layers API.

## Features

- **WebXR Layer API**: Utilizes the WebXR Layer API to render high-quality stereo images.
- **Three.js Integration**: Leverages Three.js for 3D rendering and scene management.
- **Interactive Elements**: Includes interactive elements using the `InteractiveGroup` from Three.js.
- **Compressed GPU Textures**: Demonstrates the use of compressed GPU textures for efficient rendering.
- **Polyfill Support**: Includes a polyfill for broader WebXR support.

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/AryehMischel/WebXRLayersDemo
   cd WebXRLayersDemo
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

### Running the Project

1. Build the project:
   ```sh
   npm run build
   ```

2. Start the development server:
   ```sh
   npm start
   ```

3. Open your browser and navigate to `http://localhost:3000` to view the demo.

## Project Structure

- `server.js`: Entry point for the application.  
- `public/app.js`: Main application logic, including scene setup and WebXR layer management.
- `public/index.html`: Main HTML file for the demo.
- `bundled file can be found on the build branch`


## Usage

- **WebXR Layers**: The demo uses "WebXR__Layer" classes for managing and interacting with the underlying Composite Layers supplied by the WebXR API. In this demo we are just using the "WebXRQuadUILayer" and the "WebXRCubeLayerASTC", but there are classes for all layer types.
- **Three.js Scene**: The scene is set up with various Three.js components, including a camera, XR Controllers, raycasting, OrbitControls, lights, and other interactive elements.
- **Polyfill**: A polyfill is included to ensure broader compatibility with devices that support WebXR.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the ISC License.

## Acknowledgements

- [Three.js](https://threejs.org/)
- [WebXR API](https://immersiveweb.dev/)
- [Basis Universal](https://github.com/BinomialLLC/basis_universal)

