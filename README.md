# 🎮 Pokédex App

A full-featured Pokédex web application with user authentication, team building, and type coverage analysis. Built with vanilla JavaScript and the PokeAPI.

## ✨ Features

### 🔍 Pokédex Search
- Search for any Pokémon by name
- View detailed stats (HP, Attack, Defense, Sp.Atk, Sp.Def, Speed)
- Display official sprite images
- Show Pokémon types with color-coded badges
- View height and weight information
- Random Pokémon button for discovery

### ❤️ Favorites System
- Add/remove favorite Pokémon
- Persistent storage using IndexedDB
- Export favorites as JSON
- User-specific favorites (each user has their own)

### 👥 User Authentication
- Signup with validation
- Login with credentials
- Secure password hashing
- Session persistence with "Remember Me" (30-day auto-login)
- Custom user profiles with display names
- Avatar selection (12 Pokémon options)

### ⚔️ Team Builder
- Build a team of up to 6 Pokémon from your favorites
- View team with sprite images, names, and types
- **Type Coverage Analysis:**
  - Offensive strengths (types your team is strong against)
  - Weaknesses (types that threaten your team)
  - Resistances (types your team resists)
- Team statistics (team size, type count, unique types)
- Persistent team storage per user

### 📜 Search History
- Last 5 searches saved
- Clickable history chips for quick re-search
- Automatic history management

## 🚀 Getting Started

### Option 1: Local File (Easiest)
1. Download `index.html`
2. Open in your browser: `file:///path/to/index.html`
3. Sign up → Search → Build team → Enjoy!

### Option 2: Local Server
```bash
# Navigate to project directory
cd /path/to/pokedex

# Start a simple HTTP server
python3 -m http.server 8000
# or
python -m http.server 8000
# or
npx http-server
```
Then open: **http://localhost:8000**

## 🎯 Quick Start Guide

### 1. Create an Account
- Click "Sign Up"
- Enter username (3+ characters)
- Enter password (6+ characters)
- Click "Create Account"

### 2. Search for Pokémon
- Type a Pokémon name in search box
- Click "Search" or press Enter
- Click "🎲 Random" for surprise picks
- Click the ❤️ to add to favorites

### 3. Build Your Team
- Click "Team Builder" section
- Click any empty slot ("+")
- Select 6 Pokémon from your favorites
- View type coverage analysis
- Remove pokémon with "×" button

### 4. Analyze Coverage
- **Offensive Coverage**: Types your team counters well
- **Weaknesses**: Types that threaten your team
- **Resistances**: Types your team can handle

### 5. Manage Profile
- Click user avatar in navbar
- Edit display name
- Select different avatar
- Save changes

## 🛠️ Technologies

- **Frontend**: HTML5, CSS3, Vanilla JavaScript (ES6+)
- **API**: [PokeAPI](https://pokeapi.co/) - Free Pokémon data
- **Storage**: IndexedDB (browser database)
- **Authentication**: Client-side with password hashing
- **No Dependencies**: Single HTML file, no frameworks needed

## 📊 Type System

Complete implementation of Pokémon type matchups:
- All 18 types included (Normal, Fire, Water, Electric, Grass, Ice, Fighting, Poison, Ground, Flying, Psychic, Bug, Rock, Ghost, Dragon, Dark, Steel, Fairy)
- Accurate type advantages/disadvantages
- Coverage analysis for team strategy

## 💾 Data Storage

- **IndexedDB**: Stores favorites and teams locally
- **localStorage**: Stores user accounts, preferences, search history
- **sessionStorage**: Manages current session
- **No server needed**: All data stored in your browser

### Data Structure
```
IndexedDB Database: "pokedex_db"
├── favorites (object store)
│   ├── username__pokemonname: Favorite pokémon
│   └── team_username: User's team (6 slots)
```

## 🔐 Privacy & Security

- No data sent to external servers (except PokeAPI for pokemon data)
- All user data stored locally in your browser
- Passwords are hashed before storage
- No tracking or analytics
- Complete privacy control

## 🎨 Styling Features

- Dark theme with red and white accents (Pokéball inspired)
- Smooth animations and transitions
- Responsive grid layouts
- Color-coded type badges
- Hover effects for interactivity
- Modal windows for selections

## 📱 Browser Compatibility

- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge
- Any modern browser with IndexedDB support

## 🐛 Troubleshooting

### Favorites not showing?
- Check browser settings allow IndexedDB
- Try a different browser
- Clear browser cache and reload

### Team not saving?
- Ensure you're logged in
- Check IndexedDB is enabled
- Refresh the page after adding pokémon

### Search not working?
- Check internet connection (uses PokeAPI)
- Verify Pokémon name spelling
- Try the Random button to test connectivity

## 📝 File Structure

```
pokedex/
├── index.html          # Complete app (all code in one file)
├── README.md          # This file
└── LICENSE             # MIT License
```

## 📜 License

MIT License - Feel free to use, modify, and share!

## 🙏 Credits

- **PokeAPI**: [pokéapi.co](https://pokeapi.co/) - Pokémon data
- **Pokémon**: Game Freak, Nintendo, The Pokémon Company
- **Assets**: Official Pokémon sprites from PokeAPI

## 🚀 Future Features

Potential enhancements:
- Multiple team slots (Team A, Team B, etc.)
- Team sharing between users
- Suggested move sets for team members
- Weakness coverage recommendations
- Export/import teams
- Team comparison with other users
- EV/IV calculator
- Breeding chain generator
- Competitive ranking system

## 💬 Feedback & Suggestions

Have ideas? Found a bug? Feel free to:
- Test the app thoroughly
- Report issues
- Suggest new features
- Share your favorite teams!

---

**Made with ❤️ for Pokémon fans** 🎮✨
