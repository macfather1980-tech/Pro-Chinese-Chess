# 象棋大师 - Master Xiangqi ♔♚

> A premium, feature-complete Chinese Chess (Xiangqi) game built for the modern web.

## Features

### Complete Game Rules
- **All 7 piece types**: 帥/將 (General), 士/仕 (Advisor), 象/相 (Elephant), 車 (Chariot), 馬 (Horse), 炮/砲 (Cannon), 兵/卒 (Soldier)
- **Flying General rule**: Kings cannot face each other on the same file
- **Check / Checkmate / Stalemate** detection
- **Threefold repetition** and **fifty-move rule** for draws
- **Palace restrictions** for Generals and Advisors
- **River crossing** rules for Elephants and Soldiers
- **Hobbling** detection for Horses

### AI Opponent (4 Levels)
| Level | Search Depth | Description |
|-------|-------------|-------------|
| 初级 (Beginner) | 2 | Casual play, occasional mistakes |
| 中级 (Intermediate) | 3 | Solid play, good for learning |
| 高级 (Advanced) | 4 | Challenging, strategic play |
| 大师 (Grandmaster) | 5 | Very strong, tournament-level |

**AI Features:**
- Minimax with Alpha-Beta pruning
- Quiescence search (avoids horizon effect)
- Move ordering (captures first)
- Positional evaluation (center control, king safety, pawn advancement)
- Configurable think time (1-30 seconds)

### Beautiful UI
- SVG-rendered traditional wooden board
- 3D-styled wooden pieces with red/black coloring
- Animated piece placement and check indicators
- Move hints (dots for empty squares, rings for captures)
- Last move highlighting
- Board flip (rotate 180°)
- Fully responsive design (desktop + mobile)

### Mobile Optimized
- **Touch-friendly** controls with haptic feedback
- **Fullscreen mode** for immersive play
- **Landscape mode** support
- **Safe area handling** for iOS notches
- **Prevents** pull-to-refresh and double-tap zoom
- **Add to Home Screen** ready (PWA-capable)

### Game Features
- **Sound effects** via Web Audio API (move, capture, check, game over)
- **Move history** with traditional Chinese notation
- **Undo** (reverses both AI and player moves)
- **Timer** for tracking game duration
- **Resign** option
- **Settings panel** for AI difficulty, color choice, sound toggle

## Quick Start

1. **Download** or clone this repository
2. **Open** `index.html` in any modern browser
3. **Play** — no server, no dependencies, no install needed

## Deployment

### GitHub Pages (Free)

1. Create a new GitHub repository named `xiangqi-chess`
2. Push this repository to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: 象棋大师 - Master Xiangqi"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/xiangqi-chess.git
   git push -u origin main
   ```
3. Go to **Settings → Pages**
4. Under **Source**, select `main` branch and `/ (root)` folder
5. Click **Save**
6. Your game will be live at `https://YOUR_USERNAME.github.io/xiangqi-chess/`

### Custom Domain

1. Create a file named `CNAME` (no extension) in the repository root
2. Add your domain name (e.g., `xiangqi.example.com`)
3. Point your domain's DNS to GitHub Pages

### Other Hosting

This is a static single-page application — deploy anywhere:
- **Netlify**: Drag and drop the folder
- **Vercel**: `vercel deploy`
- **Cloudflare Pages**: Connect GitHub repo
- **Any static host**: Just serve the files

## Mobile Usage

### iOS (iPhone/iPad)
1. Open the game in Safari
2. Tap the **Share** button (⬆️)
3. Select **"Add to Home Screen"**
4. Launch from your home screen like a native app

### Android (Chrome)
1. Open the game in Chrome
2. Tap the **menu** (⋮)
3. Select **"Add to Home Screen"** or **"Install App"**

## Technical Details

- **Single-file application**: Zero dependencies, no build step
- **Pure HTML/CSS/JavaScript**: Works offline
- **Responsive**: Adapts from mobile (320px) to 4K displays
- **Web Audio API**: Synthesized sound effects (no audio files needed)
- **SVG rendering**: Crisp board at any resolution
- **~56KB total**: Lightning fast loading

## Browser Support

- Chrome/Edge 80+
- Firefox 78+
- Safari 13+ (iOS 13+)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Files

| File | Description |
|------|-------------|
| `index.html` | The complete game (1800+ lines) |
| `favicon.svg` | App icon for bookmarks |
| `.gitignore` | Git ignore rules |
| `README.md` | This file |

## License

Free for personal use. For commercial licensing, contact the developer.

---

**象棋大师 v2.0** — 弈棋之乐，尽在方寸之间

*Built with ❤️ for the Chinese Chess community*
