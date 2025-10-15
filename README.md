# StreetFreak Marketplace 🚀

A modern, interactive maintenance/landing page for StreetFreak clothing brand with real-time analytics tracking.

![StreetFreak](https://img.shields.io/badge/StreetFreak-Marketplace-purple?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![Analytics](https://img.shields.io/badge/Analytics-Enabled-blue?style=for-the-badge)

## 🌟 Features

### Interactive Elements
- **Custom Purple Crosshair Cursor** - Unique cursor with trail effects for enhanced user experience
- **Auto-Rotating Banner** - Showcase promotional content with smooth transitions
- **Image Showcase Slideshow** - Display 12 product images with navigation controls
- **STREETRUNNER Mini Game** - Built-in endless runner game to engage visitors
- **Real-time Progress Tracking** - Visual progress bar showing upgrade completion (78%)

### Analytics & Tracking
- **Google Analytics 4 Integration** - Comprehensive visitor tracking
- **Click Event Tracking** - Monitor every user interaction
- **Contact Engagement Tracking** - Track email, phone, and Instagram clicks
- **Slideshow Interaction Analytics** - Measure engagement with product images
- **Game Performance Metrics** - Track game plays and user retention

### Design Highlights
- **Futuristic White Theme** - Clean, modern aesthetic with Space Grotesk font
- **Responsive Design** - Fully optimized for mobile and desktop
- **Touch Gesture Support** - Swipe controls for mobile users
- **Keyboard Navigation** - Arrow keys for slideshow control
- **Smooth Animations** - CSS animations throughout for polished experience

## 📁 Project Structure

```
StreetFreak/
├── index.html                    # Main landing page
├── ANALYTICS_SETUP.md           # Google Analytics setup guide
├── README.md                     # This file
├── LICENSE                       # MIT License
├── StreetFreak_logo.svg         # Main logo
├── StreetFreak(B2B).svg         # B2B division logo
├── BANNER/
│   ├── 1.png                    # Banner image 1
│   └── 2.png                    # Banner image 2 (default)
├── images/
│   ├── 2.png                    # Product image 1
│   ├── 3.png                    # Product image 2
│   ├── 4.png                    # Product image 3
│   ├── 5.png                    # Product image 4
│   ├── 6.png                    # Product image 5
│   ├── 7.png                    # Product image 6
│   ├── 8.png                    # Product image 7
│   ├── 9.png                    # Product image 8
│   ├── 10.png                   # Product image 9
│   ├── 11.png                   # Product image 10
│   ├── 12.png                   # Product image 11
│   └── 13.png                   # Product image 12
└── league-spartan-master/       # Font files
    └── webfonts/
        └── stylesheet.css       # League Spartan font
```

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/StreetFreak.git
cd StreetFreak
```

### 2. Open Locally
Simply open `index.html` in your browser:
```bash
open index.html  # macOS
# or
start index.html # Windows
# or
xdg-open index.html # Linux
```

### 3. Deploy to GitHub Pages

1. Push to GitHub:
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. Enable GitHub Pages:
   - Go to repository Settings
   - Navigate to Pages section
   - Select source: `Deploy from branch main`
   - Save

3. Access your site at: `https://yourusername.github.io/StreetFreak`

## 📊 Analytics Setup

Google Analytics 4 is pre-configured with ID: **G-7RGPMYTM52**

For detailed setup instructions, see [ANALYTICS_SETUP.md](ANALYTICS_SETUP.md)

### What Gets Tracked:
- ✅ Page views and session duration
- ✅ All click events with element identification
- ✅ Contact information clicks (email, phone, Instagram)
- ✅ Banner slideshow interactions
- ✅ Image showcase navigation
- ✅ STREETRUNNER game starts and plays
- ✅ Device types and geographic locations
- ✅ Traffic sources and bounce rates

## 🎮 STREETRUNNER Game

Built-in mini-game at the bottom of the page:
- **Controls**: SPACEBAR, UP ARROW, or TAP/CLICK to jump
- **Objective**: Avoid obstacles and score points
- **Features**: High score tracking with localStorage persistence
- **Mobile-friendly**: Touch controls and optimized speed

## 🎨 Customization

### Update Logo
Replace `StreetFreak_logo.svg` and `StreetFreak(B2B).svg` with your own logos.

### Change Colors
Primary color variables in CSS:
```css
#ffffff - White background
#2b2b2b - Dark accent
#5b47ff - Purple brand color
#4c3aff - Dark purple
#f5f5f5 - Light gray
```

### Update Banner Images
Add or replace images in the `BANNER/` folder. Update slideshow in HTML:
```javascript
const bannerSlides = document.querySelectorAll('.banner-slide');
```

### Modify Product Images
Add or replace images in the `images/` folder (2.png through 13.png).

### Adjust Progress Bar
Change completion percentage in CSS:
```css
@keyframes progressAnimation {
    to { width: 78%; } /* Change this value */
}
```

## 📱 Contact Information

Update contact details in the HTML:
- **Email**: contact@streetfreak.in
- **Phone**: +91 9372586948
- **Instagram**: @streetfreak.in

Find and replace these values in `index.html`.

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with animations and transitions
- **JavaScript (Vanilla)** - Interactive features and game logic
- **Google Analytics 4** - Visitor tracking and analytics
- **Space Grotesk Font** - From Google Fonts
- **League Spartan Font** - Local font files

## 🌐 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Company Information

**StreetFreak Clothing LLP**

📍 **Location**  
T4 , Prem Sagar Building,  
Subhash Nagar, Jawahar Nagar,  
Goregaon West, Mumbai - 400104

⏰ **Working Hours**  
Monday - Saturday: 10:00 AM - 7:00 PM  
Sunday: Closed

## 🤝 Contributing

This is a private company website. For inquiries, please contact us through the methods listed above.

## 📞 Support

For technical support or business inquiries:
- 📧 Email: contact@streetfreak.in
- 📱 Phone: +91 9372586948
- 📸 Instagram: [@streetfreak.in](https://instagram.com/streetfreak.in)

## 🎯 Roadmap

- [x] Interactive landing page
- [x] Product image showcase
- [x] Analytics integration
- [x] Mini game feature
- [x] Mobile optimization
- [ ] Full e-commerce integration
- [ ] Product catalog launch
- [ ] Online payment gateway
- [ ] Customer dashboard

## 📈 Performance

- **Page Load**: < 2 seconds
- **Mobile-First**: Fully responsive design
- **SEO Optimized**: Meta tags and semantic HTML
- **Analytics**: Real-time tracking enabled

## 🔐 Privacy

This website uses Google Analytics to collect anonymous usage data. No personal information is stored without consent. For more information, see our privacy practices in the analytics setup.

## 📝 Notes

- This is a maintenance/landing page during website upgrade
- Full marketplace coming soon
- B2B services available - contact for details
- Current progress: 78% complete

---

**Made with 💜 by StreetFreak Team**

*Last Updated: October 15, 2025*
