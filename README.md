# SolarVerse VR

### Interactive 3D Solar System Explorer

SolarVerse VR is an interactive **3D Solar System and VR experience** built using **React, Three.js, and React Three Fiber**.

The project allows users to explore the Sun and all eight planets in an immersive space environment, inspect planetary information, control the Solar System simulation, explore individual planets, and enter an immersive **WebXR VR experience** on supported devices.

> Developed as an academic AR/VR project.

---

## Features

### Interactive Solar System

- Complete Solar System with the **Sun + 8 planets**
- Real-time planetary rotation
- Planetary revolution around the Sun
- Independent orbital and rotation speeds
- Educational visual scaling for better exploration

### Detailed Planets

Each planet has its own visual appearance and characteristics:

- Mercury
- Venus
- Earth
- Mars
- Jupiter
- Saturn
- Uranus
- Neptune

The project uses procedural textures to create distinct planetary surfaces without relying on external texture downloads.

### Earth & Moon

- Detailed Earth surface
- Oceans and continents
- Cloud layer
- Orbiting Moon
- Independent Moon movement

### Major Moons

The project includes several important natural satellites.

**Jupiter**
- Io
- Europa
- Ganymede
- Callisto

**Saturn**
- Titan

### Saturn's Ring System

Saturn features a detailed 3D ring system with:

- Multiple ringlets
- Tilted ring geometry
- Semi-transparent materials
- Cassini Division

### Space Environment

- Multi-layer starfield
- Deep-space background
- Dynamic lighting
- Glowing Sun
- Atmospheric effects

### Camera & Exploration

Users can:

- Rotate around the Solar System
- Zoom in/out
- Pan
- Select individual planets
- Focus the camera on a planet
- Explore planets in close-up mode
- Return to the complete Solar System view

### Simulation Controls

Control the Solar System simulation with:

- Pause / Resume
- 0.5x speed
- 1x speed
- 2x speed
- 5x speed
- 10x speed

Additional controls:

- Show/Hide orbital paths
- Show/Hide planet labels
- Reset camera view

### Planet Information

Selecting a planet displays educational information including:

- Planet type
- Diameter
- Distance from the Sun
- Number of moons
- Orbital period
- Rotation period
- Average temperature
- Description
- Interesting facts

### WebXR VR

SolarVerse VR supports immersive **WebXR VR** on compatible devices.

Users can:

- Enter immersive VR
- Explore the Solar System in 6DoF
- Look around the virtual environment
- Inspect planets
- Use the spatial VR information panel

If VR is unavailable, the application automatically provides a desktop-mode fallback.

---

## Tech Stack

| Technology | Purpose |
|---|---|
| React | User interface and application structure |
| Vite | Development and build tooling |
| Three.js | 3D rendering |
| React Three Fiber | React renderer for Three.js |
| @react-three/drei | 3D helpers and utilities |
| WebXR | Immersive VR |
| CSS | UI styling and responsive layout |

---

## Project Structure

```text
SolarVerse VR/
│
├── public/
│
├── src/
│   ├── components/
│   │   ├── SolarSystem/
│   │   │   ├── SolarSystem.jsx
│   │   │   ├── Sun.jsx
│   │   │   ├── Planet.jsx
│   │   │   ├── Moon.jsx
│   │   │   ├── SaturnRings.jsx
│   │   │   ├── OrbitPath.jsx
│   │   │   ├── PlanetLabel.jsx
│   │   │   └── SpaceBackground.jsx
│   │   │
│   │   └── UI/
│   │       ├── IntroScreen.jsx
│   │       ├── LoadingScreen.jsx
│   │       ├── Header.jsx
│   │       ├── PlanetSelector.jsx
│   │       ├── PlanetInfo.jsx
│   │       ├── ControlPanel.jsx
│   │       └── VRModal.jsx
│   │
│   ├── data/
│   │   └── planets.js
│   │
│   ├── textures/
│   │   └── proceduralTextures.js
│   │
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
│
├── index.html
├── package.json
└── README.md
```

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/solarverse-vr.git
```

### 2. Navigate to the Project

```bash
cd solarverse-vr
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Start the Development Server

```bash
npm run dev
```

The application will be available at:

```text
http://localhost:5173
```

### 5. Build for Production

```bash
npm run build
```

---

## Testing VR

For VR testing:

1. Connect a compatible VR headset.
2. Open the application using a WebXR-compatible browser.
3. Launch SolarVerse VR.
4. Click **ENTER VR**.
5. Enter immersive mode.
6. Explore the Solar System.

Compatible environments may include:

- Meta Quest Browser
- Chrome with compatible WebXR hardware
- Microsoft Edge with compatible WebXR hardware
- Other WebXR-compatible environments

### Without a VR Headset

You can still use the complete **Desktop 3D Mode**.

If immersive VR is unavailable, SolarVerse VR provides a fallback message and allows you to continue using the normal 3D experience.

---

## Controls

### Desktop

| Action | Control |
|---|---|
| Rotate Camera | Mouse drag |
| Zoom | Mouse wheel |
| Pan | Mouse/right drag |
| Select Planet | Click planet |
| Explore Planet | Explore Planet button |
| Pause Simulation | Pause button |
| Change Speed | Speed controls |
| Show/Hide Orbits | Orbit toggle |
| Show/Hide Labels | Label toggle
