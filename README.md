# Glide Range Explorer Pro ✈️

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

An aviation physics simulator that calculates and visualizes aircraft glide ranges using real-world physics models. 


## ✨ Features

- **🛩️ 20+ Aircraft Models** - Commercial jets, GA aircraft, military, and gliders
- **📐 Real Physics** - L/D ratios, bank angles, configuration effects, density altitude
- **🗺️ Interactive Map** - Live glide range visualization with airport detection
- **🌤️ Live Weather** - Real-time wind data integration
- **📚 Educational Content** - Comprehensive physics explanations
- **📜 Historical Examples** - Learn from famous emergency landings (Hudson River, Gimli Glider, etc.)
- **📱 Responsive Design** - Works on all devices


## 📖 Usage

1. **Select Aircraft** - Choose from various categories and models
2. **Set Parameters** - Altitude, airspeed, wind, configuration
3. **Click Calculate** - View glide range circle and reachable airports
4. **Explore Examples** - Load historical emergency landing scenarios

### Keyboard Shortcuts
- `Ctrl/Cmd + Enter` - Calculate glide range
- `Ctrl/Cmd + R` - Reset all
- `Ctrl/Cmd + S` - Simulate flight

## 🔬 Physics Model

```
Glide Distance = (Altitude / 6076) × L/D × (Ground Speed / Airspeed)
```

**Configuration Effects:**
- Clean: 100% | Gear Down: 70% | Flaps: 60-85%

**Bank Angle:** 
- Effective L/D = Base L/D × cos(bank angle)

## 🛠️ Technical Stack

- **Frontend:** Pure HTML5, CSS3, JavaScript (no framework dependencies)
- **Mapping:** Leaflet.js + OpenStreetMap
- **Weather:** Open-Meteo API (no key required)
- **Airports:** Overpass API
- **Icons:** Font Awesome

## 📊 Aircraft Examples

| Aircraft | L/D Ratio | Best Glide |
|----------|-----------|------------|
| Boeing 737 | 15:1 | 210 kts |
| Airbus A320 | 17:1 | 240 kts |
| Boeing 787 | 19:1 | 250 kts |
| Cessna 172 | 9:1 | 65 kts |
| High-Performance Glider | 60:1 | 55 kts |


## 📄 License

MIT License - Copyright (c) 2025 Accelerate Solutions, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies.


## 🌟 Acknowledgments

- OpenStreetMap contributors
- Leaflet.js team  
- Aviation Safety Network for incident data
- Open-Meteo for weather API

---

**Created by Accelerate Solutions, LLC using GPT-5 and Claude Opus 4.1**
