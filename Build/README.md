# WebGL Build Assets

This directory contains the assets required for the WebGL build of CookieRun: Braverse Trading Card Game.

## Loading Screen Assets

### Required Files:

- `LoadingBackground.png` - Main loading screen background image
- `favicon.ico` - Browser favicon

### Loading Bar Implementation

The loading screen now includes a dynamic loading bar that matches the design from the Cookie Run Braverse loading screen image:

#### Features:

- **Bright Yellow Loading Bar**: Matches the golden/yellow color scheme from the original design
- **Smooth Animation**: Gradual fill with smooth transitions
- **Shimmer Effect**: Animated gradient that moves across the bar
- **Progress Percentage**: Real-time percentage display
- **Responsive Design**: Adapts to different screen sizes

#### Technical Details:

- The loading bar uses CSS gradients and animations
- Initial progress simulation (0-30%) before Unity loading starts
- Unity loading progress continues from 30-100%
- Smooth transitions with `ease-out` timing
- Glowing effect with box-shadow

#### CSS Classes:

- `#loading-bar-container`: Container with dark background and rounded corners
- `#loading-bar`: The actual progress bar with gradient and shine animation
- `#loading-percentage`: Text overlay showing percentage

#### JavaScript Integration:

- Progress updates are handled in the Unity loading callback
- Smooth transitions between initial loading and Unity loading phases
- Error handling for missing elements

### Asset Sources:

The loading bar design is inspired by the UI_settings_897 and UI_settings_898 assets from the Settings sprite collection, adapted for web implementation with CSS and JavaScript.

## Build Process:

1. Place your Unity WebGL build files in this directory
2. Ensure `LoadingBackground.png` is present
3. The loading bar will automatically appear during the loading process
