# Glide Range Explorer Pro ✈️

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)

## 🚀 Overview

**Glide Range Explorer Pro** is an advanced aviation physics simulator and emergency landing planner that calculates and visualizes aircraft glide ranges using real-world physics models. Whether you're a pilot, aviation enthusiast, student, or instructor, this tool provides comprehensive insights into aircraft gliding performance and emergency procedures.

### 🎯 Key Features

- **🛩️ Extensive Aircraft Database** - Commercial jets, general aviation, military aircraft, and high-performance gliders
- **🧮 Advanced Physics Modeling** - Real-world glide calculations with configuration effects, bank angles, and atmospheric conditions
- **🗺️ Interactive Mapping** - Live visualization of glide ranges with automatic airport detection
- **🌤️ Live Weather Integration** - Real-time wind data affecting glide performance
- **📚 Educational Content** - Comprehensive physics explanations and emergency procedures
- **📜 Historical Incidents** - Learn from famous emergency gliding events
- **🎮 Flight Path Simulation** - Animated visualization of glide trajectories
- **📱 Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices

## 🖼️ Screenshots

### Main Interface
The application features a modern, professional interface with dark-themed controls and a bright, clear map display:
- Left sidebar with comprehensive flight parameter controls
- Interactive map showing glide range and nearby airports
- Real-time calculation results and performance metrics

### Features in Action
- **Glide Range Visualization**: Blue circle showing maximum glide distance
- **Airport Detection**: Automatic identification of reachable airports
- **Historical Examples**: Famous emergency landings like the "Miracle on the Hudson"
- **Physics Education**: Detailed explanations of aerodynamic principles

## 🛠️ Installation

### Quick Start (Static Hosting)

1. **Download the HTML file**
```bash
wget https://raw.githubusercontent.com/yourusername/glide-explorer-pro/main/glide.html
```

2. **Open in any modern web browser**
```bash
open glide.html  # macOS
xdg-open glide.html  # Linux
start glide.html  # Windows
```

### Deploy to GitHub Pages

1. **Fork this repository**
2. **Enable GitHub Pages** in repository settings
3. **Select source branch** (usually `main`)
4. **Access your app** at `https://yourusername.github.io/glide-explorer-pro/`

### Local Development Server

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000/glide.html`

## 📖 Usage Guide

### Basic Operation

1. **Select Aircraft Type**
   - Choose from categories: Commercial, General Aviation, Military, or Gliders
   - Each aircraft has a specific L/D (Lift-to-Drag) ratio

2. **Set Flight Parameters**
   - **Altitude**: Starting height in feet (0-45,000 ft)
   - **Airspeed**: Indicated airspeed in knots
   - **Bank Angle**: Turning angle affecting sink rate
   - **Configuration**: Clean, gear down, or various flap settings

3. **Environmental Conditions**
   - **Wind**: Headwind (negative) or tailwind (positive) component
   - **Temperature**: ISA deviation affecting air density
   - **Atmosphere**: Standard, turbulent, or thermal conditions

4. **Calculate Glide Range**
   - Click "Calculate Glide Range" to see results
   - Map updates with glide circle and reachable airports
   - View detailed performance metrics

### Advanced Features

#### 🌍 Position Selection
- Enter coordinates manually
- Click on map to set position
- Use "Get My Location" for GPS positioning

#### 🌪️ Live Weather Mode
- Toggle "Advanced Weather Mode"
- Automatically fetches wind data from Open-Meteo API
- Calculates headwind/tailwind components

#### 📊 Historical Examples
- Click on famous incidents to load their parameters
- Map automatically centers on the historical flight path
- Learn from real emergency scenarios

#### ⌨️ Keyboard Shortcuts
- `Ctrl/Cmd + Enter`: Calculate glide range
- `Ctrl/Cmd + R`: Reset all parameters
- `Ctrl/Cmd + S`: Start flight simulation

## 🔬 Technical Details

### Physics Model

The application implements sophisticated aerodynamic calculations:

#### Basic Glide Equation
```
Glide Distance = (Altitude / 6076) × L/D × (Ground Speed / Airspeed)
```

#### Configuration Effects
- **Clean Configuration**: 100% L/D efficiency
- **Gear Extended**: 70% L/D efficiency  
- **Flaps 10°**: 85% L/D efficiency
- **Flaps 20°**: 75% L/D efficiency
- **Full Configuration**: 60% L/D efficiency

#### Bank Angle Effects
```
Effective L/D = Base L/D × cos(bank angle)
```
- 30° bank = 15% increase in sink rate
- 45° bank = 30% increase in sink rate

#### Density Altitude Corrections
```
True Airspeed = Indicated Airspeed × √(ρ₀/ρ)
```
Where ρ is air density at altitude

### Dependencies

- **[Leaflet.js](https://leafletjs.com/)** v1.9.4 - Interactive mapping
- **[OpenStreetMap](https://www.openstreetmap.org/)** - Map tiles and data
- **[Font Awesome](https://fontawesome.com/)** v6.4.0 - Icon library
- **[Open-Meteo API](https://open-meteo.com/)** - Weather data
- **[Overpass API](https://overpass-api.de/)** - Airport data

### Browser Compatibility

- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Opera 76+
- ⚠️ Internet Explorer (Not Supported)

## 🎓 Educational Value

### For Pilots
- Practice energy management concepts
- Understand glide performance factors
- Review emergency procedures
- Study historical incidents

### For Students
- Learn aerodynamic principles
- Visualize lift-to-drag relationships
- Explore environmental effects on flight
- Interactive physics demonstrations

### For Instructors
- Classroom demonstration tool
- Emergency procedure training
- Energy management teaching
- Historical case studies

## 📊 Aircraft Database

### Commercial Jets
| Aircraft | L/D Ratio | Best Glide Speed |
|----------|-----------|------------------|
| Boeing 737-800 | 15:1 | 210 knots |
| Boeing 757-200 | 16:1 | 220 knots |
| Airbus A320 | 17:1 | 240 knots |
| Boeing 777-300 | 18:1 | 260 knots |
| Boeing 787-9 | 19:1 | 250 knots |
| Airbus A350-900 | 20:1 | 255 knots |
| Boeing 747-8 | 21:1 | 270 knots |

### Historical Incidents Included
- **Air Transat 236** (2001) - 75-mile glide to Azores
- **Gimli Glider** (1983) - Metric conversion error
- **US Airways 1549** (2009) - Hudson River landing
- **TACA Flight 110** (1988) - Levee landing
- **British Airways 9** (1982) - Volcanic ash incident
- **Aloha Airlines 243** (1988) - Structural failure
- **Ethiopian Airlines 961** (1996) - Hijacking and ditching

## 🔧 API Configuration

### Open-Meteo Weather API
No API key required. Free tier includes:
- 10,000 requests/day
- Hourly weather data
- Wind speed and direction at multiple altitudes

### Overpass API
No API key required. Used for airport detection:
- OpenStreetMap data
- Real-time queries
- Aerodrome information

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

### Development Setup

1. Clone the repository
```bash
git clone https://github.com/yourusername/glide-explorer-pro.git
cd glide-explorer-pro
```

2. Make your changes

3. Test thoroughly in multiple browsers

4. Submit a pull request

### Areas for Contribution
- Additional aircraft types
- More historical incidents
- Enhanced physics models
- Multi-language support
- Performance optimizations
- Additional weather data sources

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Accelerate Solutions, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## ⚠️ Disclaimer

**IMPORTANT**: This tool is for **educational and training purposes only**. It should **NOT** be used for actual flight planning or emergency situations. Always consult official aircraft documentation, certified flight planning tools, and follow proper aviation procedures. The calculations provided are simplified models and may not account for all real-world factors.

## 🌟 Acknowledgments

- **OpenStreetMap Contributors** - Map data
- **Leaflet.js Team** - Mapping library
- **Aviation Safety Network** - Historical incident data
- **Open-Meteo** - Weather data API
- **Font Awesome** - Icon library
- **Aviation Community** - Technical guidance and feedback

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/yourusername/glide-explorer-pro/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/glide-explorer-pro/discussions)
- **Email**: support@acceleratesolutions.com
- **Documentation**: [Wiki](https://github.com/yourusername/glide-explorer-pro/wiki)

## 🚀 Roadmap

### Version 2.1 (Q2 2025)
- [ ] Terrain elevation analysis
- [ ] Multi-engine failure scenarios
- [ ] Export flight plans to PDF
- [ ] Mobile app development

### Version 2.2 (Q3 2025)
- [ ] 3D visualization mode
- [ ] Historical weather replay
- [ ] Pilot logbook integration
- [ ] Training mode with scenarios

### Version 3.0 (Q4 2025)
- [ ] AI-powered landing site recommendations
- [ ] Real-time ADS-B integration
- [ ] Multiplayer training sessions
- [ ] VR support for training

## 📈 Project Stats

- **Stars**: ![GitHub stars](https://img.shields.io/github/stars/yourusername/glide-explorer-pro)
- **Forks**: ![GitHub forks](https://img.shields.io/github/forks/yourusername/glide-explorer-pro)
- **Issues**: ![GitHub issues](https://img.shields.io/github/issues/yourusername/glide-explorer-pro)
- **Contributors**: ![GitHub contributors](https://img.shields.io/github/contributors/yourusername/glide-explorer-pro)

---

**Built with ❤️ by Accelerate Solutions, LLC**

*Making aviation safer through education and technology*
