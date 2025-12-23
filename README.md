# The Hook Spin 🎰

A gamified micro-tool for content creators, indie hackers, and business owners. Generate viral hooks for your Reels, TikToks, and social media content with an interactive slot machine experience.

**Live at:** [creativeforge.site](https://creativeforge.site)

## What is it?

"The Hook Spin" is a single-page web application that gamifies the creative process for content creators. Instead of browsing through static lists of hooks, users click a button to spin through proven viral opening lines that land on their next content idea.

### Features

- 🎲 Interactive slot machine-style hook generator
- 🎨 Casino-cyberpunk aesthetic with neon colors
- ⚡ Lightning-fast spin animations
- 📱 Fully responsive design
- 💳 Stripe payment integration for upsell

## Setup Instructions

1. **Clone or download this repository**

2. **Set up Stripe Payment Link**
   - Create a Stripe account (if you don't have one)
   - Create a product called "The Viral Hook Cheatsheet" for $9
   - Generate a Payment Link for this product
   - Open `index.html` and replace `REPLACE_WITH_YOUR_STRIPE_PAYMENT_LINK` with your actual Stripe payment link URL

3. **Deploy**
   - The project is a single HTML file with no build process required
   - Deploy `index.html` to any static hosting service:
     - Netlify (drag and drop)
     - Vercel
     - GitHub Pages
     - Any web server

4. **Test Locally**
   - Simply open `index.html` in your web browser
   - No server required - it's pure HTML/CSS/JS

## Customization

### Adding More Hooks

Edit the `hooks` array in the `hookMachine()` function within `index.html`:

```javascript
hooks: [
    "Your hook text here.",
    "Another hook here.",
    // Add as many as you want
]
```

### Changing Colors

The color scheme is defined in the Tailwind config within `index.html`:

```javascript
colors: {
    'neon-pink': '#ff00ff',
    'neon-blue': '#00ffff',
    'dark-bg': '#1a0b2e',
}
```

### Adjusting Spin Duration

Modify the timeout value in the `spin()` function (currently 800ms):

```javascript
setTimeout(() => {
    // ...
}, 800); // Change this value (in milliseconds)
```

## Tech Stack

- **HTML5** - Structure
- **Tailwind CSS** (CDN) - Styling
- **Alpine.js** (CDN) - Reactive behavior
- **Vanilla JavaScript** - Core functionality

## Business Model

- **Free:** Interactive hook spinner
- **Upsell:** $9 "Viral Hook Cheatsheet" with 500+ hooks via Stripe

## Marketing

The product is designed for viral marketing via:
- TikTok/Instagram Reels showing the slot machine in action
- Low-friction funnel: Play → Get ideas → Purchase full cheatsheet

## License

This project is open source and available for personal or commercial use.

