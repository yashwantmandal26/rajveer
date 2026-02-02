# 🎉 Funny Birthday Prank Website

An interactive, futuristic birthday prank web experience with stunning visual effects, animations, and surprise reveals. This project creates a playful birthday celebration for "Rajveer Bhai" with a fun prank button that runs away from the user before revealing birthday surprises.

## ✨ Features

### 🎮 Interactive Prank Mechanics
- **Escaping Button**: The gift button dodges mouse/touch attempts 15 times before allowing interaction
- **Dynamic Text Changes**: Button text changes with humorous phrases in Hindi/English on each attempt
- **Progressive Difficulty**: Button behavior intensifies with neon effects after multiple attempts

### 🎨 Premium Visual Effects
- **Glassmorphism Design**: Modern frosted glass UI elements with backdrop blur
- **Animated Gradient Background**: Dynamic color-shifting background with floating orbs
- **Neon Glow Effects**: Cyberpunk-inspired glowing borders and text
- **Fireworks Canvas**: Real-time particle system with physics simulation
- **Confetti Rain**: Colorful confetti particles with rotation animations
- **Sparkle Stars**: Twinkling star background particles
- **Emoji Rain**: Falling animated emojis during interactions

### 🎭 Multi-Phase Reveals
1. **Phase 1 - Karela (Bitter Gourd) Prank**: Initial humorous reveal with a vegetable gift
2. **Phase 2 - Real Birthday Celebration**: Actual birthday message with cake image
3. **Phase 3 - Video Surprise**: Trump birthday wish video appears (bottom-right corner)

### 🎵 Audio Integration
- First reveal sound effect (Karela reveal)
- Final celebration sound effect (Cake reveal)
- Auto-volume adjustment during video playback

### 📱 Fully Responsive Design
- **Desktop**: Optimized for large screens (1920x1080+) and medium laptops (1366x768)
- **Tablets**: Enhanced touch targets and adjusted layouts
- **Mobile Portrait/Landscape**: Adaptive sizing for phones (down to iPhone SE size)
- **Touch Optimization**: Larger touch targets and appropriate touch event handling

### 🖱️ Custom Elements
- **Monkey Cursor**: Custom emoji cursor (🐵) throughout the experience
- **Scanline Effect**: Retro CRT monitor aesthetic overlay

## 🛠️ Technology Stack

- **Pure HTML5**: Semantic markup
- **CSS3**: Advanced animations, transforms, glassmorphism, gradients
- **Vanilla JavaScript**: Canvas API, particle systems, event handling
- **Responsive Design**: Media queries for all device sizes

## 📦 Required Assets

The project requires the following assets in the same directory:

```
Funny BIRTHDAY/
├── index.html
├── karela.png          (Image: Bitter gourd / karela)
├── rajveer.png           (Image: Birthday person's photo)
├── first_reveal.mp3    (Audio: First reveal sound)
├── final_reveal.mp3    (Audio: Celebration sound)
└── trump_wish.mp4      (Video: Birthday video message)
```

## 🚀 Usage

### Running the Project

1. **Clone or Download** the project files
2. **Add Required Assets**: Place all images, audio, and video files in the project folder
3. **Open in Browser**: Simply open `index.html` in any modern web browser
   ```
   No server required - runs completely client-side
   ```

### How It Works

1. **Initial Screen**: User sees a greeting and a "Click for Gift 🎁" button
2. **Prank Phase**: Button escapes from cursor/touch 15 times with funny messages
3. **Karela Reveal**: After 15 attempts, clicking reveals a humorous bitter gourd gift (6 seconds)
4. **Birthday Reveal**: Transitions to the actual birthday celebration with fireworks and confetti
5. **Video Surprise**: After 5 seconds, a birthday video appears in the corner

## 🎯 Key Animations

- **gradientShift**: Background color cycling
- **floatOrbs**: Floating gradient orbs
- **neonPulse**: Glowing button effects
- **textGlow**: Shimmering text effects
- **confettiFall**: Confetti physics
- **sparkle**: Twinkling stars
- **videoGlow**: Video container pulse effect
- **Fireworks**: Real-time Canvas particle system

## 🎨 Color Palette

```css
Primary: #00ffff (Cyan)
Secondary: #ff00ff (Magenta)
Accent: #00ff88 (Mint Green)
Background: Dark gradient (#0a0a1a to #1a2a4e)
Gold: #FFD700 (Birthday celebration)
```

## 📐 Responsive Breakpoints

- Extra Large Desktop: `≥1200px`
- Medium Laptops: `992px - 1199px`
- Tablets: `768px - 991px`
- Mobile Landscape: `≤767px` (landscape)
- Mobile Portrait: `≤576px` (portrait)
- Extra Small: `≤375px`

## 🎭 Customization

### Change Recipient Name
```javascript
// In index.html, update these elements:
<h1 id="main-title">Hey Rajveer Bro! ✨</h1>
<h1>Happy Birthday Rajveer! 🎉</h1>
<h1>🎂 HAPPY BIRTHDAY RAJVEER! 🎂</h1>
```

### Adjust Prank Difficulty
```javascript
const maxAttempts = 15; // Change this number (line ~878)
```

### Modify Button Phrases
```javascript
const phrases = [
    "Your custom phrase here! 😎",
    // Add more phrases...
]; // Lines ~881-896
```

### Change Visual Effects
```css
/* Adjust fireworks frequency (line ~1145) */
if (Math.random() < 0.04) { // Increase/decrease probability

/* Confetti amount (line ~871) */
for (let i = 0; i < 30; i++) { // Change count

/* Sparkle count (line ~844) */
for (let i = 0; i < 15; i++) { // Change count
```

## ⚡ Performance Optimizations

- Reduced particle counts on mobile devices
- Optimized animation frame rates
- Efficient DOM element cleanup (automatic removal)
- Canvas clearing with fade effect (reduced memory usage)
- Conditional effect disabling during video playback
- Debounced sparkle generation

## 🌐 Browser Compatibility

- ✅ Chrome/Edge (Recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Requirements**:
- HTML5 Canvas support
- CSS3 animations
- Audio/Video playback
- Backdrop-filter support (graceful degradation)

## 📝 License

This project is open-source and free to use for personal birthday pranks and celebrations.

## 🎓 Learning Highlights

This project demonstrates:
- Advanced CSS animations and transitions
- Canvas-based particle systems
- Responsive design patterns
- Event handling for touch and mouse
- Audio/video integration
- Glassmorphism UI design
- Performance optimization techniques

## 🤝 Credits

Created with ❤️ for Rajveer Bhai's birthday celebration

---

**Note**: Replace the asset files (images, audio, video) with your own content before use. The project is designed to be easily customizable for any birthday recipient!

🎂 Happy Coding & Happy Birthday! 🎉
