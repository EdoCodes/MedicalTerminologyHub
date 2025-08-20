# Deployment Guide

This document explains how to deploy the Medical Terminology Hub to various platforms.

## 🚀 Deployment Options

### Netlify (Recommended)

1. **Connect your GitHub repository** to Netlify
2. **Build settings**:
   - Build command: `npm run build`
   - Publish directory: `dist`
3. **Deploy**: Netlify will automatically build and deploy

### Vercel

1. **Import your GitHub repository** to Vercel
2. **Framework preset**: Astro
3. **Build settings** are automatically detected
4. **Deploy**: Vercel handles the rest

### GitHub Pages

1. **Enable GitHub Pages** in repository settings
2. **Add GitHub Actions workflow**:
   ```yaml
   # .github/workflows/deploy.yml
   name: Deploy to GitHub Pages
   
   on:
     push:
       branches: [ main ]
   
   jobs:
     build:
       runs-on: ubuntu-latest
       steps:
         - uses: actions/checkout@v3
         - uses: actions/setup-node@v3
           with:
             node-version: 18
         - run: npm install
         - run: npm run build
         - uses: actions/deploy-pages@v1
           with:
             artifact_name: github-pages
             path: dist
   ```

### Manual Deployment

1. **Build the project**:
   ```bash
   npm run build
   ```

2. **Upload the `dist` folder** to your web server

## 🔧 Build Configuration

The project uses Astro's static site generation:

```javascript
// astro.config.mjs
export default defineConfig({
  integrations: [tailwind()],
  output: 'static',
  build: {
    inlineStylesheets: 'auto'
  }
});
```

## 🌐 Custom Domain

To use a custom domain:

1. **Configure DNS** to point to your hosting provider
2. **Update canonical URLs** in the HTML meta tags
3. **Update sitemap** if using one
4. **Test thoroughly** after domain change

## 📊 Performance Optimization

The build process automatically:
- Minifies CSS and JavaScript
- Optimizes images
- Generates static HTML
- Inlines critical CSS
- Creates efficient bundles

## 🔍 SEO Considerations

After deployment:
- Submit sitemap to search engines
- Verify meta tags are correct
- Test social media previews
- Monitor Core Web Vitals
- Check mobile usability

## 🛠️ Troubleshooting

### Common Issues

**Build fails with Tailwind errors**:
- Ensure all Tailwind classes are valid
- Check `tailwind.config.mjs` content paths

**JavaScript not working**:
- Verify all script tags are properly included
- Check browser console for errors

**Styles not loading**:
- Confirm CSS files are in the correct location
- Check build output for CSS files

### Environment Variables

This project doesn't require environment variables for basic functionality. If you add features that need them:

1. Create `.env.example` file
2. Document required variables
3. Add `.env` to `.gitignore`

## 📈 Analytics

To add analytics:

1. **Google Analytics**:
   ```html
   <!-- Add to <head> in index.astro -->
   <script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
   ```

2. **Plausible Analytics** (privacy-friendly):
   ```html
   <script defer data-domain="yourdomain.com" src="https://plausible.io/js/script.js"></script>
   ```

## 🔒 Security

- No sensitive data is stored client-side
- All content is static and safe
- Regular dependency updates recommended
- HTTPS is enforced on all hosting platforms

---

For deployment questions, check the hosting provider's documentation or open an issue in this repository.