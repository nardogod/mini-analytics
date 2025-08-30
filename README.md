# Analytics Dashboard LLM made in two hours 
(estimated time counting planning, design, code adjustment, versioning and deployment)

Real-time analytics system with modern glassmorphism UI and interactive heatmap tracking.

## Live Demo

**Deploy:** [Vercel](https://mini-analytics2025.vercel.app/)  
**Repository:** [GitHub](https://github.com/nardogod/mini-analytics)

## Features

### Core Analytics
- Real-time IP detection and geolocation
- Browser fingerprinting and device analysis
- Session timing with live updates
- Language and resolution detection

### Heatmap Tracking
- Interactive click tracking with coordinates
- Visual ripple effects on interactions
- Real-time click counters per element
- Click history with timestamps

### UI/UX
- Glassmorphism design with backdrop filters
- Animated gradient backgrounds
- Responsive mobile-first layout
- Live status indicators

## Technical Implementation

### Frontend Stack
```
HTML5 + CSS3 + Vanilla JavaScript ES6+
```

### External APIs
- **ipapi.co** - IP geolocation service
- **Firebase Realtime Database** - Real-time data synchronization

### Key Technologies

| Technology | Implementation |
|------------|----------------|
| Glassmorphism | CSS backdrop-filter with rgba transparency |
| Heatmap Tracking | Event listeners capturing click coordinates |
| Real-time Updates | JavaScript intervals with DOM manipulation |
| API Integration | Fetch API with async/await error handling |
| Responsive Design | CSS Grid/Flexbox with mobile-first approach |
| Performance | Efficient DOM updates and memory management |



### Data Flow
1. **Client Detection** → Browser analysis via User Agent
2. **Geolocation** → IP-based location via REST API
3. **Session Tracking** → Timer-based analytics
4. **Interaction Tracking** → Click coordinates and frequency
5. **Real-time Display** → Live UI updates

## Analytics Metrics

| Metric | Source | Purpose |
|--------|--------|---------|
| IP Address | ipapi.co API | User identification |
| Geographic Location | ipapi.co API | Regional analytics |
| Browser Type | navigator.userAgent | Compatibility tracking |
| Screen Resolution | window.screen | Device analytics |
| Session Duration | JavaScript timer | Engagement metrics |
| Click Patterns | Event listeners | UX behavior analysis |

## Performance Optimizations

- **Async API Calls** - Non-blocking data fetching
- **Efficient DOM Updates** - Minimal reflows and repaints
- **Event Delegation** - Optimized event handling
- **Memory Management** - Proper cleanup of intervals and listeners

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Installation & Deployment

### Local Development
```bash
# Clone repository
git clone https://github.com/nardogod/mini-analytics.git

# Open in browser
open index.html
```

### Production Deployment
```bash
# Vercel CLI
npm install -g vercel
vercel login
vercel --prod

# GitHub Pages
git push origin main
# Enable Pages in repository settings
```

## Code Structure

### Core Functions
- `collectData()` - Initializes analytics collection
- `getBrowserInfo()` - Parses User Agent string
- `fetchIP()` - Handles geolocation API calls
- `trackClick()` - Processes heatmap interactions
- `updateClickList()` - Manages click history display

### CSS Architecture
- **BEM-inspired** class naming
- **CSS Custom Properties** for theming
- **Flexbox/Grid** hybrid layout system
- **Animation keyframes** for smooth transitions

## Security Considerations

- Client-side only implementation
- No sensitive data storage
- CORS-compliant API usage
- Input sanitization for display

## Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/enhancement`)
3. Commit changes (`git commit -m 'Add enhancement'`)
4. Push to branch (`git push origin feature/enhancement`)
5. Open Pull Request

## License

MIT License - Open source and free to use.

---

**Built with 100% LLM technologies to demonstrate full-stack capabilities and contemporary UI design patterns.**
