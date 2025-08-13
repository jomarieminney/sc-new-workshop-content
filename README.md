# She Codes Australia Workshop Tutorials

Welcome to the She Codes Australia One Day Workshop tutorial content! This repository contains all the learning materials for our hands-on coding workshops.

🌐 **Live Site:** [https://tutorials.shecodes.com.au](https://tutorials.shecodes.com.au)

## Workshop Content

Our tutorials cover the following topics:

- **HTML & CSS** - Learn the building blocks of web development
- **JavaScript** - Interactive programming with our Cupcake Smash game
- **Python** - Space Turtle Chomp adventure and programming fundamentals  
- **Django** - Build a dynamic Bakery Finder web application

## Framework and Tools

- **Hugo** v0.147.9 - Static site generator ([Hugo Documentation](https://gohugo.io/))
- **Hugo Relearn Theme** - Documentation theme ([Theme Documentation](https://mcshelby.github.io/hugo-theme-relearn/))
- **Netlify** - Automated deployment and hosting

## Development Setup

### Prerequisites

- Node.js (for package management)
- Hugo (install via npm or download directly)

### Running Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/SheCodesAustralia/new-workshop-content.git
   cd new-workshop-content
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   # Using npm (recommended)
   npx hugo server
   
   # Or if Hugo is installed globally
   hugo server
   ```

4. **View the site**
   Open your browser to [http://localhost:1313](http://localhost:1313)

The site will automatically reload when you make changes to the content.

## Deployment

Deployment is fully automated via Netlify:

- **Production:** Pushes to `main` branch deploy to [https://tutorials.shecodes.com.au](https://tutorials.shecodes.com.au)
- **Preview:** Other branches create preview deployments at `https://[branch-name]--shecodes-tutorials.netlify.app`

## Content Structure

```
content/
├── html_and_css/          # HTML & CSS workshop materials
├── javascript/            # JavaScript Cupcake Smash game tutorial
├── python/               # Python programming workshop
└── django/               # Django web development tutorial
```

## Contributing

1. Create a new branch for your changes
2. Make your edits to the markdown files in the `content/` directory
3. Test locally with `hugo server`
4. Push your branch to see a preview deployment
5. Create a pull request when ready

## Content Guidelines

- All tutorial content is written in Markdown
- Images should be placed in the appropriate `images/` folder within each section
- Use the Hugo shortcodes provided by the Relearn theme for enhanced formatting
- Test certificate generation functionality when editing certificate pages

## Support

For questions about the workshop content or technical issues, please create an issue in this repository or contact the She Codes Australia team.

---

**She Codes Australia** - Empowering women in technology through education and community.
