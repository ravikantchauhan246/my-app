# Three.js Angular Application

A simple Angular application that demonstrates the integration of Three.js for 3D graphics. This application features an interactive 3D cube that rotates continuously and changes color when clicked.

## Features

- Interactive 3D cube with continuous rotation
- Color-changing functionality on click
- Orbit controls for camera manipulation (rotate, zoom, pan)
- Responsive design that adapts to window resizing
- Shadow effects for enhanced visual appeal

## Technologies Used

- Angular 17+
- Three.js
- TypeScript
- CSS

## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd my-app
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   ng serve
   ```

4. Open your browser and navigate to `http://localhost:4200/`

## Building for Production

To build the application for production:

```
npm run build
```

The build artifacts will be stored in the `dist/` directory.

## Usage

- **Rotate the view**: Click and drag with the mouse
- **Zoom in/out**: Use the mouse wheel
- **Change cube color**: Click on the cube

## Project Structure

- `src/app/scene/scene.component.ts`: Main component that handles the Three.js scene
- `src/app/app.component.html`: Main template with UI overlay
- `src/app/app.component.css`: Styles for the UI overlay

## Troubleshooting

### Common Issues

1. **OrbitControls Import Error**:
   If you encounter an error like:
   ```
   Could not resolve "three/examples/jsm/controls/OrbitControls"
   ```
   Make sure to include the `.js` extension in the import:
   ```typescript
   import { OrbitControls } from 'three/examples/jsm/controls/OrbitControls.js';
   ```

2. **Performance Issues**:
   - Reduce the complexity of the 3D objects
   - Lower the shadow map resolution
   - Disable antialiasing if needed

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Three.js community for the excellent documentation
- Angular team for the framework
