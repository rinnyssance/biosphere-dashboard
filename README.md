# Verde: A Biosphere Dashboard

A comprehensive environmental monitoring platform for the Hampton Roads region, featuring real-time climate data, interactive mapping, and biosphere analytics.

## Features

- 🌍 **Real-time Environmental Data** - Live climate and environmental metrics
- 🌡️ **Climate Monitoring** - Temperature trends and atmospheric data
- 🗺️ **Interactive Mapping** - Leaflet-based maps with temperature overlays
- 📊 **Data Visualization** - Charts and graphs for environmental insights

## Technology Stack

- **Frontend**: React 18 + TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS
- **Maps**: Leaflet + React-Leaflet
- **Charts**: Chart.js + React-Chartjs-2
- **API**: Open-Meteo (weather data)

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Deployment to Vercel

### Method 1: Vercel CLI (Recommended)

1. **Install Vercel CLI**:
   ```bash
   npm i -g vercel
   ```

2. **Login to Vercel**:
   ```bash
   vercel login
   ```

3. **Deploy from your project directory**:
   ```bash
   vercel
   ```

4. **Follow the prompts**:
   - Link to existing project? → No
   - Project name → `biosphere-dashboard` (or your preferred name)
   - Directory → `./` (current directory)
   - Override settings? → No

5. **Your app will be deployed** and you'll get a URL like `https://biosphere-dashboard-xxx.vercel.app`

### Method 2: GitHub Integration

1. **Push your code to GitHub**:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Go to [vercel.com](https://vercel.com)** and sign in

3. **Click "New Project"**

4. **Import your GitHub repository**

5. **Configure the project**:
   - Framework Preset: Vite
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`

6. **Click "Deploy"**

### Method 3: Drag & Drop

1. **Build your project**:
   ```bash
   npm run build
   ```

2. **Go to [vercel.com](https://vercel.com)**

3. **Drag and drop the `dist` folder** to the Vercel dashboard

## Environment Variables

No environment variables are required for this project as it uses public APIs.

## Project Structure

```
src/
├── components/
│   ├── TitleBanner.tsx    # Main title banner
│   ├── Navbar.tsx         # Navigation component
│   ├── Overview.tsx       # Overview dashboard
│   ├── Climate.tsx        # Climate monitoring
│   ├── Map.tsx           # Map container
│   ├── LeafletMap.tsx    # Interactive map
│   ├── TemperatureChart.tsx # Temperature charts
│   └── Footer.tsx        # Footer component
├── App.tsx               # Main app component
├── main.tsx             # App entry point
└── style.css            # Global styles
```

## API Usage

This project uses the Open-Meteo API for weather data:
- **Current Weather**: `https://api.open-meteo.com/v1/forecast`
- **Hourly Forecast**: `https://api.open-meteo.com/v1/forecast`
- **No API key required** - Free public API

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the MIT License.

---

**Developer**: Rinny  
**Location**: Hampton Roads, Virginia  
**Last Updated**: 2024

