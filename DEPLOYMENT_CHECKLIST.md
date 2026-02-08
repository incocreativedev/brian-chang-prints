# 🚀 Deployment Checklist

Follow this checklist to launch your photography print shop successfully.

---

## ✅ Phase 1: Pre-Launch Setup

### 1. Airtable Configuration
- [ ] Create Airtable base following `AIRTABLE_SETUP.md`
- [ ] Upload at least 2-3 albums with 10-15 photos total
- [ ] Add watermarked and original versions of all photos
- [ ] Write descriptions for all albums
- [ ] Write stories for key photos
- [ ] Mark 2-3 albums as "Featured"
- [ ] Set "Available for Sale" checkbox on all prints
- [ ] Test Airtable Personal Access Token and Base ID

### 2. Content Preparation
- [ ] Watermark all gallery images with 张 logo (15-20% opacity)
- [ ] Resize images for web (1200-1600px wide, <300kb)
- [ ] Keep original high-res files for Phase 2
- [ ] Write "About Me" content (update `src/pages/About.jsx` if needed)
- [ ] Choose domain name (e.g., brianchangprints.com)

### 3. Site Configuration
- [ ] Update contact email in `src/constants/index.js`
- [ ] Verify Instagram handle is correct
- [ ] Review all site copy and branding
- [ ] Test all navigation links
- [ ] Review SEO meta tags in `index.html`

### 4. Local Testing
- [ ] Install dependencies: `npm install`
- [ ] Add `.env` file with Airtable credentials
- [ ] Run dev server: `npm run dev`
- [ ] Test homepage loads with featured albums
- [ ] Test all album pages load correctly
- [ ] Test photo lightbox (keyboard nav, zoom, thumbnails)
- [ ] Test mobile responsiveness (iPhone, Android)
- [ ] Test on different browsers (Chrome, Safari, Firefox)
- [ ] Check loading speeds (<3 seconds)
- [ ] Verify watermarks are visible but not obtrusive

---

## 🌐 Phase 2: Deployment

### 1. Version Control
- [ ] Initialize git: `git init`
- [ ] Create `.gitignore` (already included)
- [ ] Commit all files: `git add . && git commit -m "Initial commit"`
- [ ] Create GitHub repository
- [ ] Push to GitHub: `git push -u origin main`

### 2. Vercel Deployment
- [ ] Sign up at [vercel.com](https://vercel.com) (free)
- [ ] Click "New Project"
- [ ] Import from GitHub
- [ ] Vercel auto-detects Vite (no config needed)
- [ ] Add environment variables:
  - `VITE_AIRTABLE_API_KEY` = your token
  - `VITE_AIRTABLE_BASE_ID` = your base ID
- [ ] Click "Deploy"
- [ ] Wait 2-3 minutes for build
- [ ] Test live site at `your-project.vercel.app`

### 3. Custom Domain (Optional)
- [ ] Purchase domain (brianchangprints.com)
- [ ] In Vercel → Project Settings → Domains
- [ ] Add custom domain
- [ ] Update DNS records at your registrar:
  - Type: `A`, Name: `@`, Value: `76.76.21.21`
  - Type: `CNAME`, Name: `www`, Value: `cname.vercel-dns.com`
- [ ] Wait 24-48 hours for DNS propagation
- [ ] Verify SSL certificate is active (automatic)

---

## 🧪 Phase 3: Post-Launch Testing

### 1. Functional Testing
- [ ] Visit live site from multiple devices
- [ ] Test all pages load correctly
- [ ] Verify images load and display properly
- [ ] Check navigation and all links work
- [ ] Test lightbox on mobile (swipe gestures)
- [ ] Verify Airtable data updates reflect on site

### 2. Performance Testing
- [ ] Run Google Lighthouse audit (target: 90+ scores)
- [ ] Check PageSpeed Insights
- [ ] Test loading speed from different locations
- [ ] Verify images are optimized

### 3. SEO Setup
- [ ] Submit sitemap to Google Search Console
- [ ] Verify meta tags are correct
- [ ] Test Open Graph preview (Facebook, Twitter)
- [ ] Set up Google Analytics (optional)

---

## 📢 Phase 4: Marketing Launch

### 1. Social Media
- [ ] Update Instagram bio with website link
- [ ] Create announcement post about print shop
- [ ] Share featured albums/photos with website links
- [ ] Add website to all social profiles

### 2. Content Strategy
- [ ] Plan new album releases
- [ ] Set schedule for uploading new photos
- [ ] Consider email newsletter (Phase 3 feature)

### 3. Promotion
- [ ] Paid Instagram/Facebook ads (optional)
- [ ] Reach out to photography communities
- [ ] Consider collaborations with interior designers
- [ ] Look into Airbnb host partnerships

---

## 🔄 Ongoing Maintenance

### Weekly
- [ ] Upload new photos to keep content fresh
- [ ] Monitor site performance
- [ ] Check for broken links

### Monthly
- [ ] Review analytics (if set up)
- [ ] Update featured albums
- [ ] Refresh homepage hero image

### As Needed
- [ ] Respond to customer inquiries
- [ ] Update About page with new projects
- [ ] Add new albums for seasonal content

---

## 🆘 Troubleshooting

### Site Not Loading?
1. Check environment variables in Vercel
2. Verify Airtable API key is valid
3. Check browser console for errors

### Photos Not Displaying?
1. Verify Airtable attachments are uploaded
2. Check field names match exactly (case-sensitive)
3. Ensure "Available for Sale" is checked

### Build Failing?
1. Run `npm run build` locally to test
2. Check Vercel build logs for errors
3. Verify all dependencies are in `package.json`

---

## 📞 Need Help?

If you encounter issues:
1. Check `README.md` for documentation
2. Review `AIRTABLE_SETUP.md` for database help
3. Check Vercel deployment logs
4. Google the specific error message

---

**Good luck with your launch! 🎉**

Remember: Phase 1 is about showcasing your work beautifully. Phase 2 will add the e-commerce functionality.
