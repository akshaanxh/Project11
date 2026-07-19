# 🏏 IPL Pro Analyst

<div align="center">



**Your Data-Driven Edge for the Indian Premier League**

</div>

---

## 🌟 Overview

IPL Pro Analyst is a comprehensive, data-driven analytics platform that transforms raw IPL cricket statistics into actionable insights. Whether you're a fantasy cricket enthusiast, a stats geek, or just love the game, this platform provides the tools you need to make informed decisions.

**🔗 Live Demo:** [https://xproject11.vercel.app/](https://xproject11.vercel.app/)

---

## ✨ Features

### 📊 Player Stats Hub
- **Advanced Search**: Quickly find any player from IPL history
- **Comprehensive Statistics**: View detailed batting and bowling career stats
- **Head-to-Head Analysis**: Compare player performance against specific opponents
- **Venue-Specific Stats**: Analyze how players perform at different grounds
- **Recent Form**: Track the last 5 IPL performances with visual indicators

### ⚡ Match Predictor
- **Smart Team Selection**: Pick 11 players from competing teams
- **AI-Powered Predictions**: Statistical model predicts match winners
- **Visual Probability Display**: See win percentages with interactive progress bars
- **Real-Time Updates**: Dynamic predictions based on your lineup selections

### 🎯 Fantasy XI Builder
- **Budget Management**: Build teams within the 100-credit constraint
- **Role-Based Selection**: Automatic validation for WK, BAT, AR, BOWL positions
- **Captain & Vice-Captain**: Assign multipliers to maximize points
- **AI Suggestions**: Get optimal team recommendations based on historical PPG (Points Per Game)
- **Team Comparison**: Compare your picks against AI-suggested lineups
- **Interactive Cards**: Visual feedback for player selection and team composition

---

## 🎨 Design Highlights

- **Modern Dark Theme**: Sleek gradient backgrounds with slate color palette
- **Glassmorphism Effects**: Contemporary UI with backdrop blur and transparency
- **Responsive Design**: Seamless experience across desktop, tablet, and mobile
- **Micro-Animations**: Smooth transitions and hover effects for enhanced UX
- **Sticky Navigation**: Context-aware headers that stay accessible while scrolling
- **Visual Feedback**: Color-coded indicators for constraints, selections, and predictions

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: Next.js 15.5.6 with Turbopack
- **Language**: TypeScript
- **Styling**: TailwindCSS with custom utilities
- **UI Components**: shadcn/ui component library
- **Icons**: Lucide React

### Features
- **State Management**: React Hooks (useState, useMemo, useCallback)
- **Performance**: Memoized calculations for optimal rendering
- **Type Safety**: Full TypeScript implementation with strict mode
- **Code Quality**: ESLint with TypeScript rules

### Deployment
- **Platform**: Vercel
- **CI/CD**: Automatic deployments from GitHub
- **Performance**: Edge-optimized with global CDN

---

## 📁 Project Structure

```
ipl-website/
├── app/
│   ├── page.tsx              # Main application component
│   ├── layout.tsx            # Root layout
│   └── globals.css           # Global styles
├── components/
│   └── ui/                   # shadcn/ui components
├── public/                   # Static assets
├── data/                     # CSV/JSON data files
│   ├── player_roles.json
│   ├── batting_stats.json
│   ├── bowling_stats.json
│   ├── fantasy_points.json
│   └── match_data.json
└── scripts/
    └── convert_csv_to_json.py # Data processing script
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ installed
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/akshaanxh/Project11.git
   cd Project11
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Prepare data files** (if needed)
   ```bash
   python convert_csv_to_json.py
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

---

## 📊 Data Processing

The application uses historical IPL data processed from CSV files:

- **Player Roles**: Team assignments and player credits
- **Batting Statistics**: Runs, balls, strike rates, dismissals
- **Bowling Statistics**: Wickets, economy, averages
- **Fantasy Points**: Historical points per game (PPG)
- **Match Data**: Team matchups and venues

### Adding New Data

1. Place CSV files in the `data/` directory
2. Run the conversion script:
   ```bash
   python convert_csv_to_json.py
   ```
3. Import JSON files into `app/page.tsx`

---

## 🎯 Key Features Explained

### Fantasy Team Builder Algorithm

The AI suggestion engine uses a **value-based selection approach**:

1. **Calculate PPG/Credit ratio** for each player
2. **Sort players** by value efficiency
3. **Greedy selection** within budget and role constraints
4. **Optimize for maximum PPG** while respecting limits

```typescript
Value Score = Player PPG / Player Credits
```

### Match Prediction Model

Win probability calculation based on:
- **Team PPG differential**: Higher PPG increases win probability
- **Baseline 50-50 split**: Adjusted by performance metrics
- **Capped predictions**: Min 30%, Max 70% to account for uncertainty

---

## 🎨 UI Components

### Custom Components Used
- **Cards**: Container components for sections
- **Select Dropdowns**: Team, player, and venue selection
- **Checkboxes**: Player lineup selection
- **Radio Groups**: Captain/Vice-Captain selection
- **Progress Bars**: Win probability visualization
- **Dialogs**: Fantasy team analysis modal
- **Tabs**: Main navigation between features

---

## 📈 Performance Optimizations

- **Memoization**: Heavy calculations cached with `useMemo`
- **Callback Optimization**: Functions memoized with `useCallback`
- **Lazy Loading**: Components loaded on-demand
- **Turbopack**: Lightning-fast builds and hot reloading
- **Edge Deployment**: Sub-100ms response times globally

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a Pull Request**

---

## 🐛 Known Issues & Future Enhancements

### Known Issues
- None currently reported

### Planned Features
- [ ] Live match integration with real-time scoring
- [ ] Player comparison tool
- [ ] Advanced filtering and sorting options
- [ ] Export team sheets as images
- [ ] Historical season comparisons
- [ ] Mobile app version
- [ ] User accounts and saved teams

---

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**Akshaan**

- GitHub: [@akshaanxh](https://github.com/akshaanxh)
- Project Link: [https://github.com/akshaanxh/Project11](https://github.com/akshaanxh/Project11)
- Live Demo: [https://xproject11.vercel.app/](https://xproject11.vercel.app/)

---

## 🙏 Acknowledgments

- **IPL**: For providing the world's most exciting cricket league
- **shadcn/ui**: For the beautiful component library
- **Vercel**: For seamless deployment and hosting
- **Next.js Team**: For an amazing React framework
- **Cricket Fans**: For the inspiration and support

---

<div align="center">

### ⭐ Star this repo if you found it helpful!

**Made with ❤️ and ☕ by cricket enthusiasts, for cricket enthusiasts**



</div>

<!-- note: - Improved loading state UX flow -->
