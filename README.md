# Little Afternoon ☀️

**A quiet little escape.**

Little Afternoon is a cozy, interactive 3D room exploration experience built with HTML, CSS, JavaScript, and Three.js.

Step into a peaceful bedroom filled with warm afternoon sunlight, wooden furniture, soft fabrics, plants, books, and little things worth noticing. Explore the room at your own pace, interact with everyday objects, and discover five small comforts hidden throughout the space.

No objectives to rush through. No pressure. Just a little moment to yourself.

## ✨ Features

- **Immersive 3D Environment** — Explore a detailed bedroom with cozy furniture, decorations, and interior elements.
- **Warm Afternoon Atmosphere** — Soft lighting, shadows, atmospheric fog, and floating dust particles.
- **Interactive Objects** — Discover small interactions throughout the room, each with its own message.
- **Five Hidden Comforts** — Find five special objects scattered around the room.
- **Dynamic Lighting** — Toggle the bedside lamp on and off.
- **First-Person Exploration** — Walk freely and look around using keyboard and mouse controls.
- **Touchscreen Support** — Navigate with on-screen directional buttons and touch gestures.
- **Procedural Textures** — Wood grain and fabric textures generated using HTML Canvas.
- **Responsive Rendering** — The 3D scene adapts to browser window resizing.

## 🛠️ Built With

- HTML5
- CSS3
- JavaScript (ES Modules)
- [Three.js](https://threejs.org/)
- [Google Fonts](https://fonts.google.com/)

## 🚀 Getting Started

### Prerequisites

- A modern web browser with WebGL support.
- An internet connection to load Three.js and Google Fonts from their CDNs.
- Python 3, Node.js, or Visual Studio Code with the Live Server extension to run a local server.

No additional packages or build tools are required for the project itself.

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/web-animation-3d.git
```

Replace `YOUR_USERNAME` with your GitHub username.

**2. Navigate to the project directory**

```bash
cd web-animation-3d
```

**3. Verify the project structure**

```text
web-animation-3d/
└── index.html
```

The `index.html` file contains the complete application, including the HTML structure, CSS styling, 3D scene, controls, interactions, and animation logic.

**4. Start a local development server**

Using Python:

```bash
python3 -m http.server 8000
```

Or using Node.js:

```bash
npx serve .
```

You can also open the project folder in Visual Studio Code and use the Live Server extension.

**5. Open the experience**

For the Python server, visit:

```text
http://localhost:8000
```

Click **Step inside →** to enter the room and start exploring.

## 🎮 Controls

### Desktop

| Input | Action |
|---|---|
| `W` / `↑` | Move forward |
| `S` / `↓` | Move backward |
| `A` / `←` | Move left |
| `D` / `→` | Move right |
| Mouse | Look around |
| `E` | Interact with objects |
| `Shift` | Move faster |
| `Esc` | Release mouse control and return to the overlay |

### Mobile and Touchscreens

- Use the on-screen arrow buttons to move.
- Drag across the scene to look around.
- Tap the **E** button to interact with objects.

## 🧸 Discover the Five Comforts

Explore the room and interact with five special objects.

| Object | Interaction |
|---|---|
| Teddy Bear | Say hello to the bear |
| Notebook | Read the little notebook |
| Tea Cup | Enjoy a quiet cup of tea |
| Cookie | Take a little cookie |
| Ceramic Bunny | Admire the ceramic bunny |

Look directly at an object and move close enough for its interaction prompt to appear. Press `E` or tap the on-screen interaction button to interact.

Each discovery displays a short message and updates the discovery counter. Finding all five comforts triggers a final message.

## 🪴 Additional Interactions

Other interactive elements include:

- **Bedside Lamp** — Toggle the warm bedside light.
- **Bedroom Door** — Interact with the door to display a message.

Little Afternoon is designed as a relaxing exploration experience rather than a traditional level-based game.

## 🎨 Visual Design

The visual style features a warm, muted palette inspired by cozy interiors and late-afternoon sunlight.

- Cream and beige surfaces.
- Natural oak and dark wood.
- Sage-green textiles and plants.
- Soft pink accents.
- Warm amber lighting.
- Atmospheric fog and subtle vignette shading.

Procedural textures add detail to wooden surfaces, fabrics, and walls without requiring external texture files.

## ⚙️ Technical Details

### 3D Rendering

The project uses Three.js for real-time 3D rendering, including:

- Perspective camera.
- WebGL renderer with antialiasing.
- ACES Filmic tone mapping.
- Soft shadow mapping.
- Hemisphere, directional, and point lighting.
- Atmospheric fog.
- Procedural canvas textures.

### Movement and Collision

Player movement is relative to the camera's viewing direction. Simple collision boundaries prevent the player from walking through registered furniture and beyond the room's boundaries.

### Interaction System

A raycaster detects objects near the center of the screen. When an interactive object is within range and is not blocked by another opaque object, an interaction prompt appears.

### Animation

The animation loop updates player movement, subtle camera motion, floating dust particles, object selection, and scene rendering.

## 📁 Project Structure

```text
web-animation-3d/
├── index.html
└── README.md
```

The project is self-contained. No separate assets directory, package installation, or compilation step is required.

## 🌐 Deployment

This is a static web project and can be deployed to any compatible static hosting provider.

- [GitHub Pages](https://pages.github.com/)
- [Netlify](https://www.netlify.com/)
- [Vercel](https://vercel.com/)

Upload or connect the repository and configure the deployment to serve `index.html` from the project root.

No backend, database, or server-side runtime is required.

**Note:** Serve the project over HTTP or HTTPS rather than opening the file directly with `file://`, because the application imports Three.js as an ES module through an import map.

## 🐛 Troubleshooting

### The room does not load

- Check your internet connection.
- Ensure that your browser supports WebGL.
- Run the project through a local development server.
- Check the browser developer console for JavaScript errors.

### The screen is blank

- Verify that the Three.js CDN is accessible.
- Try a modern browser with hardware acceleration enabled.
- Check for WebGL or JavaScript errors in the developer console.

### Mouse controls are not working

- Click **Step inside →** to activate mouse pointer lock.
- If pointer lock is unavailable, try dragging across the scene.
- Browser security settings may restrict pointer lock in certain contexts.

### Touch controls are missing

Touch controls rely on the CSS `pointer: coarse` media query. Some devices or browser configurations may not trigger this detection.

### Performance is slow

- Close unnecessary browser tabs.
- Use a device with hardware-accelerated WebGL support.
- Consider reducing rendering resolution or shadow quality if you modify the source code.

## 📜 License

No license is currently specified in the project source. Add a `LICENSE` file if you intend to define permissions for using, modifying, and redistributing the project.

## 💛 The Idea

Not every digital experience needs to be competitive, fast, or demanding.

Sometimes, it is enough to walk into a quiet room, notice the sunlight, make a cup of tea, and stay a little longer.

**Stay a little.**
