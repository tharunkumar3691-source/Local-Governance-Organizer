# 🏛️ Local Governance Organizer

A comprehensive web application providing city information, essential services, citizen interaction, and online civic support for local people.

**⚠️ IMPORTANT DISCLAIMER**: This app uses simulated city data for demonstration purposes only. All data, locations, services, and functionality are fictional and created for educational and portfolio purposes. This is not an official government service.

## 📋 Project Overview

The Local Governance Organizer is a modern, responsive web application built with React that serves as a civic engagement platform. It provides citizens with easy access to city information, emergency services, public issue reporting, and city analytics.

### Key Features

1. **🏙️ City Information Dashboard**
   - Display city name, population, area, and infrastructure counts
   - Welcome message and city overview
   - Key statistics at a glance

2. **🗺️ Interactive City Map**
   - Leaflet.js-powered interactive map
   - Markers for hospitals, fire stations, police stations, ambulance centers, schools, and services
   - Category filtering for easy navigation
   - Click markers to view details and contact information

3. **🚑 Emergency Services (Simulated)**
   - Quick access to ambulance services
   - Fire department contact and request system
   - Police station information and contact
   - Hospital listings with specialties
   - **Demo disclaimer clearly displayed**

4. **📋 Online Police Complaint System**
   - Guided form for filing complaints
   - Complaint type selection
   - Location and description input
   - Automatic reference number generation
   - Complaint status tracking

5. **💬 Public Local Problem Sharing**
   - Social civic feed for local issues
   - Categories: Road, Water, Garbage, Power, Other
   - Ward/area selection
   - Upvoting system to highlight important issues
   - No login required for MVP

6. **⭐ Essential Services & Shops**
   - Grocery stores listing
   - Medical stores/pharmacies
   - Emergency supplies
   - Star ratings and hours of operation
   - Contact and location information

7. **📊 City Analytics & Statistics**
   - Population growth graphs
   - Water supply vs demand analysis
   - Educational institutions distribution
   - Interactive charts using Recharts
   - Year-wise statistics and trends

## 🏗️ Project Structure

```
local-governance-organizer/
├── client/
│   ├── public/
│   │   └── data/
│   │       ├── city_profile.json
│   │       ├── population.csv
│   │       ├── hospitals.csv
│   │       ├── fire_stations.csv
│   │       ├── police_stations.csv
│   │       ├── schools_colleges.csv
│   │       ├── ambulance_centers.csv
│   │       ├── water_data.csv
│   │       └── services.csv
│   ├── src/
│   │   ├── pages/
│   │   │   ├── Home.tsx
│   │   │   ├── Map.tsx
│   │   │   ├── Services.tsx
│   │   │   ├── Report.tsx
│   │   │   ├── Issues.tsx
│   │   │   ├── Shops.tsx
│   │   │   └── Analytics.tsx
│   │   ├── components/
│   │   │   └── Navigation.tsx
│   │   ├── contexts/
│   │   │   └── CivicContext.tsx
│   │   ├── lib/
│   │   │   └── dataLoader.ts
│   │   ├── App.tsx
│   │   ├── main.tsx
│   │   └── index.css
│   └── index.html
├── package.json
└── README.md
```

## 🛠️ Tech Stack

- **Frontend Framework**: React 19 with TypeScript
- **Styling**: Tailwind CSS 4
- **Routing**: Wouter (lightweight client-side router)
- **Maps**: Leaflet.js with OpenStreetMap
- **Charts**: Recharts for data visualization
- **UI Components**: shadcn/ui
- **Build Tool**: Vite
- **Package Manager**: pnpm

## 📦 Fake City Data

### NovaCity Dataset

The application includes a complete simulated dataset for **NovaCity**:

- **Population**: 1.25 million (2024)
- **Area**: 450 sq km
- **Hospitals**: 5 medical facilities
- **Fire Stations**: 5 stations
- **Police Stations**: 5 precincts
- **Schools & Colleges**: 6 institutions
- **Ambulance Centers**: 5 centers
- **Essential Services**: 8 shops and services
- **Water Data**: Monthly supply and demand statistics

All data is loaded automatically from CSV and JSON files in the `/data/` folder.

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- pnpm (recommended) or npm

### Installation

1. **Clone or download the project**
   ```bash
   cd local-governance-organizer
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   # or
   npm install
   ```

3. **Start the development server**
   ```bash
   pnpm dev
   # or
   npm run dev
   ```

4. **Open in browser**
   - Navigate to `http://localhost:3000`
   - The app will automatically load all city data

### Building for Production

```bash
pnpm build
# or
npm run build
```

## 📱 Features in Detail

### 1. Dashboard (Home Page)
- City overview with key statistics
- Quick access buttons to all major features
- City information card with contact details
- Infrastructure summary

### 2. Interactive Map
- Real-time map powered by Leaflet.js
- Filter services by category
- Click markers for detailed information
- Responsive design for all devices

### 3. Emergency Services
- Location input for emergency requests
- Simulated emergency dispatch system
- Success confirmation messages
- Direct calling links to all services
- Hospital information with specialties

### 4. Police Complaint System
- Easy-to-use complaint form
- Multiple complaint type options
- Automatic reference number generation
- Complaint history display
- Status tracking

### 5. Public Issues Feed
- Create and share local problems
- Upvoting system for community support
- Category-based organization
- Ward/area tracking
- Real-time issue updates

### 6. Services & Shops
- Browse grocery stores, pharmacies, and emergency supplies
- Star ratings for each service
- Operating hours and contact information
- Category filtering
- Top-rated services section

### 7. Analytics Dashboard
- Population growth trends
- Water supply analysis
- Educational statistics
- Interactive charts and graphs
- Historical data visualization

## 🎨 UI/UX Design

- **Clean Government Style**: Professional, accessible interface
- **Mobile-Friendly**: Fully responsive design for all devices
- **Easy Navigation**: Simple top navigation bar
- **Color-Coded Categories**: Different colors for different service types
- **Clear Disclaimers**: Demo/simulation notices prominently displayed
- **Accessibility**: Keyboard navigation and screen reader support

## 🔐 Data & Privacy

- **Simulated Data Only**: All data is fictional for demonstration
- **No Real User Data**: No actual personal information is collected
- **Local Storage**: Data is managed in browser context
- **Demo System**: Not connected to real government systems

## 📊 Data Sources

All data is simulated and stored in the `/data/` folder:

- `city_profile.json`: City information and metadata
- `population.csv`: Year-wise population statistics
- `hospitals.csv`: Hospital locations and details
- `fire_stations.csv`: Fire station information
- `police_stations.csv`: Police precinct details
- `schools_colleges.csv`: Educational institutions
- `ambulance_centers.csv`: Ambulance service locations
- `water_data.csv`: Monthly water supply and demand
- `services.csv`: Essential services and shops

## 🔄 Data Loading

The application uses a custom data loader utility that:
1. Fetches CSV and JSON files from the `/data/` folder
2. Parses CSV data into structured objects
3. Provides TypeScript interfaces for type safety
4. Manages data through React Context API
5. Automatically loads all data on app startup

## 🎯 Use Cases

1. **Civic Engagement**: Citizens can report local issues and track their status
2. **Emergency Access**: Quick access to emergency services with location tracking
3. **Service Discovery**: Find hospitals, pharmacies, and essential services
4. **Public Complaints**: File police complaints with reference tracking
5. **City Analytics**: View city statistics and trends
6. **Community Support**: Upvote and support important local issues

## 🚨 Important Notes

- **This is a DEMO application** - Not for production use
- **All data is simulated** - No real government data
- **Emergency calls should use official numbers** - Always call 911 (or local emergency number) for real emergencies
- **Educational Purpose** - Built for learning and portfolio demonstration
- **No Official Status** - This is not an official government service

## 📈 Future Enhancements

- User authentication and profiles
- Real-time notifications
- Advanced filtering and search
- Mobile app version
- Multi-language support
- Integration with real government APIs
- Real-time issue tracking
- Community voting system
- Event calendar
- Budget transparency dashboard

## 🤝 Contributing

This is a demonstration project. For improvements or suggestions, please refer to the project requirements.

## 📄 License

This project is created for educational and portfolio purposes.

## 👨‍💻 Developer Notes

### Architecture Decisions

1. **React Context for State Management**: Chosen for simplicity and avoiding prop drilling
2. **Wouter for Routing**: Lightweight alternative to React Router
3. **Tailwind CSS**: Utility-first approach for rapid UI development
4. **Recharts**: Simple and effective charting library
5. **Leaflet.js**: Lightweight and feature-rich mapping solution

### Performance Considerations

- Data is loaded once on app startup
- CSV parsing is optimized for small datasets
- Images are lazy-loaded where applicable
- Responsive images for different screen sizes

### Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📞 Contact & Support

For questions about this demo application, refer to the project documentation.

---

**Created for: Local Governance Civic Tech Project**
**Version: 1.0.0**
**Last Updated: January 2026**

⚠️ **Remember: This is a DEMO system using simulated data for educational purposes only.**
