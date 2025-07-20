# X/Twitter Login

Allow customers to login to your BigCommerce store using their X (Twitter) accounts.

## Overview

X/Twitter Login provides an additional social login option for customers who prefer to use their X credentials. This can be especially useful for stores targeting social media-savvy audiences.

![X Login Demo](../assets/images/twitter-login-demo.gif)

## Benefits

### For Customers
- **Alternative option**: Use existing X account
- **Quick access**: Fast login process
- **No new passwords**: Use familiar X credentials
- **Profile integration**: Basic profile information synced

### For Your Store
- **More login options**: Cater to different user preferences
- **Broader reach**: Access X user base
- **Social engagement**: Connect with socially active customers
- **Reduced friction**: Alternative to traditional registration

## Setup

### Enable X/Twitter Login

1. Go to Papa Social Login dashboard
2. Find **"X/Twitter Login"** in the Social Providers section
3. Toggle the switch to **ON**
4. Configure your X OAuth credentials if needed
5. Click **"Save Changes"**

![Enable Twitter Login](../assets/images/enable-twitter-login.png)

Note: X/Twitter login may require additional OAuth setup depending on your configuration.

## Testing

### Test the Login Flow

1. Open your website in an incognito/private browser window
2. Go to your login page (yourstore.com/login.php)
3. You should see the "Sign in with X" button
4. Click the button and login with an X account
5. Verify you're redirected back and logged into your store

![X Login Test](../assets/images/twitter-login-test.png)

## Common Issues

### Login Button Not Visible
- Check that X/Twitter Login is enabled in the dashboard
- Verify the script is properly installed
- Clear your browser cache

### Login Not Working
- Ensure your store uses HTTPS (required for OAuth)
- Check that popups are not blocked in your browser
- Verify X OAuth configuration if using custom settings

### Customer Account Issues
- New customers are automatically created in BigCommerce
- Existing customers with the same email are automatically linked
- Customer information is synced from their X profile

### X API Limitations
- X has strict API usage policies
- Only basic profile information is accessible
- Some features may require additional X Developer approval

## Support

Need help with X/Twitter Login setup?

- **Email**: support@papathemes.com
- **Live Chat**: Available in dashboard
- **Documentation**: [Complete setup guide](../getting-started.md)

!!! info "X Developer Requirements"
    X/Twitter login may require custom OAuth setup and X Developer account approval for some configurations. Contact support for assistance with X Developer account setup.