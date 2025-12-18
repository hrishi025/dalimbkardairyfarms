# Dalimbkar Dairy Farms Website

A professional, modern, and responsive static website showcasing premium dairy products from Dalimbkar Dairy Farms.

## 🌟 Features

- ✨ **Modern Design**: Professional aesthetics with smooth gradients and glassmorphism effects
- 🎭 **Smooth Animations**: Scroll-triggered animations, parallax effects, and hover interactions
- 📱 **Fully Responsive**: Optimized for mobile, tablet, and desktop devices
- 🚀 **Performance Optimized**: Fast loading with lazy loading and debounced scroll events
- ♿ **SEO Friendly**: Proper meta tags, semantic HTML, and accessibility features

## 📁 Project Structure

```
ddf/
├── index.html          # Main HTML file with all sections
├── styles.css          # Professional CSS with animations
├── script.js           # Interactive JavaScript features
├── images/             # Product and hero images
│   ├── hero.png
│   └── ghee.png
└── README.md           # This file
```

## 🔧 How to Use

### Local Development

1. **Open Locally**: Simply open `index.html` in any modern web browser
2. **Use Local Server** (Recommended for testing):
   ```bash
   # Using Python 3
   python3 -m http.server 8000
   
   # Using Node.js (if you have it)
   npx serve
   ```
   Then visit `http://localhost:8000` in your browser

### Updating Content

#### Update Contact Information
Open `index.html` and search for these placeholders to update:
- `[Your Complete Address]` - Replace with actual address
- `[Your Phone Number]` - Replace with actual phone number (in multiple places)
- `info@dalimbkardairyfarms.in` - Update if using different email

#### Update Pricing
Find the pricing section in `index.html` and update the prices as needed.

#### Update Social Media Links
Find the social icons section and update the `href` attributes:
```html
<a href="https://facebook.com/yourpage" class="social-icon">
```

#### Add Google Maps
1. Get your Google Maps embed code
2. Replace the `.map-placeholder` div in the Location section with:
```html
<iframe src="YOUR_GOOGLE_MAPS_EMBED_URL" 
        width="100%" 
        height="100%" 
        style="border:0; border-radius: 24px;" 
        allowfullscreen="" 
        loading="lazy">
</iframe>
```

## 🚀 Deployment Options

### Option 1: GitHub Pages (Recommended)

1. **Create a GitHub Repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/dalimbkar-dairy.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Select `main` branch as source
   - Save and wait for deployment
   - Your site will be at: `https://yourusername.github.io/dalimbkar-dairy`

3. **Connect Custom Domain**
   - Add a `CNAME` file with content: `www.dalimbkardairyfarms.in`
   - In your GoDaddy domain settings:
     - Add CNAME record: `www` → `yourusername.github.io`
     - Add A records pointing to GitHub IPs:
       - `185.199.108.153`
       - `185.199.109.153`
       - `185.199.110.153`
       - `185.199.111.153`

### Option 2: Netlify (Easy & Fast)

1. **Drag & Drop Deployment**
   - Visit [netlify.com](https://netlify.com)
   - Drag your project folder to Netlify Drop
   - Get instant deployment

2. **Git-based Deployment**
   ```bash
   netlify init
   netlify deploy --prod
   ```

3. **Connect Custom Domain**
   - In Netlify dashboard: Domain Settings → Add custom domain
   - Follow DNS configuration instructions
   - Update GoDaddy DNS:
     - Add CNAME: `www` → `yoursite.netlify.app`

### Option 3: Vercel

1. **Install Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **Deploy**
   ```bash
   vercel
   ```

3. **Connect Domain**
   - In Vercel dashboard: Settings → Domains
   - Add `www.dalimbkardairyfarms.in`
   - Update GoDaddy DNS as instructed

### Option 4: Google Sites Alternative

While Google Sites doesn't support custom HTML/CSS directly, you can:
1. Use **Firebase Hosting** (Google's service):
   ```bash
   npm install -g firebase-tools
   firebase login
   firebase init hosting
   firebase deploy
   ```

2. Connect your GoDaddy domain:
   - In Firebase Console: Hosting → Add custom domain
   - Update GoDaddy DNS records as shown

## 🎨 Customization

### Colors
Edit CSS variables in `styles.css`:
```css
:root {
    --primary-color: #2d7a4f;    /* Main green color */
    --secondary-color: #f4a261;  /* Accent orange */
    --accent-color: #e76f51;     /* Highlight red */
}
```

### Fonts
Current fonts: Poppins (headings) and Inter (body text)
To change, update the Google Fonts import in `index.html` and CSS variables.

### Images
- Replace images in the `images/` folder
- Keep the same filenames or update references in `index.html`
- Recommended sizes:
  - Hero image: 1920x1080px
  - Product images: 800x600px

## 📧 Contact Form Setup

The contact form currently shows a success message without sending emails. To make it functional:

### Option A: Using Formspree (Easiest)
1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form and get your endpoint
3. Update the form in `index.html`:
   ```html
   <form id="contact-form" action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
   ```
4. Comment out the JavaScript form handler in `script.js`

### Option B: Using EmailJS
1. Sign up at [emailjs.com](https://emailjs.com)
2. Follow their integration guide
3. Update the form submission code in `script.js`

### Option C: Backend API
Create your own backend endpoint and update the fetch URL in `script.js`.

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 TODO / Future Enhancements

- [ ] Add actual product images (replace icon placeholders)
- [ ] Integrate Google Analytics for tracking
- [ ] Add product image gallery/lightbox
- [ ] Implement blog section for farm updates
- [ ] Add customer testimonials section
- [ ] Create product ordering system
- [ ] Add multi-language support
- [ ] Integrate WhatsApp Business API

## 📞 Support

For questions or issues with the website, contact:
- Email: info@dalimbkardairyfarms.in
- Phone: [Your Phone Number]

## 📄 License

© 2024 Dalimbkar Dairy Farms. All rights reserved.

---

**Made with ❤️ for quality dairy products**