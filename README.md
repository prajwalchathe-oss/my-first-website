# Environment and Agriculture in India

An educational and informational website focused equally on the environment and agriculture of India. Designed with a modern, nature-inspired green-and-white theme, this platform serves students, farmers, researchers, and general citizens.

---

## 🏛️ Project Architecture

The project is strictly organized into two separate folders:

```text
Agriculture_portal/
├── backend/                  # Node.js & Express API Backend
│   ├── data/                 # Comprehensive datasets (Environment, Agriculture, Updates)
│   │   ├── environmentData.js
│   │   ├── agricultureData.js
│   │   └── updatesData.js
│   ├── routes/               # Express REST API routes
│   │   ├── environmentRoutes.js
│   │   ├── agricultureRoutes.js
│   │   └── updatesRoutes.js
│   ├── services/             # Modular API Integration Placeholders
│   │   └── placeholderApiIntegration.js
│   ├── package.json
│   └── server.js             # API Server (Port 5000)
│
└── frontend/                 # React.js Single Page Application (Vite)
    ├── public/
    ├── src/
    │   ├── components/       # Responsive UI components
    │   │   ├── Navbar.jsx
    │   │   ├── Hero.jsx
    │   │   ├── VitalRibbon.jsx
    │   │   ├── EnvironmentSection.jsx
    │   │   ├── AgricultureSection.jsx
    │   │   ├── UpdatesSection.jsx
    │   │   ├── EducationalHub.jsx
    │   │   ├── TopicDetailModal.jsx
    │   │   ├── ApiPlaceholderModal.jsx
    │   │   └── Footer.jsx
    │   ├── services/         # API Service & Client Mock Fallback
    │   │   ├── apiConfig.js
    │   │   ├── apiService.js
    │   │   └── mockData.js
    │   ├── App.jsx
    │   ├── index.css         # Nature-inspired Green & White Design System
    │   └── main.jsx
    ├── index.html
    ├── package.json
    └── vite.config.js
```

---

## 🌿 1. Environment of India (50% Focus)

1. **Forests and Wildlife**: 24.62% forest and tree cover (80.9 MHa), Project Tiger (3,682 wild tigers, 75% of global count), Western Ghats & Himalayan wildlife corridors, Nagar Van urban forests, and Wildlife Protection Act 1972.
2. **Biodiversity**: 4 global biodiversity hotspots (Western Ghats, Himalayas, Indo-Burma, Sundaland), 85 Ramsar protected wetlands, endemic flora/fauna, sacred groves (Orans, Devarakadus).
3. **Climate Change**: Monsoon variations, Himalayan cryosphere retreat, coastal resilience, and India's Panchamrit commitments (500 GW non-fossil by 2030, Net-Zero by 2070, Mission LiFE).
4. **Air and Water Pollution**: River basin health (Namami Gange), seasonal agricultural stubble management (Happy Seeders & bio-decomposers), NCAP clean air targets, and CPCB industrial standards.
5. **Natural Resources**: Fertile alluvial Indo-Gangetic plains, Deccan black regur soils, Red & Laterite profiles, groundwater overexploitation and recharge under Atal Bhujal Yojana.
6. **Renewable Energy**: 190+ GW non-fossil installed capacity, Ultra-Mega Solar Parks (Bhadla 2,245 MW), PM-KUSUM farmer solar pumps, wind energy corridors, and National Green Hydrogen Mission.

---

## 🌾 2. Agriculture in India (50% Focus)

1. **Types of Agriculture in India**: Subsistence farming, intensive cultivation, commercial plantations (tea, coffee, rubber, sugarcane), and Zero Budget Natural Farming (ZBNF) / 100% organic model (Sikkim).
2. **Major Crops**: Seasonal cropping cycles with interactive calendar:
   - **Kharif** (Monsoon: Rice, Cotton, Maize, Soybean, Bajra, Jowar).
   - **Rabi** (Winter: Wheat, Mustard, Gram, Barley, Peas).
   - **Zaid** (Summer: Watermelon, Cucumber, Summer Moong).
3. **Irrigation Methods**: Canal networks, tube wells, micro-irrigation (Drip & Sprinkler with 50-70% water savings), PMKSY "Per Drop More Crop", and community check-dam revival.
4. **Modern Farming**: Kisan Drones for precision foliar spraying, IoT wireless soil probes, hydroponics/vertical farming, climate-controlled polyhouses, and AI pest diagnostics.
5. **Government Schemes**: PM-KISAN (₹6,000 direct income transfer), PM Fasal Bima Yojana (crop loss shield), Soil Health Cards, and e-NAM pan-India electronic trading.
6. **Farmers’ Challenges**: Generational land fragmentation, monsoon dependency, market price volatility & middlemen, cold-chain post-harvest deficits, and FPO aggregation.

---

## 📡 3. Latest Updates & Live Trackers

- **Indian Environment News**: Curated policy and conservation updates (MoEFCC, CPCB, WII).
- **Indian Agriculture News**: Crop prices, ICAR climate-resilient seed releases, export policies.
- **Weather and Rainfall**: Regional breakdowns across North, South, Central, West, East, and Northeast India with monsoon departure and farmer field advisories.
- **Crop Market Prices (Mandi Bhav)**: Searchable APMC mandi commodity prices (Wheat, Paddy, Mustard, Cotton, Soybean, Onion) with Minimum Support Price (MSP) benchmarks and market trends.
- **Air Quality Index (AQI)**: Continuous CPCB National Air Quality Index (NAQI) monitor for major Indian cities (Delhi-NCR, Mumbai, Kolkata, Bengaluru, Lucknow, Patna, Hyderabad, Chennai) with color-coded severity meters and health advisories.

---

## 🔌 4. API Integration Placeholders Architecture

Per the project requirements, **no external APIs are connected yet**. Instead, dedicated, modular placeholder services with realistic, structured schemas are implemented:

| Module | Target Future API | Environment Variable | Status |
| :--- | :--- | :--- | :--- |
| **Weather & Rainfall** | India Meteorological Department (IMD) / OpenWeather | `WEATHER_API_KEY` | Placeholder Active (Simulated Schema) |
| **Crop Market Prices** | Agmarknet / data.gov.in e-NAM Daily Market Rates | `DATA_GOV_IN_API_KEY` | Placeholder Active (Simulated Schema) |
| **Air Quality Index** | CPCB CAAQMS / OpenAQ Global Air Quality API | `CPCB_AQI_API_KEY` | Placeholder Active (Simulated Schema) |
| **National News** | Press Information Bureau (PIB) RSS / NewsAPI | `NEWS_API_KEY` | Placeholder Active (Simulated Schema) |

- **Backend Controller**: `backend/services/placeholderApiIntegration.js`
- **Frontend Configuration**: `frontend/src/services/apiConfig.js`
- **Resilience**: The frontend includes a fallback layer (`apiService.js`), ensuring the entire website operates smoothly even when running as a standalone SPA without the backend.

---

## 🚀 Running the Project

### 1. Start the Backend API (Port 5000)
```bash
cd backend
npm install
npm start
```
The backend API will run on `http://localhost:5000/api`.

### 2. Start the Frontend Application (Port 3000)
```bash
cd frontend
npm install
npm run dev
```
Open your browser at `http://localhost:3000` to explore the website.
