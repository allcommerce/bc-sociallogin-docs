# OTP Email Login

Allow customers to login to your BigCommerce store using passwordless email verification codes.

## Overview

OTP (One-Time Password) Email Login provides a secure, passwordless way for customers to access your store. Customers simply enter their email address and receive a temporary login code.

![OTP Login Demo](../assets/images/otp-login-demo.gif)

## Benefits

### For Customers
- **Passwordless**: No need to remember or create passwords
- **Secure**: Temporary codes that expire quickly
- **Simple**: Just need an email address
- **Accessible**: Works for customers without social accounts

### For Your Store
- **Higher conversion**: Remove password barriers
- **Broader accessibility**: Reach customers who don't use social media
- **Reduced support**: No password reset requests
- **Enhanced security**: No stored passwords to compromise

## How It Works

1. **Customer enters email** on login page
2. **System sends 6-digit code** to their email instantly
3. **Customer enters code** to complete login
4. **Code expires after 10 minutes** for security
5. **Account created automatically** if email doesn't exist

## Setup

### Enable OTP Email Login

1. Go to Papa Social Login dashboard
2. Find **"OTP Email Login"** in the Social Providers section
3. Toggle the switch to **ON**
4. Configure your SMTP server settings (required)
5. Click **"Save Changes"**

![Enable OTP Login](../assets/images/enable-otp-login.png)

### SMTP Configuration Required

You must configure your own SMTP server to send OTP emails:

```json
{
  "host": "smtp.gmail.com",
  "port": 587,
  "secure": false,
  "auth": {
    "user": "your-email@gmail.com",
    "pass": "your-app-password"
  },
  "from": {
    "name": "Your Store Name",
    "email": "your-email@gmail.com"
  }
}
```

### Popular SMTP Providers

**Gmail SMTP:**
- Host: smtp.gmail.com
- Port: 587
- Requires App Password (not your regular Gmail password)

**SendGrid SMTP:**
- Host: smtp.sendgrid.net
- Port: 587
- Use API key as password

**Other providers:** Most email providers offer SMTP services. Check your provider's documentation for settings.

## Testing

### Test the OTP Flow

1. Open your website in an incognito/private browser window
2. Go to your login page (yourstore.com/login.php)
3. You should see the "Sign in with Email" button
4. Enter an email address
5. Check email for the 6-digit code
6. Enter the code to complete login

![OTP Login Test](../assets/images/otp-login-test.png)

## Common Issues

### OTP Emails Not Sending
- Verify SMTP configuration is correct
- Check your email provider's SMTP settings
- Test SMTP connection using the built-in test feature
- Check spam/junk folders

### Invalid Code Errors
- Codes expire after 10 minutes
- Each code can only be used once
- Check for typos in the entered code
- Request a new code if needed

### Email Delivery Issues
- Configure proper SPF records for your domain
- Ensure your sending domain has good reputation
- Consider using a dedicated email service like SendGrid

## Email Template

The OTP email template includes:
- 6-digit verification code
- Expiration time (10 minutes)
- Store name and branding
- Security reminder

Example email content:
```
Your login code for [Store Name]: 123456

This code will expire in 10 minutes.
If you didn't request this code, please ignore this email.
```

## Support

Need help with OTP Email Login setup?

- **Email**: support@papathemes.com
- **Live Chat**: Available in dashboard
- **Documentation**: [SMTP configuration guide](../configuration.md)

!!! warning "SMTP Required"
    OTP Email Login requires your own SMTP server configuration. Papa Social Login does not provide email sending services.