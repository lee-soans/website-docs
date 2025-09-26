---
title: "How to Generate Application Passwords on WordPress Hosting"
sidebar_label: "Generate Application Passwords"
description: "This article guides you through generating application-specific passwords in WordPress Hosting. A custom plugin is required for enabling this feature."
---

Application passwords allow you to grant access to your WordPress site without sharing your primary login credentials. They are particularly useful for integrating third-party services and applications while maintaining account security.  

On our WordPress Hosting environment, this feature requires a **custom plugin** to be enabled. We’ve provided a sample plugin stub below that you can download and install.  

![](./img/application-password-example.png)

---

### Why Application Passwords Are Useful  

- **Secure Integrations** – Safely connect third-party apps without sharing your main password.  
- **Easy Revocation** – Revoke access for a specific application without affecting your main login.  
- **Improved Security** – Reduce exposure of your primary account credentials.  

---

### Steps to Enable and Generate an Application Password  

1. **Download and Install the Plugin**  
   - Use the provided stub plugin from our GitHub repository.  
   - [![Download Plugin](https://img.shields.io/badge/Download-Plugin-blue?style=for-the-badge)](https://github.com/example-org/wp-app-password-plugin-stub/archive/refs/heads/main.zip)  

2. **Activate the Plugin in WordPress**  
   - Log into your WordPress Admin Dashboard.  
   - Navigate to **Plugins → Add New → Upload Plugin**.  
   - Upload the ZIP file and activate it.  

3. **Access the Application Password Settings**  
   - Go to **Users → Profile**.  
   - Scroll to the **Application Passwords** section (enabled by the custom plugin).  
   - Enter a name for the application (e.g., “Mail Client” or “CRM Integration”).  

4. **Generate and Save the Password**  
   - Click **Add New Application Password**.  
   - A new password will be generated — copy and save it securely.  
   - Use this password in your third-party application instead of your main WordPress login.  

---

### Security Considerations  

- Treat application passwords like normal passwords — store them securely.  
- Revoke unused or compromised passwords immediately.  
- Combine with [Two-Step Authentication](https://wordpress.com/support/security/two-step-authentication/application-specific-passwords/) for stronger protection.  

---

### Troubleshooting  

- If the **Application Passwords** section does not appear, ensure the custom plugin is installed and active.  
- Conflicts with poorly coded plugins or themes may interfere — test with only the stub plugin active.  
- Check PHP error logs for signs of misconfiguration.  

![](./img/application-password-troubleshoot.png)

---
