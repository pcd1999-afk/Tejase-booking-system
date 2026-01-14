# 🧪 Complete Prototype Testing Guide

## What This Prototype Does

This is a **fully integrated version** where:
✅ All 4 pages load custom background images from Settings
✅ Background shows on: Index, Client Booking, Admin Dashboard, Settings
✅ Images are stored in browser localStorage
✅ Changes apply immediately across all pages

## File Structure

```
tejase-prototype-complete/
└── src/
    ├── index.html              (Landing page with background)
    ├── client-booking.html     (Booking page with background)
    ├── admin-dashboard.html    (Admin panel with background)
    └── settings.html           (Settings page with background)
```

## Step-by-Step Testing Instructions

### Step 1: Open the Prototype
1. Download all files from the `tejase-prototype-complete/src/` folder
2. Put them in a folder on your iPad/computer
3. Open `index.html` in Safari

**What you should see:**
- Landing page with earth-tone gradient background
- Two buttons: "Book an Appointment" and "Admin Dashboard"

### Step 2: Test Admin Dashboard
1. Click "Admin Dashboard" button
2. You'll see the admin dashboard with stats and calendar

**What you should see:**
- Same earth-tone background as landing page
- Dashboard with bookings and calendar
- ⚙️ Settings button in top-right

### Step 3: Access Settings
1. Click the **⚙️ Settings** button (top-right)
2. Settings page opens

**What you should see:**
- Settings page with four sections
- Background Image uploader at top
- Services, Business Hours, Contact Info below

### Step 4: Upload a Background Image

**Option A: From Computer**
1. Click the upload area (with 🖼️ icon)
2. Select an image from your device
3. Wait for preview to appear
4. Click **💾 Save All Settings** at bottom

**Option B: Drag & Drop**
1. Find an image file on your computer
2. Drag it onto the upload area
3. Drop it
4. Wait for preview
5. Click **💾 Save All Settings**

**Recommended Test Images:**
- Spa photo (stones, candles, plants)
- Nature scene (forest, beach, mountains)
- Abstract texture (watercolor, marble)
- Size: 1920x1080 or similar
- Keep under 5MB

### Step 5: Verify Background Loads

**After saving, test each page:**

1. **Go to Admin Dashboard**
   - Click "← Back to Dashboard"
   - Your uploaded image should be the background
   - Semi-transparent overlay keeps content readable

2. **Go to Index/Landing Page**
   - Navigate back or close and reopen `index.html`
   - Your image appears as background
   - Buttons and text still readable

3. **Go to Client Booking**
   - Click "Book an Appointment"
   - Your image shows as background
   - Booking form still easy to read

4. **Go back to Settings**
   - Navigate to Settings again
   - Your image is also the background there
   - You can see your uploaded image in the preview

### Step 6: Test Removing Background

1. In Settings, click **"Remove Background Image"**
2. Confirm removal
3. Click **💾 Save All Settings**
4. Navigate to other pages
5. Default gradient should be back

### Step 7: Test Multiple Images

1. Upload a new image (overwrites previous)
2. Save settings
3. Navigate through pages
4. New image should show everywhere

## What To Look For

### ✅ Success Indicators

**Background Image:**
- [ ] Image appears on all 4 pages
- [ ] Image doesn't distort (proper scaling)
- [ ] Text remains readable over image
- [ ] Semi-transparent overlay helps visibility
- [ ] Image persists after refresh
- [ ] Image loads quickly

**Settings Page:**
- [ ] Upload area accepts images
- [ ] Preview shows before saving
- [ ] "Save All Settings" shows success message
- [ ] Can remove and restore default
- [ ] Drag & drop works

**Overall Experience:**
- [ ] Navigation between pages works
- [ ] Background doesn't slow down pages
- [ ] Forms still function correctly
- [ ] Booking process still works
- [ ] Admin features still work

### ⚠️ Potential Issues

**If image doesn't show:**
- Check browser console (F12) for errors
- Verify file size is under 5MB
- Try a different image format (JPG vs PNG)
- Make sure you clicked "Save All Settings"
- Try refreshing the page (Ctrl/Cmd + R)

**If image is too dark/light:**
- The semi-transparent overlay can be adjusted
- Choose images with good contrast
- Lighter images work better

**If text is hard to read:**
- Try a different image
- Choose images with less busy patterns
- The overlay automatically adds readability

## Advanced Testing

### Test on Different Devices
- [ ] iPad Safari
- [ ] iPhone Safari
- [ ] Desktop Chrome
- [ ] Desktop Firefox

### Test Different Image Types
- [ ] Large image (3MB+)
- [ ] Small image (<500KB)
- [ ] PNG with transparency
- [ ] JPG photo
- [ ] Wide landscape image
- [ ] Tall portrait image

### Test Edge Cases
- [ ] Upload, then immediately navigate away
- [ ] Upload multiple times in a row
- [ ] Remove, then immediately re-upload
- [ ] Close browser completely, reopen

## Console Debugging

Open browser console (F12) to see debug messages:

**Expected messages:**
```
✓ Custom background loaded on booking page
✓ Custom background loaded on admin dashboard
✓ Custom background loaded on settings page
```

**If you see errors:**
- Note the error message
- It will help diagnose the issue

## Sample Test Images

For testing, try searching for:
- "spa background images"
- "healing arts background"
- "nature meditation background"
- "subtle texture background"

**Good test image characteristics:**
- Calm, soothing colors
- Not too busy/detailed
- Good contrast areas for text
- Professional quality
- Relevant to healing/wellness

## Testing Checklist

Complete this checklist:

- [ ] Downloaded all 4 HTML files
- [ ] Opened index.html in browser
- [ ] Navigated to Admin Dashboard
- [ ] Clicked Settings button
- [ ] Uploaded a background image
- [ ] Clicked "Save All Settings"
- [ ] Saw success message
- [ ] Went back to Dashboard - saw image
- [ ] Went to Index - saw image
- [ ] Went to Client Booking - saw image
- [ ] Went to Settings - saw image
- [ ] Removed background image
- [ ] Saw default gradient return
- [ ] Uploaded different image
- [ ] Confirmed new image everywhere
- [ ] Closed browser and reopened
- [ ] Background still there

## Troubleshooting Guide

### Problem: Image won't upload
**Solutions:**
1. Check file size (must be under 5MB)
2. Try a different image format
3. Make sure browser allows localStorage
4. Check if file is actually an image

### Problem: Image shows in preview but not on pages
**Solutions:**
1. Did you click "Save All Settings"?
2. Try refreshing the pages (Ctrl/Cmd + R)
3. Check browser console for errors
4. Clear localStorage and try again

### Problem: Image is gone after closing browser
**Solutions:**
1. Browser may have cleared localStorage
2. Check browser privacy settings
3. Make sure not in Incognito/Private mode
4. Try different browser

### Problem: Image makes text unreadable
**Solutions:**
1. This is expected with some images
2. Try a lighter, less busy image
3. The overlay helps but isn't perfect
4. Choose images with natural spaces for text

### Problem: Page loads slowly
**Solutions:**
1. Image is too large (over 5MB)
2. Try compressing the image first
3. Use JPEG instead of PNG
4. Choose smaller resolution image

## Success Criteria

The prototype is working correctly if:
✅ You can upload an image in Settings
✅ The image appears on all 4 pages
✅ Text remains readable
✅ Image persists after browser refresh
✅ You can change or remove the image
✅ All other features still work (booking, calendar, etc.)

## Next Steps After Testing

Once testing is complete:
1. ✅ Note any issues or improvements
2. ✅ Decide if ready for production
3. ✅ Prepare for GitHub deployment
4. ✅ Create backup of working version

---

**Ready to test?** Open `index.html` and follow the steps above!

## Quick Test Script

**5-Minute Quick Test:**
1. Open index.html
2. Click Admin Dashboard
3. Click Settings
4. Upload any image
5. Save
6. Click Back to Dashboard
7. See your image as background ✓
8. Navigate to other pages
9. Confirm image everywhere ✓
10. Success!
