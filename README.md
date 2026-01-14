# TEJASE Booking System - Complete Prototype

## 🎯 What This Is

A **fully functional prototype** of the TEJASE Healing Arts booking system with **integrated custom background images** that work across all pages.

## ✨ Features

### Working Features
✅ **Custom Background Images** - Upload and see them on ALL pages
✅ **Client Booking System** - 3-step booking process
✅ **Admin Dashboard** - Manage appointments and view calendar
✅ **Settings Page** - Customize services, hours, contact info
✅ **Time Blocking** - Block vacation days, lunch breaks
✅ **Responsive Design** - Works on iPad, mobile, desktop
✅ **TEJASE Branding** - Healing arts color scheme

### Background Image Integration
- Upload in Settings
- Appears on Index, Client Booking, Admin Dashboard, Settings
- Stored in browser localStorage
- Changes apply immediately
- Can be removed/changed anytime

## 📁 Files Included

```
src/
├── index.html              # Landing page
├── client-booking.html     # Client booking interface
├── admin-dashboard.html    # Admin panel
└── settings.html          # Settings & customization
```

## 🚀 Quick Start

1. **Download all files** from the `src/` folder
2. **Put them in one folder** on your device
3. **Open `index.html`** in Safari or Chrome
4. **Click "Admin Dashboard"** → **"⚙️ Settings"**
5. **Upload a background image**
6. **Click "💾 Save All Settings"**
7. **Navigate through pages** - see your image everywhere!

## 📸 Testing the Background Feature

### Upload an Image:
1. Go to Settings page
2. Click the upload area
3. Choose an image (under 5MB)
4. Preview appears
5. Click "Save All Settings"

### Verify It Works:
1. Go to Dashboard - ✓ See image
2. Go to Index - ✓ See image  
3. Go to Booking - ✓ See image
4. Refresh page - ✓ Still there

## 🎨 Recommended Images

**What works best:**
- Spa/wellness photos (stones, candles, plants)
- Soft nature scenes (beaches, forests)
- Abstract textures (watercolor, marble)
- Calm colors (greens, blues, earth tones)

**Image specs:**
- Size: 1920x1080px recommended
- Max: 5MB
- Format: JPG, PNG, WEBP

## 🔧 How It Works

### Technical Overview:
1. Settings page saves image as base64 in localStorage
2. Each page loads settings on page load
3. Background image applied via CSS
4. Semi-transparent overlay ensures readability
5. All pages share the same localStorage key

### Storage:
- Key: `tejaseSettings`
- Contains: backgroundImage, services, hours, contact
- Persists until browser cache cleared

## 📱 Device Compatibility

Tested on:
- ✅ iPad Safari
- ✅ iPhone Safari  
- ✅ Chrome (Desktop/Mobile)
- ✅ Firefox
- ✅ Edge

## 🐛 Known Limitations

- Background image stored in browser (doesn't sync across devices)
- 5MB file size limit (browser localStorage limit)
- Very dark images may reduce text readability
- Incognito/Private mode won't persist settings

## 💡 Tips

**For Best Results:**
- Use high-quality images
- Choose images with good contrast
- Lighter images work better
- Test on your target devices
- Keep file sizes reasonable (<3MB ideal)

**If Issues Occur:**
- Check browser console (F12)
- Verify file is under 5MB
- Try different image format
- Clear localStorage and retry

## 📖 Documentation

See `TESTING_GUIDE.md` for:
- Detailed testing instructions
- Step-by-step walkthrough
- Troubleshooting guide
- Success criteria

## 🔄 Next Steps

After testing this prototype:
1. Verify background feature works as expected
2. Test on all target devices
3. Make any final adjustments
4. Deploy to production/GitHub
5. Train Danielle on using Settings

## ⚙️ Settings Features

Beyond backgrounds, Settings also manages:
- **Services**: Add/edit/delete offerings
- **Business Hours**: Set availability schedule
- **Contact Info**: Business details
- **Booking Instructions**: Special client notes

All stored in the same localStorage system.

## 🎓 Learning Notes

This prototype demonstrates:
- LocalStorage for data persistence
- Base64 image encoding
- CSS background properties
- Responsive design patterns
- Multi-page state management

## 🆘 Support

If you encounter issues:
1. Check `TESTING_GUIDE.md`
2. Review browser console
3. Try a different image/browser
4. Clear localStorage and start fresh

## ✅ Ready to Use

This prototype is **production-ready** for testing. All core features work:
- ✓ Background images integrated
- ✓ Booking system functional
- ✓ Admin tools working
- ✓ Settings page complete
- ✓ Responsive on all devices

---

**Start testing:** Open `src/index.html` and follow the Quick Start guide above!
