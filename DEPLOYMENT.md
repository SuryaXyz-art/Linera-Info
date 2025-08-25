# Deployment Guide - Linera Protocol Website

This guide provides instructions for deploying the Linera Protocol website to various hosting platforms.

## 🚀 Quick Start

### Local Development
1. Download all files to your local machine
2. Open `index.html` in your web browser
3. The website should load immediately with all features working

### File Requirements
Ensure you have all these files in the same directory:
- `index.html` - Main HTML file
- `styles.css` - CSS styles
- `script.js` - JavaScript functionality
- `README.md` - Documentation
- `DEPLOYMENT.md` - This deployment guide

## 🌐 Hosting Options

### 1. GitHub Pages (Free)

**Steps:**
1. Create a new GitHub repository
2. Upload all website files to the repository
3. Go to Settings > Pages
4. Select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"
7. Your site will be available at `https://yourusername.github.io/repository-name`

**Advantages:**
- Free hosting
- Automatic HTTPS
- Custom domain support
- Easy updates via Git

### 2. Netlify (Free Tier)

**Steps:**
1. Sign up for Netlify
2. Drag and drop your website folder to Netlify's deploy area
3. Your site will be live instantly
4. Customize the URL in site settings

**Advantages:**
- Free tier available
- Automatic deployments
- Custom domain support
- Form handling
- CDN distribution

### 3. Vercel (Free Tier)

**Steps:**
1. Sign up for Vercel
2. Install Vercel CLI: `npm i -g vercel`
3. Navigate to your website directory
4. Run `vercel`
5. Follow the prompts

**Advantages:**
- Free tier available
- Automatic deployments
- Edge network
- Custom domain support

### 4. Traditional Web Hosting

**Steps:**
1. Purchase web hosting (e.g., Bluehost, HostGator, SiteGround)
2. Access your hosting control panel
3. Upload files via FTP or file manager
4. Point your domain to the hosting

**File Upload:**
- Upload all files to the `public_html` or `www` directory
- Ensure `index.html` is in the root directory

### 5. AWS S3 + CloudFront

**Steps:**
1. Create an S3 bucket
2. Enable static website hosting
3. Upload all files to the bucket
4. Configure CloudFront for CDN
5. Set up custom domain (optional)

**Advantages:**
- Highly scalable
- Global CDN
- Cost-effective for high traffic
- Custom domain support

## 🔧 Configuration

### Custom Domain Setup

1. **Purchase a domain** (e.g., from Namecheap, GoDaddy, Google Domains)
2. **Configure DNS:**
   - For GitHub Pages: Add CNAME record pointing to `yourusername.github.io`
   - For Netlify: Add CNAME record pointing to your Netlify URL
   - For Vercel: Add CNAME record pointing to your Vercel URL

### SSL/HTTPS

Most modern hosting platforms provide automatic SSL certificates:
- **GitHub Pages**: Automatic HTTPS
- **Netlify**: Automatic HTTPS
- **Vercel**: Automatic HTTPS
- **Traditional hosting**: Usually included or can be enabled

### Performance Optimization

1. **Enable Gzip compression** (usually automatic on modern platforms)
2. **Set up caching headers** for static assets
3. **Use CDN** for global distribution
4. **Optimize images** if you add any

## 📊 Analytics Setup

### Google Analytics

1. Create a Google Analytics account
2. Get your tracking ID
3. Add this code to the `<head>` section of `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Other Analytics Options

- **Plausible Analytics**: Privacy-focused analytics
- **Fathom Analytics**: Simple, privacy-friendly analytics
- **Matomo**: Self-hosted analytics solution

## 🔍 SEO Optimization

The website already includes:
- Meta tags for SEO
- Open Graph tags for social sharing
- Twitter Card tags
- Semantic HTML structure
- Proper heading hierarchy

### Additional SEO Steps

1. **Submit sitemap** to search engines
2. **Register with Google Search Console**
3. **Set up Bing Webmaster Tools**
4. **Add structured data** if needed

## 🚨 Troubleshooting

### Common Issues

1. **Website not loading:**
   - Check file permissions
   - Ensure all files are uploaded
   - Verify `index.html` is in the root directory

2. **Styles not loading:**
   - Check file paths in HTML
   - Ensure `styles.css` is uploaded
   - Clear browser cache

3. **JavaScript not working:**
   - Check browser console for errors
   - Ensure `script.js` is uploaded
   - Verify file paths

4. **Mobile menu not working:**
   - Check if JavaScript is enabled
   - Verify `script.js` is loaded
   - Test on different devices

### Performance Issues

1. **Slow loading:**
   - Enable Gzip compression
   - Use CDN for external resources
   - Optimize images
   - Minimize HTTP requests

2. **Layout issues:**
   - Test on different browsers
   - Check responsive breakpoints
   - Verify CSS is loading properly

## 📱 Testing Checklist

Before going live, test:

- [ ] Desktop browsers (Chrome, Firefox, Safari, Edge)
- [ ] Mobile devices (iOS Safari, Android Chrome)
- [ ] Tablet devices
- [ ] Navigation functionality
- [ ] Form submission
- [ ] Responsive design
- [ ] Loading animations
- [ ] Touch gestures (mobile)
- [ ] Keyboard navigation
- [ ] Screen reader compatibility

## 🔄 Updates and Maintenance

### Regular Updates

1. **Content updates:** Edit HTML files directly
2. **Style changes:** Modify CSS files
3. **Functionality updates:** Edit JavaScript files
4. **Deploy changes:** Upload updated files to your hosting platform

### Version Control

Consider using Git for version control:
1. Initialize Git repository
2. Commit changes regularly
3. Use branches for major updates
4. Tag releases for important versions

## 📞 Support

For deployment issues:
1. Check hosting provider documentation
2. Review browser console for errors
3. Test on different devices and browsers
4. Contact hosting provider support

---

**Happy Deploying! 🚀**
