# Facebook Login

Allow customers to login to your BigCommerce store using their Facebook accounts.

## Overview

Facebook Login provides a familiar and convenient way for customers to access your store using their existing Facebook credentials. This reduces friction and improves the shopping experience.

![Facebook Login Demo](../assets/images/facebook-login-demo.gif)

## Benefits

### For Customers
- **Familiar**: Use existing Facebook account
- **Quick**: Login with just a few clicks  
- **No passwords**: No need to remember store passwords
- **Profile sync**: Name and email automatically filled

### For Your Store
- **Increased signups**: Lower barriers to account creation
- **Reduced abandonment**: Faster checkout process
- **Better engagement**: Social connection can increase loyalty
- **Accurate data**: Real customer information from Facebook

## Setup

### Enable Facebook Login

1. Go to Papa Social Login dashboard
2. Find **"Facebook Login"** in the Social Providers section
3. Toggle the switch to **ON**
4. Click **"Save Changes"**

![Enable Facebook Login](../assets/images/enable-facebook-login.png)

Facebook Login is ready to use immediately - no additional configuration needed!

## Testing

### Test the Login Flow

1. Open your website in an incognito/private browser window
2. Go to your login page (yourstore.com/login.php)
3. You should see the "Sign in with Facebook" button
4. Click the button and login with a Facebook account
5. Verify you're redirected back and logged into your store

![Facebook Login Test](../assets/images/facebook-login-test.png)

## Common Issues

### Login Button Not Visible
- Check that Facebook Login is enabled in the dashboard
- Verify the script is properly installed
- Clear your browser cache

### Login Not Working
- Ensure your store uses HTTPS (required for OAuth)
- Check that popups are not blocked in your browser
- Try logging out of Facebook and back in

### Customer Account Issues
- New customers are automatically created in BigCommerce
- Existing customers with the same email are automatically linked
- Customer information is synced from their Facebook profile

### Facebook App Restrictions
- Facebook has privacy restrictions that may limit some data access
- Only basic profile information (name, email) is accessed
- Customer controls what information is shared

## Support

Need help with Facebook Login setup?

- **Email**: support@papathemes.com
- **Live Chat**: Available in dashboard
- **Documentation**: [Complete setup guide](../getting-started.md)

!!! tip "Privacy Note"
    Papa Social Login only accesses basic profile information (name, email, profile picture) and does not access posts, friends, or other private data.