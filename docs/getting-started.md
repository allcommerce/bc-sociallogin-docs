# Quick Start Guide

Welcome to Papa Social Login! This guide will help you set up and use the application within **10 minutes**.

## Prerequisites

!!! info "System Requirements"
    - Active BigCommerce store
    - Store admin access
    - Email address for account registration

## Step 1: Install from BigCommerce App Store

### 1.1 Find the Application

1. Log in to your **BigCommerce Admin Panel**
2. Select **Apps** > **App Marketplace**
3. Search for **"Papa Social Login"**
4. Click on the application in search results

![Search Papa Social Login](assets/images/app-store-search.png)

### 1.2 Install the Application

1. Click **"Install"** or **"Get This App"** button
2. Review the permissions the app requires:
   - Read customer information
   - Create and update customers
   - Read store configuration
3. Click **"Confirm"** to complete installation

!!! warning "Important"
    Make sure you read the permissions carefully before installing. Papa Social Login only requests necessary permissions to function properly.

### 1.3 Access the Application

After successful installation:

1. You'll see **Papa Social Login** in **Apps** > **My Apps**
2. Click on the app name to open the dashboard
3. The system will automatically create an account for you

## Step 2: Basic Configuration

### 2.1 Enable Login Methods

After opening the dashboard, you'll see an interface like this:

![Papa Social Login Dashboard](assets/images/dashboard.png)

**Enable Google Login:**

1. Toggle the **"Google Login"** switch to ON
2. The app will automatically use default Google configuration
3. Wait a few seconds for the system to update

**Enable Facebook Login:**

1. Toggle the **"Facebook Login"** switch to ON
2. Similarly, the system will use default configuration
3. Wait for the update to complete

!!! tip "7-Day Free Trial"
    Start your 7-day free trial to access all features including Google and Facebook login with custom configuration, Email OTP, and more. No credit card required to start!

### 2.2 Install Script for Website

In the dashboard, click **"Install the script to this site"** button.

!!! tip "Multi-store channels"
    If you want to install on a different store channel, select the channel from the dropdown menu next to the button.

A new script "Papa Social Login by PapaThemes" will be automatically installed to the Script Manager of the current Store Channel.

![Install Script](assets/images/install-script.png)

### 2.3 Test Functionality

1. Open your website in a new tab
2. Go to the login page (**yourstore.com/login.php**)
3. You should see new login buttons:

![Social Login Buttons](assets/images/login-buttons.png)

4. Try logging in with Google or Facebook

!!! success "Complete!"
    If you can successfully log in, you've successfully set up Papa Social Login!

## Step 3: Monitor Activity

### 3.1 View Statistics

Return to Papa Social Login dashboard:

1. The **"Statistics"** section displays:
   - Total logins today
   - Most used method
   - 7-day chart

![Statistics Dashboard](assets/images/statistics.png)

### 3.2 Check New Customers

1. In BigCommerce Admin, go to **Customers** > **View All**
2. Customers who logged in via social media will have:
   - Avatar from social account
   - Complete information (name, email)
   - Note "Created via Papa Social Login"

## Advanced Configuration (Optional)

### Enable Email OTP (Advanced Feature)

If you want to allow customers to login with email OTP:

1. Start your 7-day free trial or subscribe
2. In dashboard, enable **"OTP Email Login"**
3. Configure your SMTP server settings

### Customize Interface

1. Go to **Settings** > **Appearance**
2. Customize:
   - Login button colors
   - Size and position
   - Display text

![Appearance Settings](assets/images/appearance-settings.png)

### Custom OAuth Configuration

To use your own Google/Facebook apps:

1. Read [OAuth Configuration Guide](configuration.md)
2. Create apps on Google/Facebook Developer Console
3. Enter Client ID and Client Secret into Papa Social Login

## Common Troubleshooting

### Don't See Login Buttons

- **Check**: Is the script installed?
- **Solution**: Try reinstalling the script or check cache

### Error When Logging in with Google/Facebook

- **Check**: Is the store using HTTPS?
- **Solution**: BigCommerce requires HTTPS for OAuth

### Duplicate Customer Creation

- **Check**: Does the customer's email already exist in the system?
- **Solution**: Papa Social Login will automatically link to existing accounts

!!! question "Need Help?"
    If you encounter difficulties, please see:
    
    - [Troubleshooting Guide](troubleshooting.md)
    - [FAQ](faq.md)
    - Or contact support@papathemes.com

## Next Steps

Now that you've successfully set up Papa Social Login! Here are some suggestions:

<div class="grid cards" markdown>

-   :material-cog: **Advanced Customization**

    ---

    Configure features in detail

    [:octicons-arrow-right-24: View guide](configuration.md)

-   :material-chart-line: **Monitor Performance**

    ---

    Analyze impact on conversion rates

    [:octicons-arrow-right-24: View dashboard](management/dashboard.md)

-   :material-palette: **Customize Interface**

    ---

    Make login buttons match your theme

    [:octicons-arrow-right-24: Customize](advanced/customization.md)

-   :material-security: **Enhance Security**

    ---

    Learn about security features

    [:octicons-arrow-right-24: Security](advanced/security.md)

</div>

---

!!! success "Congratulations!"
    You have completed setting up Papa Social Login. Your customers can now log in more easily, and conversion rates will improve significantly!