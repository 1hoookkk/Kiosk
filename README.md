# Harvey Norman - Robot Vacuum Video Showcase

An autoplay video showcase kiosk application designed for iPad display on the Harvey Norman sales floor.

## Features

- **Auto-rotating videos**: Automatically cycles through product videos every 15 seconds
- **Touch controls**: Swipe left/right to navigate between videos
- **iPad optimized**: Responsive design specifically tailored for iPad displays
- **Full-screen mode**: Clean, distraction-free interface perfect for sales floor kiosks
- **28 Product Videos**: Showcasing ECOVACS, Roborock, Dreame, EUFY, MOVA, NARWAL and more

## Products Featured

- ECOVACS WS2, X11, Mopping Demo
- Roborock Z10
- Dreame X50 Ultra, L40 Ultra, L40, Aqua
- EUFY Robot Vacuums
- MOVA Roller, Z60
- SAROS 10R, Z10
- NARWAL Flow
- Buying guides and setup tutorials

## How to Use

### On iPad

1. Open Safari and navigate to the deployed URL
2. Tap the share button and select "Add to Home Screen"
3. Open the app from your home screen for full-screen experience
4. Enable "Guided Access" in iPad settings to lock the kiosk to this app

### Controls

- **Swipe Left/Right**: Navigate between videos
- **Tap Play/Pause Button**: Pause/resume autoplay
- **Tap Navigation Dots**: Jump to specific video
- **Arrow Buttons**: Manual navigation

### Auto-play Settings

- Videos auto-advance every 15 seconds
- Progress bar shows time remaining
- Auto-play can be paused using the center button
- Swipe gestures reset the auto-play timer

## Deployment

### GitHub Pages (Recommended - Free & Automatic)

The site automatically deploys to GitHub Pages when you push to the repository.

**Your live URL**: `https://1hoookkk.github.io/Kiosk`

To enable GitHub Pages:
1. Go to your GitHub repository settings
2. Navigate to **Pages** (under "Code and automation")
3. Under "Source", select **GitHub Actions**
4. Push this code to your repository
5. The site will automatically deploy!

Access from any phone or iPad by visiting the URL above.

### Vercel

```bash
npm i -g vercel
vercel --prod
```

### Manual Hosting

Simply upload the `index.html` file to any web server. No build process required.

## iPad Kiosk Setup

1. **Enable Guided Access**:
   - Go to Settings > Accessibility > Guided Access
   - Turn on Guided Access
   - Set a passcode

2. **Open the app and activate Guided Access**:
   - Triple-click the home button (or side button on newer iPads)
   - This locks the iPad to only this application

3. **Prevent screen dimming**:
   - Settings > Display & Brightness > Auto-Lock > Never

4. **Keep iPad charged**:
   - Use a tablet stand with built-in charging

## Technical Details

- Pure HTML/CSS/JavaScript - no dependencies
- YouTube embed API for video playback
- Touch event handling for swipe gestures
- Wake Lock API to prevent screen sleep
- Responsive design with iPad-specific optimizations

## Browser Compatibility

- Safari (iPad) - Primary target
- Chrome, Firefox, Edge - Desktop testing

## Notes

- Videos are embedded from YouTube with autoplay and mute enabled
- First interaction may be required to enable audio due to browser autoplay policies
- Internet connection required for video streaming
