# Yash's Portfolio

A modern, responsive portfolio website built with React and Vite, featuring dark mode and a beautiful UI.

## Features

- 🎨 Modern, responsive design
- 🌙 Dark/Light theme toggle
- 📱 Mobile-first approach
- ⚡ Fast performance with Vite
- 🚀 Ready for GitHub Pages deployment

## Tech Stack

- **Frontend**: React 18
- **Build Tool**: Vite
- **Styling**: CSS with CSS Variables
- **Deployment**: GitHub Pages

## Getting Started

### Prerequisites

- Node.js 16+ 
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/portfolio.git
cd portfolio
```

2. Install dependencies:
```bash
npm install
```

3. Start development server:
```bash
npm run dev
```

4. Open [http://localhost:5173](http://localhost:5173) in your browser.

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run deploy` - Deploy to GitHub Pages (manual)

## Deployment to GitHub Pages

### Automatic Deployment (Recommended)

1. Push your code to the `main` branch
2. GitHub Actions will automatically build and deploy to GitHub Pages
3. Go to your repository Settings → Pages
4. Set source to "GitHub Actions"

### Manual Deployment

1. Build the project:
```bash
npm run build
```

2. Deploy using the deploy script:
```bash
npm run deploy
```

### Manual Setup

1. Build the project:
```bash
npm run build
```

2. Go to your repository Settings → Pages
3. Set source to "Deploy from a branch"
4. Select `gh-pages` branch and `/ (root)` folder
5. Click Save

## Project Structure

```
portfolio/
├── public/
│   └── images/          # Project images
├── src/
│   ├── components/      # React components
│   ├── assets/          # Static assets
│   ├── App.jsx          # Main app component
│   ├── main.jsx         # Entry point
│   └── styles.css       # Global styles
├── .github/workflows/   # GitHub Actions
├── vite.config.js       # Vite configuration
└── package.json         # Dependencies and scripts
```

## Customization

### Adding Projects

Edit `src/components/Projects.jsx` to add new projects:

```jsx
const projects = [
  {
    title: "Your Project",
    description: "Project description",
    tags: ['React', 'Node.js'],
    link: 'https://your-project.com',
    image: './images/your-project.jpg',
    imageAlt: 'Project screenshot',
  },
  // ... more projects
]
```

### Styling

- Colors and themes are defined in CSS variables in `src/styles.css`
- Modify the `:root` selector to change the color scheme
- Add new styles following the existing BEM-like naming convention

### Images

- Place project images in `public/images/`
- Use relative paths like `./images/filename.jpg`
- Images will automatically show fallback placeholders if they fail to load

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

If you have any questions or need help, please open an issue on GitHub.
