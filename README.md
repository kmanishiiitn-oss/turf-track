# ⚽ Soccer Map Explorer

An interactive web application that helps you discover soccer teams and their match histories through an intuitive map interface. Click anywhere on the map to find nearby soccer teams, compare their stats, and explore their recent matches!

![Soccer Map Explorer Demo](https://i.ibb.co/z4mpGSr/ezgif-6-b1be4cc9b465.gif)

## 🌟 Features

- **Interactive Map Exploration**: Click anywhere to discover nearby soccer teams
- **Team Comparison**: Select and compare any two teams
- **Match History**: View detailed history of matches between selected teams
- **Multi-League Support**: Access data from 10 major European leagues:
  - 🏴󠁧󠁢󠁥󠁮󠁧󠁿 England
  - 🇩🇪 Germany
  - 🇫🇷 France
  - 🇪🇸 Spain
  - 🇮🇹 Italy
  - 🇵🇹 Portugal
  - 🇷🇺 Russia
  - 🇧🇪 Belgium
  - 🇦🇹 Austria
  - 🇳🇱 Netherlands

## 🎮 Demo

### Finding Nearby Teams
![Get closest teams](https://i.ibb.co/z4mpGSr/ezgif-6-b1be4cc9b465.gif)

### Selecting Teams
![Choose a team](https://i.ibb.co/Wk8SSB2/ezgif-6-dc3ac2c2c566.gif)

### Comparing Teams
![Compare two teams](https://i.ibb.co/b655jDv/ezgif-6-96cb35c80b3b.gif)

## 🚀 Getting Started

### Prerequisites

1. Google Cloud API key
2. SportMonks API key
3. Node.js and npm/yarn installed

### Environment Setup

Create a `.env` file in both the backend and frontend directories:

```env
# Backend .env
GOOGLE_MAPS_API_KEY=your_google_api_key
SPORTMONKS_API_KEY=your_sportmonks_api_key

# Frontend .env
REACT_APP_GOOGLE_MAPS_API_KEY=your_google_api_key
```

### Installation

1. Clone the repository:
```bash
git clone [repository-url]
```

2. Start the backend:
```bash
cd backend
npm install
npm start
```

3. Start the frontend:
```bash
cd ../app
yarn install
yarn start
```

## 🛠️ How It Works

1. **Map Interaction**:
   - User clicks a point on the map
   - System captures latitude and longitude

2. **Location Processing**:
   - Backend uses Google Geocoding API to identify country and region
   - Queries database for teams in the specified area

3. **Team Selection**:
   - Shows 3 closest teams in the region
   - If fewer than 3 teams in region, finds next closest teams

4. **Match History**:
   - After selecting two teams, retrieves match history via SportMonks API
   - Displays detailed comparison and statistics

## 💻 Technologies

- **Frontend**:
  - React
  - React Google Maps
  - Modern UI/UX design

- **Backend**:
  - Express.js
  - MongoDB
  - RESTful API architecture

- **Development Tools**:
  - Postman (API testing)
  - MongoDB Compass (Database management)
  - Git (Version control)

## 📝 Notes

- Currently supports top-tier leagues only
- Team locations are based on stadium coordinates
- Database is pre-seeded with team information

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](link-to-issues).
