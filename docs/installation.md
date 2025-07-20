# Detailed Installation Guide

This document provides detailed installation instructions for Papa Social Login for special cases and manual installation.

## Installation from BigCommerce App Store

### Step 1: Access App Marketplace

1. Log in to **BigCommerce Control Panel**
2. In the left menu, select **Apps** → **App Marketplace**
3. Use the search bar, type **"Papa Social Login"**

![BigCommerce App Store](assets/images/bc-app-store.png)

### Step 2: Review Application Information

Before installing, review:

- **User reviews**: Check ratings and reviews
- **Developer information**: PapaThemes
- **Required permissions**:
  - Read customer information
  - Write customer information
  - Read store information
  - Read script tags

### Step 3: Install Application

1. Click **"Get This App"** or **"Install"**
2. Carefully read the list of permissions the application requires
3. Click **"Confirm"** to agree to installation
4. Wait a few seconds for the installation to complete

!!! warning "Important Note"
    Papa Social Login needs these permissions to:

    - **Read customer**: Check if customer already exists
    - **Write customer**: Create new account from social login
    - **Read store**: Get store configuration information
    - **Read script**: Manage script injection

## Script Installation

After installing the application, you need to install the script to display login buttons on your website.

### Automatic Installation

1. Open Papa Social Login dashboard
2. Click **"Install the script to this site"** button

!!! tip "Multi-store channels"
    If you want to install on a different store channel, select the channel from the dropdown menu next to the button.

A new script "Papa Social Login by PapaThemes" will be automatically installed to the Script Manager of the current Store Channel.

![Install Script](assets/images/install-script.png)

## Custom Theme Configuration

### Popular Themes

Papa Social Login has been tested with the following themes:

| Theme | Compatibility | Notes |
|-------|---------------|-------|
| Cornerstone | ✅ | Works perfectly |
| Stencil | ✅ | Requires minor CSS adjustments |
| Custom themes | ❓ | Depends on structure |

## Installation Verification

### Check Frontend

1. Open website in incognito browser
2. Go to login page
3. Check if social login buttons are visible

![Login Buttons on Frontend](assets/images/frontend-login.png)

### Check Console

Open Developer Tools (F12) and check:

1. **Console tab**: No JavaScript errors
2. **Network tab**: Script loads successfully
3. **Elements tab**: Login buttons are in DOM

### Test Login

1. Try logging in with Google
2. Try logging in with Facebook
3. Check if account is created in BigCommerce Admin

## Installation Troubleshooting

### Login Buttons Not Visible

**Possible causes:**

- Script not loaded
- Theme conflict
- Incorrect store hash configuration

**Solutions:**

1. Check browser console for errors
2. Verify script is added to Script Manager
3. Clear browser and BigCommerce cache

### Login Buttons Not Working

**Possible causes:**

- Store not using HTTPS
- Popup blocked
- Incorrect OAuth configuration

**Solutions:**

1. Ensure store uses SSL
2. Add domain to popup whitelist
3. Check configuration in dashboard

### Customer Not Created

**Possible causes:**

- Missing API permissions
- Email already exists
- Database connection error

**Solutions:**

1. Check application permissions
2. View logs in dashboard
3. Contact support if needed

## Multi-Store Installation

If you have multiple BigCommerce stores:

1. **Separate installation**: Each store needs separate script installation
2. **Separate configuration**: Each store has its own OAuth configuration
