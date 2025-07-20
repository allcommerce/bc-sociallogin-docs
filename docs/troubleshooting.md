# Troubleshooting

Common solutions for Papa Social Login issues.

## Login Buttons Not Appearing

### Check Script Installation
1. Verify the script is installed in your BigCommerce Script Manager
2. Clear your browser cache and try again
3. Test in an incognito/private browser window

### Check Provider Settings
1. Go to Papa Social Login dashboard
2. Verify the login providers are enabled (toggled ON)
3. Click "Save Changes" after making any updates

## Social Login Not Working

### HTTPS Required
- Ensure your store uses HTTPS (required for OAuth)
- Check that your store URL starts with `https://`

### Popup Blocked
- Allow popups for your store domain
- Try logging in with a different browser
- Disable browser extensions that might block popups

### Clear Browser Data
1. Clear cookies and browser cache
2. Try logging in again
3. Test with incognito/private browsing

## OTP Email Issues

### OTP Emails Not Sending
1. **Check SMTP Configuration:**
   - Verify your SMTP server settings are correct
   - Test your email provider's SMTP connection
   - Check spam/junk folders

2. **Email Provider Issues:**
   - Gmail: Use App Password (not regular password)
   - SendGrid: Verify API key is correct
   - Other providers: Check SMTP settings documentation

### Invalid OTP Code
- Codes expire after 10 minutes
- Each code can only be used once
- Check for typos when entering the code
- Request a new code if needed

## Customer Account Issues

### Duplicate Accounts
- Papa Social Login automatically links social accounts to existing BigCommerce customers with matching emails
- If issues persist, contact support for manual account linking

### Missing Customer Information
- Some social providers have privacy restrictions
- Only basic information (name, email, profile picture) is typically available

## General Issues

### Login Buttons Look Wrong
1. Check if your theme has conflicting CSS
2. Clear browser cache
3. Try a different browser

### Login Process Slow
1. Check your internet connection
2. Verify your store's performance
3. Test during different times of day

### JavaScript Errors
1. Open browser Developer Tools (F12)
2. Check Console tab for errors
3. If you see Papa Social Login related errors, contact support

## Getting Help

### Before Contacting Support
1. Try the solutions above
2. Test with different browsers
3. Check if the issue occurs on mobile devices
4. Note any error messages you see

### Contact Information
- **Email**: support@papathemes.com
- **Live Chat**: Available in Papa Social Login dashboard
- **Response Time**: Within 24 hours

### Information to Include
When contacting support, please provide:
- Your store URL
- Which login method has issues (Google, Facebook, etc.)
- Browser and device you're using
- Any error messages
- Screenshots if helpful

!!! tip "Quick Test"
    Try logging in with an incognito/private browser window first - this solves many common issues by bypassing cache and cookies.