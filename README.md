# � Rescue Robo - Emergency Response Pathfinding Visualizer

An interactive educational tool that visualizes pathfinding algorithms (Greedy Best-First Search + Backtracking) to solve a Traveling Salesman Problem variant: finding the optimal rescue route from a helicopter launch point through multiple survivor locations to a hospital in a disaster zone.

## ✨ Features

- 🎨 **Interactive Map Editor**: Design custom grid maps with walls, treasures, start and goal points
- 🔍 **Real-time Visualization**: Watch algorithms explore the map step-by-step
- 📊 **Live Metrics**: Track distance, treasures collected, nodes explored, and permutations tested
- 🎯 **Optimal Path Finding**: Uses Greedy Best-First Search + Backtracking optimization
- 📱 **Fully Responsive**: Works on desktop, tablet, and mobile devices
- 🎓 **Educational**: Perfect for learning pathfinding and optimization algorithms

## 🌐 Live Demo

**Access the app**: [https://rescue-robo-daa-solver.netlify.app](https://rescue-robo-daa-solver.netlify.app)

Works on:
- 💻 Desktop (Windows, Mac, Linux)
- 📱 Mobile (Android, iOS)
- 🖥️ Any device with a modern web browser

## 🛠️ Tech Stack

- **Frontend**: React 18 + TypeScript + Vite
- **Styling**: TailwindCSS 3 + Radix UI
- **Routing**: React Router 6
- **Algorithms**: Greedy Best-First Search (A*), Backtracking
- **Canvas**: HTML5 Canvas for grid visualization

## 📋 Prerequisites

Before running this project locally, ensure you have:

1. **Node.js** (v18 or higher) - [Download here](https://nodejs.org/)
2. **PNPM** (Package Manager) - Install: `npm install -g pnpm`
3. **Git** (optional) - [Download here](https://git-scm.com/)

## 🏃 Running Locally

### 1. Clone the repository

```bash
git clone https://github.com/your-username/rescue-robo.git
cd rescue-robo
```

### 2. Install dependencies
```bash
pnpm install
```

### 3. Start development server
```bash
pnpm dev
```

### 4. Open in browser
- **On PC**: Navigate to `http://localhost:8080`
- **On Mobile** (same WiFi network):
  1. Find your PC's IP address:
     - Windows: `ipconfig` (look for IPv4 Address)
     - Mac/Linux: `ifconfig` or `ip addr`
  2. On mobile browser: `http://<YOUR_PC_IP>:8080`
     - Example: `http://192.168.1.100:8080`

## 📦 Available Scripts

```bash
pnpm dev        # Start dev server (port 8080)
pnpm build      # Build for production
pnpm start      # Run production server
pnpm typecheck  # TypeScript validation
pnpm test       # Run tests
```

## 🌐 Deployment

### Deploy to Netlify (Recommended - FREE)

1. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "Ready for deployment"
   git push origin main
   ```

2. **Deploy on Netlify**:
   - Go to [netlify.com](https://netlify.com)
   - Sign up/Login (can use GitHub account)
   - Click "Add new site" → "Import an existing project"
   - Connect to GitHub and select this repository
   - Netlify auto-detects settings from `netlify.toml`
   - Click "Deploy"

3. **Get your link**:
   - You'll receive a URL like: `https://rescue-robo-algo.netlify.app`
   - Share this link with anyone - works on all devices!

### Alternative: Deploy to Vercel

```bash
# Install Vercel CLI
pnpm install -g vercel

# Deploy
vercel
```

## 🎮 How to Use

1. **Home Page**: Learn about the project and algorithms
2. **Editor Page**: 
   - Use the tool palette to place Helicopter (�), Hospital (�), Survivors (🆘), and Debris (🧱)
   - Click "Random Map" for a quick start
   - Click "Run Simulation" when ready
3. **Simulation Page**:
   - Watch the algorithm explore and find the optimal path
   - Control playback speed
   - View real-time metrics
4. **Results Page**:
   - See the optimal path visualization
   - Review performance statistics
   - Check survivor rescue order

## 🧠 Algorithms Used

### 1. Greedy Best-First Search (Preprocessing Phase)
- Finds shortest paths between all key points (helicopter, survivors, hospital)
- Uses Manhattan distance heuristic
- Visualized with blue-tinted cells showing exploration

### 2. Backtracking (Optimization Phase)
- Explores all permutations of survivor rescue orders
- Finds the optimal sequence that minimizes total distance
- Tracks and displays the number of routes tested

### 3. Path Execution
- Constructs complete path from ordered route segments
- Animates explorer movement with purple→pink gradient path

## 🎨 Color Scheme

- **Light Theme**: Purple and pink gradient palette
- 🚩 **Start**: Green
- 🎯 **Goal**: Red
- 🆘 **Survivor**: Amber
- 🧱 **Wall**: Brick texture
- 📍 **Path**: Purple→Pink gradient

## 📁 Project Structure

```
rescue-robo/
├── client/              # React frontend
│   ├── pages/          # Route components
│   ├── components/     # Reusable components
│   └── utils/          # Utility functions
├── server/             # Express backend (minimal)
├── shared/             # Shared types & algorithms
│   ├── types.ts       # Position, Grid, Cell types
│   └── algorithms.ts  # RescueRobotSolver
└── netlify/           # Netlify deployment config
```

## 🤝 Contributing

This is an educational project for DAA (Design & Analysis of Algorithms) lab. Feel free to:
- Report bugs
- Suggest improvements
- Fork and experiment

## 📝 License

MIT License - See [LICENSE](LICENSE) file for details

## 👨‍💻 Author

**Siddhesh Bisen**
- GitHub: [@siddhesh17b](https://github.com/siddhesh17b)
- Project Repository: [rescue-robo](https://github.com/your-username/rescue-robo)

Created as part of Design & Analysis of Algorithms coursework

## 🙏 Acknowledgments

- Built with [Fusion Starter](https://github.com/fusion-starter) template
- UI components from [Radix UI](https://www.radix-ui.com/)
- Icons from [Lucide React](https://lucide.dev/)

---

**🌟 Star this repo if you found it helpful!**
