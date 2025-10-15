# StreetFreak Website Analytics Setup Guide

## 📊 Google Analytics 4 - Click Tracking System

Your website now has comprehensive click tracking installed. Follow these steps to activate it:

---

## Step 1: Create Google Analytics Account

1. Go to: https://analytics.google.com/
2. Click **"Start measuring"** or **"Admin"** (gear icon)
3. Click **"Create Account"**
   - Account name: `StreetFreak`
   - Configure data sharing settings (optional)
   - Click **"Next"**

## Step 2: Create a Property

1. Property name: `StreetFreak Website`
2. Select timezone: `India`
3. Select currency: `Indian Rupee (₹)`
4. Click **"Next"**

## Step 3: Provide Business Information

1. Industry category: `Retail/Apparel`
2. Business size: Choose appropriate size
3. Select how you plan to use Google Analytics
4. Click **"Create"**
5. Accept Terms of Service

## Step 4: Set Up Data Stream

1. Select **"Web"** as platform
2. Website URL: `https://yourusername.github.io/StreetFreak`
   - Replace `yourusername` with your actual GitHub username
3. Stream name: `StreetFreak Main Site`
4. Click **"Create stream"**

## Step 5: Get Your Measurement ID

1. After creating the stream, you'll see your **Measurement ID**
2. It looks like: `G-XXXXXXXXXX` (starts with G-)
3. **COPY THIS ID** - you'll need it in the next step

## Step 6: Update Your Website Code

1. Open `index.html` in a text editor
2. Find these two lines near the top (around line 10-15):
   ```javascript
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
   ```
   and
   ```javascript
   gtag('config', 'G-XXXXXXXXXX', {
   ```

3. **Replace BOTH occurrences of `G-XXXXXXXXXX`** with your actual Measurement ID
   - Example: If your ID is `G-ABC123XYZ`, change to:
   ```javascript
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-ABC123XYZ"></script>
   ```
   and
   ```javascript
   gtag('config', 'G-ABC123XYZ', {
   ```

4. Save the file

## Step 7: Deploy to GitHub Pages

1. Commit and push your changes to GitHub:
   ```bash
   git add index.html
   git commit -m "Add Google Analytics tracking"
   git push origin main
   ```

2. Make sure GitHub Pages is enabled:
   - Go to your repository on GitHub
   - Settings → Pages
   - Source: Deploy from branch `main`
   - Save

3. Wait 2-3 minutes for deployment

## Step 8: Test Your Analytics

1. Visit your live website: `https://yourusername.github.io/StreetFreak`
2. Go back to Google Analytics
3. Click on **"Reports"** → **"Realtime"**
4. You should see yourself as "1 user right now"
5. Click around your website and watch the real-time data update!

---

## 🎯 What Gets Tracked

Your website now tracks:

### 1. **All Clicks** - Every click is recorded with:
   - Element type (link, button, image, etc.)
   - Element description
   - Page location
   - Timestamp

### 2. **Contact Interactions** - Special tracking for:
   - ✉️ Email clicks (`contact@streetfreak.in`)
   - 📱 Phone clicks (`+91 9372586948`)
   - 📸 Instagram clicks (`@streetfreak.in`)

### 3. **Slideshow Interactions**:
   - Banner arrow clicks
   - Image showcase arrow clicks
   - Image showcase dot clicks (with image number)

### 4. **Game Interactions**:
   - STREETRUNNER game starts
   - Player engagement

### 5. **Automatic Tracking**:
   - Page views
   - Session duration
   - Bounce rate
   - Device type (mobile/desktop)
   - Geographic location
   - Traffic sources

---

## 📈 View Your Analytics Data

### Daily Click Summary
1. Go to Google Analytics
2. **Reports** → **Engagement** → **Events**
3. Look for these events:
   - `click` - All website clicks
   - `contact_click` - Contact info clicks
   - `slideshow_interaction` - Slideshow usage
   - `game_interaction` - Game plays

### Daily Visitor Count
1. **Reports** → **Realtime** (for current visitors)
2. **Reports** → **Acquisition** → **Overview** (for historical data)
3. Select date range to see daily/weekly/monthly stats

### Click Heatmap View
1. **Reports** → **Engagement** → **Events**
2. Click on specific event (e.g., `click`)
3. Add secondary dimension: `Event label`
4. This shows what elements people click most

### Best Time of Day
1. **Reports** → **Engagement** → **Overview**
2. Look at the hourly breakdown graph
3. Helps you know when your visitors are most active

---

## 🔍 Understanding Your Data

### Key Metrics:
- **Users**: Unique visitors per day
- **Sessions**: Total visits (one person can have multiple sessions)
- **Pageviews**: Total page loads
- **Bounce Rate**: % of visitors who leave immediately
- **Average Session Duration**: How long people stay

### Click Data:
- Go to **Events** → Click on `click` event
- See **Event count** for total clicks
- Check **Event label** to see what was clicked
- **Event category** groups related clicks

---

## 📱 Mobile App Alternative (Optional)

Download the **Google Analytics mobile app**:
- iOS: Search "Google Analytics" in App Store
- Android: Search "Google Analytics" in Play Store
- Check your stats on the go!

---

## 🚨 Troubleshooting

### Not Seeing Data?
1. Wait 24-48 hours for data to populate
2. Check **Realtime** report - should show live visitors
3. Verify Measurement ID is correct in both places
4. Make sure you pushed changes to GitHub
5. Clear browser cache and visit site again

### Still Not Working?
1. Open browser Developer Tools (F12)
2. Go to **Console** tab
3. Look for any errors mentioning "gtag" or "analytics"
4. Check **Network** tab for requests to `google-analytics.com`

---

## 📊 Daily Check Routine

Every day, quickly check:
1. Open Google Analytics
2. Click **Realtime** - see current visitors
3. Click **Reports** → **Engagement** → **Events** → Select "Yesterday"
4. Look at total clicks and most clicked elements
5. Check **Acquisition Overview** for visitor count

---

## 🎉 You're All Set!

Your website now tracks every click and visitor automatically. The data is stored forever in Google Analytics, and you can access it anytime from anywhere.

**Important**: Keep your Measurement ID private - don't share it publicly!

---

## Need Help?

If you need assistance:
1. Google Analytics Help Center: https://support.google.com/analytics
2. Check the Realtime report first to test if tracking works
3. Most issues are solved by double-checking the Measurement ID

---

**Created for StreetFreak Website**  
*Last Updated: October 15, 2025*
