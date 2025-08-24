# ActiveShield - Modern Affiliate Website

![ActiveShield Logo](https://img.shields.io/badge/ActiveShield-Safety%20First-blue?style=for-the-badge&logo=shield)

A modern, conversion-optimized affiliate website focused on home security, personal safety, and legal rights education. Built for the activeshield.site domain with a professional dark theme design.

## 🚀 Live Website

Visit us at: **https://activeshield.site**

## 📋 Features

### Core Functionality
- ✅ **Modern Dark Theme Design** - Professional gradient backgrounds and smooth animations
- ✅ **Mobile-First Responsive Design** - Optimized for all devices
- ✅ **Smooth Navigation** - Scroll-to-section functionality
- ✅ **Affiliate Product Showcase** - Ring doorbells, NordVPN, security cameras, and legal services
- ✅ **Educational Resources** - Free guides on legal rights and safety

### SEO & Analytics
- ✅ **SEO Optimized** - Comprehensive meta tags and Open Graph properties
- ✅ **Schema Markup** - Structured data for better search visibility
- ✅ **Google Analytics Ready** - Tracking code placeholder included
- ✅ **Social Media Ready** - Open Graph tags for social sharing

### Conversion Features
- ✅ **Contact Forms** - Working contact and newsletter signup
- ✅ **Trust Elements** - Security badges and testimonials
- ✅ **Urgency Elements** - Countdown timers and limited-time offers
- ✅ **Exit-Intent Popup** - Lead capture for departing visitors
- ✅ **Affiliate Link Tracking** - UTM parameters and analytics integration

## 🛠️ Tech Stack

- **HTML5** - Semantic markup and accessibility
- **CSS3** - Modern styling with flexbox/grid layouts
- **Vanilla JavaScript** - No dependencies for fast loading
- **GitHub Pages** - Simple, reliable hosting

## 🚀 Deployment

### GitHub Pages Setup

1. **Fork this repository** or clone it to your GitHub account
2. **Configure custom domain**:
   - Go to repository Settings → Pages
   - Set source to "Deploy from a branch" → main branch
   - Add your custom domain (e.g., activeshield.site)
3. **Update DNS** (for custom domain):
   ```
   Type: CNAME
   Name: www
   Value: yourusername.github.io
   
   Type: A
   Name: @
   Values: 
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

### Local Development

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/activeshield-site.git
   cd activeshield-site
   ```

2. **Start local server**:
   ```bash
   # Using Python
   python3 -m http.server 8080
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8080
   ```

3. **Open in browser**: `http://localhost:8080`

## ⚙️ Configuration

### Analytics Setup
1. Replace the Google Analytics placeholder in `index.html`:
   ```javascript
   // Replace 'GA_MEASUREMENT_ID' with your actual GA4 ID
   gtag('config', 'GA_MEASUREMENT_ID');
   ```

### Affiliate Links
Update the affiliate URLs in the product cards with your tracking links:
- Ring Security Systems
- NordVPN Services  
- Legal Shield Protection
- Personal Safety Devices
- Dashboard Cameras
- Safety Training Courses

### Contact Form
The contact form uses Formspree by default. To set up:
1. Sign up at [Formspree.io](https://formspree.io)
2. Replace the form action URL with your Formspree endpoint
3. Or integrate with your preferred form handler

## 🎯 Conversion Optimization

### Key Features
- **Urgency Banners** - Limited-time offers and countdown timers
- **Social Proof** - Customer testimonials and trust badges
- **Exit Intent** - Popup to capture leaving visitors
- **Mobile Optimized** - Fast loading on all devices
- **Trust Indicators** - Security badges and guarantees

### Performance
- ⚡ **Fast Loading** - Optimized CSS and minimal JavaScript
- 📱 **Mobile First** - Responsive design for all screen sizes
- 🔍 **SEO Ready** - Meta tags and structured data
- ♿ **Accessible** - ARIA labels and keyboard navigation

## 📊 Analytics & Tracking

The site includes comprehensive tracking for:
- Page views and user engagement
- Affiliate link clicks and conversions
- Form submissions and newsletter signups
- Exit intent and popup interactions

## 🔒 Legal & Compliance

- **Affiliate Disclosure** - Clearly stated on all pages
- **Privacy Policy** - Link in footer (add your own)
- **Terms of Service** - Link in footer (add your own)
- **Educational Disclaimer** - Not legal advice notice

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit changes: `git commit -am 'Add feature'`
4. Push to branch: `git push origin feature-name`
5. Submit a pull request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Support

For questions about setup or customization:
- 📧 Email: support@activeshield.site
- 🐛 Issues: [GitHub Issues](https://github.com/yourusername/activeshield-site/issues)
- 💬 Discussions: [GitHub Discussions](https://github.com/yourusername/activeshield-site/discussions)

---

**⚠️ Important**: This website is for educational purposes and should not be considered legal advice. Always consult with qualified professionals for specific legal or safety concerns.

**💡 Affiliate Notice**: We may earn a commission from purchases made through our recommended links. This helps support our educational content at no extra cost to you.