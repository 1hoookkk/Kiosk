# Video Showcase - Quick Guide

## Why Some Videos Don't Play

Videos might not play for these reasons:

1. **Wrong Video ID** - Typos in the YouTube ID
2. **Private/Deleted Videos** - Owner removed or restricted the video
3. **Regional Restrictions** - Video not available in your country
4. **Age Restrictions** - Some videos require sign-in

## How to Fix Videos

### Easy Method - Edit the HTML File

1. Open `index.html` in any text editor
2. Find the video list (around line 350)
3. Look for this section:

```javascript
const videos = [
    { title: "Product Name", id: "VIDEO_ID" },
    // Add more here!
];
```

### How to Get the Video ID

From any YouTube URL, the ID is:

**Regular videos:**
- URL: `https://www.youtube.com/watch?v=ABC123xyz`
- ID: `ABC123xyz`

**Shorts:**
- URL: `https://www.youtube.com/shorts/XYZ789abc`
- ID: `XYZ789abc`

### Add/Edit Videos

Just copy this line and change the title and ID:

```javascript
{ title: "My Product Name", id: "dQw4w9WgXcQ" },
```

**Important:** Don't forget the comma at the end!

## Current Video Count

The showcase now has **28 videos** organized by brand:
- ECOVACS (3 videos)
- Roborock (1 video)
- Dreame (6 videos)
- EUFY (3 videos)
- MOVA (2 videos)
- SAROS (2 videos)
- NARWAL (5 videos)
- General guides (6 videos)

## Testing Videos

To test if a video ID works:
1. Go to: `https://www.youtube.com/watch?v=VIDEO_ID`
2. Replace `VIDEO_ID` with your ID
3. If it plays in YouTube, it should work in the showcase!

## Quick Deploy

After editing:
1. Save the file
2. Commit: `git add index.html && git commit -m "Update videos"`
3. Push: `git push`
4. Wait 1-2 minutes for deployment

Your showcase will update automatically at:
`https://1hoookkk.github.io/Kiosk`

## Need Help?

If a video still doesn't work:
1. Verify the video ID is exactly 11 characters (usually)
2. Test the video in a regular YouTube URL
3. Try a different video if it's private/restricted
