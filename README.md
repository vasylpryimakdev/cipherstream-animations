# CipherStream Scroll Animations

A modern web showcase featuring advanced CSS scroll-driven animations for a tech company portfolio.

## 🚀 Live Demo

👉 [https://vasylpryimakdev.github.io/cipherstream-animations/](https://vasylpryimakdev.github.io/cipherstream-animations/)

## Features

### Scroll-Driven Animations

- **Hero Section**: Parallax video layers with smooth transitions
- **Navigation Header**: Dynamic height and background color changes on scroll
- **Team Section**: Horizontal scrolling grid with 3D image rotations
- **Background Animations**: Color transitions and neon effects

### Key Animation Techniques

- CSS `view-timeline` and `timeline-scope`
- Scroll-driven keyframe animations
- Sticky positioning with animated backgrounds
- 3D transforms and clip-path animations
- SVG stroke animations with neon glow effects

## Project Structure

```
exercise-3/
|-- css/
|   |-- base.css          # Base styles and timeline scope
|   |-- hero.css          # Hero section animations
|   |-- nav.css           # Navigation scroll animations
|   |-- team.css          # Team section scroll animations
|   |-- features.css      # Feature cards styling
|   |-- services.css      # Services section styling
|   |-- footer.css        # Footer styling
|   |-- styles.css        # Main stylesheet imports
|-- assets/
|   |-- *.mp4             # Background videos
|   |-- *.svg             # Icons and logos
|   |-- *.jpg             # Team member images
|-- index.html            # Main HTML structure
|-- script.js             # JavaScript functionality
|-- README.md             # This file
```

## Animation Details

### Navigation Header Animation

- **Timeline**: `--hero-view` (hero section scroll)
- **Range**: `exit-crossing 50%` to `exit-crossing 70%`
- **Effect**: Transitions from full height (100px) to compact height with background

### Team Section Animations

- **Timeline**: `--team-view` (team section scroll)
- **Effects**:
  - Horizontal grid movement (`moveTeamGrid`)
  - 3D image rotation (`rotateTeamMemberImage`)
  - Background color transitions (`teamBg`)
  - Title fade-in (`titleAppear`)
  - Card appearance with clip-path (`cardAppear`)
  - SVG logo drawing with neon glow (`drawLogo`, `neon`)

## Technologies Used

- **HTML5**: Semantic markup with accessibility features
- **CSS3**: Modern scroll-driven animations
- **JavaScript**: Basic interactivity
- **Google Fonts**: Poppins and Roboto Mono font families

## Browser Support

This project uses modern CSS scroll-driven animations. Best viewed in browsers that support:

- `view-timeline` CSS property
- `animation-timeline` CSS property
- `animation-range` CSS property

Recommended browsers:

- Chrome 115+
- Edge 115+
- Safari 16.4+
- Firefox 108+

## Getting Started

1. Clone the repository

```bash
git clone https://github.com/vasylpryimakdev/cipherstream-animations.git
cd cipherstream-animations
```

2. Open `index.html` in a modern web browser
3. Scroll through the page to experience the animations

## Customization

### Timeline Adjustments

Modify the `animation-range` values in CSS files to control when animations trigger:

```css
.example {
  animation-timeline: --section-view;
  animation-range: entry-crossing 20% entry-crossing 80%;
}
```

### Animation Speed

Adjust animation duration and timing functions:

```css
@keyframes example {
  to {
    transform: translateX(-100%);
  }
}

.example {
  animation: linear 1s both example;
}
```

### Color Scheme

Update CSS custom properties in `base.css`:

```css
:root {
  --bg: #0a120f;
  --green: #4ade80;
  --header-height: 60px;
}
```
