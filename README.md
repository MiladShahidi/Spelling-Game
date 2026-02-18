# Type Defense - Typing Game for Kids

A fun, adaptive typing game where kids shoot down falling alien words by typing them correctly. The game automatically adjusts difficulty based on the player's performance, making it perfect for kids at any skill level.

## Features

- **Adaptive Difficulty**: Game speed adjusts based on player performance - speeds up when they're doing well, slows down when struggling
- **Visual Feedback**: Colorful aliens, laser beams, and explosion effects
- **Sound Effects**: Programmatically generated sounds (no external files needed)
- **High Score Tracking**: Persistent high scores saved locally
- **Custom Word Lists**: Easy to customize word lists via CSV file
- **Offline Ready**: Runs completely locally in a browser

## How to Play

1. **Start the Game**: Open `index.html` in a web browser and press SPACE
2. **Type the Words**: As words fall from the top of the screen, type them exactly to shoot them down
3. **Don't Let Them Land**: If any word reaches the ground, the game is over
4. **Beat Your High Score**: Try to type more words correctly to set new records

## Installation

### Running Locally

1. Download all files to a folder on your computer:
   - `index.html`
   - `words.csv`
   - `README.md`

2. Open `index.html` in a modern web browser:
   - Double-click the file, or
   - Right-click and select "Open with" → your browser
   - Recommended browsers: Chrome, Firefox, Safari, Edge

3. Press SPACE to start playing!

### Deploying Online

To make the game accessible from anywhere:

#### Option 1: GitHub Pages (Free)
1. Create a GitHub account at https://github.com
2. Create a new repository
3. Upload `index.html` and `words.csv`
4. Go to repository Settings → Pages
5. Select main branch and save
6. Your game will be live at `https://yourusername.github.io/repositoryname`

#### Option 2: Netlify (Free)
1. Create account at https://netlify.com
2. Drag and drop the folder containing your files
3. Get instant URL like `https://your-game.netlify.app`

#### Option 3: Vercel (Free)
1. Create account at https://vercel.com
2. Import your project
3. Deploy with one click

## Customizing Word Lists

The game uses words from `words.csv`. To create custom word lists:

1. Open `words.csv` in any text editor
2. Add one word per line
3. Save the file
4. Refresh the game in your browser

**Tips for word lists:**
- Mix short (3-4 letter) and longer words for variety
- Use words appropriate for your child's reading level
- Focus on spelling words they're learning in school
- Keep it between 20-100 words for good variety

**Example custom list for learning colors:**
```
red
blue
green
yellow
orange
purple
pink
brown
black
white
```

## Game Controls

- **SPACE**: Start game / Play again after game over
- **A-Z Keys**: Type letters
- **BACKSPACE**: Delete last letter

## How Adaptive Difficulty Works

The game tracks where on the screen you destroy each word:

- **High on screen** (top third): You're doing great! Game speeds up gradually
- **Middle**: Perfect pace, no changes
- **Low on screen** (bottom third): Struggling? Game slows down to help

The first 3 words are always slow to let players learn the mechanics. Adjustments happen every 5 words and are gradual (10% changes) so the difficulty feels natural, not jarring.

## Browser Compatibility

Works best on:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

Requires JavaScript enabled and Web Audio API support (available in all modern browsers).

## Troubleshooting

**Words aren't loading:**
- Make sure `words.csv` is in the same folder as `index.html`
- If CSV is missing, the game will use a built-in word list automatically

**No sound:**
- Check that your browser allows audio (some browsers block audio until user interaction)
- Click anywhere on the page before pressing SPACE to start
- Check your device volume settings

**Game runs too fast/slow:**
- The game adjusts automatically, but starts very slow
- Play a few rounds - it will adapt to your speed
- Try different browsers if performance is poor

**High scores not saving:**
- Make sure your browser allows localStorage
- Check you're not in private/incognito mode
- Try clearing browser cache and playing again

## Technical Details

- **Technology**: Vanilla JavaScript, HTML5 Canvas API, Web Audio API
- **File Size**: ~30KB (single file)
- **Requirements**: Modern web browser with JavaScript enabled
- **Performance**: Runs at 60 FPS on most devices
- **Storage**: Uses localStorage for high scores (< 1KB)

## Tips for Parents

- Start with simple 3-4 letter words for beginners
- Create themed word lists (animals, food, school subjects)
- Play together and take turns to make it social
- Celebrate new high scores to build confidence
- Let the game adjust naturally - don't force difficulty changes
- Use as a fun supplement to traditional spelling practice

## Future Ideas

Want to enhance the game? Some ideas:
- Add power-ups (slow motion, shields)
- Multiple difficulty modes (easy/medium/hard presets)
- Word categories to choose from
- Multiplayer split-screen mode
- Mobile touch keyboard support
- Progress tracking and statistics

## License

Free to use, modify, and share for educational purposes.

## Support

For issues or questions, check that:
1. Files are in the same folder
2. Using a modern browser
3. JavaScript is enabled
4. No browser console errors (press F12 to check)

Enjoy practicing your typing skills! 🚀
