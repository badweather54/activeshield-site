# 🛡️ ActiveShield - Modern Affiliate Website

A professional, high-converting affiliate website for safety products and legal education resources. Built with modern web standards, mobile-first design, and comprehensive tracking.

## 🌟 Features

### 🎯 Conversion-Optimized
- **Urgency banners** with real-time countdown timers
- **Exit-intent popups** to capture leaving visitors
- **Social proof** with ratings and testimonials
- **Trust badges** and security indicators
- **Compelling CTAs** with hover animations
- **Limited time offers** and discount pricing

### 📱 Mobile-First Responsive Design
- **Breakpoints**: 768px (tablet), 480px (mobile)
- **Touch-friendly** navigation and buttons
- **Optimized typography** scaling with clamp()
- **Flexible grid layouts** with CSS Grid and Flexbox
- **Mobile menu** with hamburger toggle

### 🔍 SEO & Performance Optimized
- **Schema markup** (Organization, LocalBusiness)
- **Open Graph** and Twitter Card meta tags
- **Semantic HTML5** structure
- **Loading animations** and skeleton screens
- **Lazy loading** for images (when applicable)
- **Optimized fonts** with system font stack

### ♿ Accessibility Features
- **ARIA labels** and descriptions
- **Skip links** for keyboard navigation
- **Focus management** and visible focus indicators
- **Screen reader support** with semantic markup
- **High contrast mode** support
- **Reduced motion** preferences respected

### 📊 Analytics & Tracking
- **Google Analytics 4** integration
- **Affiliate link tracking** with UTM parameters
- **Event tracking** for conversions and interactions
- **Form submission** tracking
- **Download tracking** for resources
- **Exit intent** and popup interaction tracking

### 🛒 Affiliate Integration
- **Amazon Associates** ready links
- **Multiple affiliate networks** supported
- **UTM parameter** tracking for attribution
- **Product recommendations** with ratings
- **Price comparison** and discount highlighting
- **FTC compliant** disclosure statements

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/badweather54/activeshield-site.git
cd activeshield-site
```

### 2. Set Up Your Domain
The site is configured for `activeshield.site`. Update the CNAME file if using a different domain:
```bash
echo "yourdomain.com" > CNAME
```

### 3. Configure Google Analytics
1. Replace `GA_MEASUREMENT_ID` in the Google Analytics script with your actual GA4 measurement ID
2. Update the gtag configuration in `index.html`

### 4. Update Affiliate Links
Replace the example affiliate links with your actual affiliate URLs:
- Amazon Associates links
- LegalShield affiliate URLs  
- NordVPN affiliate links
- Other affiliate network URLs

### 5. Customize Content
- Update product descriptions and pricing
- Add your own testimonials
- Customize the urgency banner messaging
- Update social media links in the footer

## 📁 File Structure

```
activeshield-site/
├── index.html          # Main website file (complete with CSS/JS)
├── CNAME              # Custom domain configuration
├── .gitignore         # Git ignore rules
└── README.md          # This documentation
```

## 🔧 Configuration

### Google Analytics Setup
1. Create a GA4 property at [Google Analytics](https://analytics.google.com)
2. Get your Measurement ID (format: G-XXXXXXXXXX)
3. Replace `GA_MEASUREMENT_ID` in the HTML file:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

### Affiliate Link Configuration
Update all affiliate links with your tracking parameters:

**Amazon Associates:**
```html
href="https://amazon.com/dp/PRODUCT_ID?tag=YOUR_TAG-20&utm_source=activeshield&utm_medium=affiliate&utm_campaign=CAMPAIGN_NAME"
```

**Other Networks:**
Add your affiliate ID and tracking parameters to each link.

### Email Integration
The contact form and newsletter signup are currently set up for frontend validation only. To enable backend processing:

1. **Option 1: Formspree**
   - Sign up at [Formspree](https://formspree.io)
   - Update form action: `<form action="https://formspree.io/f/YOUR_ID">`

2. **Option 2: Netlify Forms**
   - Add `netlify` attribute to forms: `<form netlify>`
   - Deploy on Netlify for automatic form processing

3. **Option 3: Custom Backend**
   - Set up your own form processing endpoint
   - Update form actions accordingly

## 🚀 Deployment

### GitHub Pages (Recommended)
1. Fork this repository
2. Go to Settings > Pages
3. Select "Deploy from a branch"
4. Choose "main" branch
5. Your site will be available at `https://username.github.io/activeshield-site`

### Custom Domain Setup
1. Update CNAME file with your domain
2. Configure DNS A records to point to GitHub Pages:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
3. Wait for DNS propagation (up to 24 hours)

### Alternative Deployment Options

**Netlify:**
1. Connect your GitHub repository to Netlify
2. Set build command to `` (empty, since it's a static site)
3. Set publish directory to `/`

**Vercel:**
1. Import your GitHub repository to Vercel
2. No additional configuration needed

**Traditional Hosting:**
1. Upload all files to your web server
2. Ensure index.html is in the root directory

## 🎨 Customization

### Colors & Branding
Update CSS custom properties in the `:root` selector:
```css
:root {
    --primary-color: #667eea;    /* Main brand color */
    --secondary-color: #764ba2;  /* Secondary brand color */
    --accent-color: #2196f3;     /* Accent color */
    --success-color: #4caf50;    /* Success/positive actions */
    --warning-color: #ff9800;    /* Warnings/attention */
    --danger-color: #e74c3c;     /* Errors/urgent actions */
}
```

### Typography
The site uses a system font stack for optimal performance:
```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
```

To use custom fonts, add Google Fonts or other web fonts to the `<head>` section.

### Content Updates
- **Products**: Update the product grid in the `#products` section
- **Testimonials**: Modify the testimonial cards in the `#testimonials` section
- **Resources**: Update educational resources in the `#education` section
- **Contact Info**: Update footer and contact section with your information

## 📊 Analytics Events Tracked

The site automatically tracks these events:

| Event Name | Description | Category |
|------------|-------------|----------|
| `purchase_intent` | Affiliate link clicks | `affiliate_click` |
| `file_download` | Resource downloads | `resource_download` |
| `form_submit` | Contact form submissions | `contact_form` |
| `newsletter_signup` | Newsletter subscriptions | `engagement` |
| `popup_show` | Exit intent popup displays | `exit_intent` |
| `lead_generation` | Exit intent conversions | `exit_intent_conversion` |

## 🔒 Privacy & Compliance

### GDPR Compliance
- Add a cookie consent banner if serving EU users
- Update privacy policy with data collection details
- Implement opt-out mechanisms for tracking

### FTC Compliance
- Affiliate disclosures are included and prominent
- All affiliate links are marked with `rel="nofollow"`
- Transparent about compensation from affiliate links

### Accessibility Compliance
- WCAG 2.1 AA compliant design
- Keyboard navigation support
- Screen reader compatibility
- High contrast mode support

## 🛠️ Development

### Local Development
Since this is a static HTML file, you can:

1. **Simple**: Open `index.html` directly in a browser
2. **With Live Reload**: Use a local server:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Node.js (with http-server)
   npx http-server .
   
   # PHP
   php -S localhost:8000
   ```

### Performance Testing
Test your site with:
- [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [GTmetrix](https://gtmetrix.com/)
- [WebPageTest](https://webpagetest.org/)

### SEO Testing
Validate your SEO with:
- [Google Search Console](https://search.google.com/search-console)
- [Schema Markup Validator](https://validator.schema.org/)
- [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/)

## 📞 Support

### Common Issues

**Q: Affiliate links not tracking properly**
A: Ensure UTM parameters are correctly formatted and your affiliate network supports them.

**Q: Forms not submitting**
A: Set up a backend service (Formspree, Netlify Forms, etc.) as the frontend-only validation is for demo purposes.

**Q: Mobile menu not working**
A: Check that JavaScript is enabled and there are no console errors.

**Q: Countdown timer not updating**
A: Verify JavaScript is running and there are no blocking errors in the console.

### Need Help?
- Check the [Issues](https://github.com/badweather54/activeshield-site/issues) section
- Create a new issue with detailed description
- Review browser console for JavaScript errors

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Links

- **Live Site**: [https://activeshield.site](https://activeshield.site)
- **Repository**: [https://github.com/badweather54/activeshield-site](https://github.com/badweather54/activeshield-site)
- **Issues**: [https://github.com/badweather54/activeshield-site/issues](https://github.com/badweather54/activeshield-site/issues)

---

**Built with ❤️ for safer communities**

*Last updated: January 2025*