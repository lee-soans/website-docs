---
sidebar_position: 1
---

# Domain Setup
To set up your domain for WordPress Hosting, there are two records you’ll need to change.  
  
**A record:** Allows you to point your root domain to your website

**CNAME record**: Allows pointing a subdomain to your website, such as www.

To set up your A record, log in to your domain registrar and access your domain settings. From there, choose to add an A record. For this new record, add the following information:  
  
**HOST**: This should be either blank or @ (depending on your provider) <br/>
**Points to**: 34.149.86.124 <br/>
**TTL**: 3600 seconds (1 hour)

To set up your CNAME record, log in to your domain registrar and access your domain settings. From there, choose to add a CNAME record and enter the following information:  
  
**HOST**: This should be the subdomain you want to use (usually www) <br/>
**Points to**: host.wordpresshosting.com <br/>
**TTL**: 3600 seconds (1 hour)  

Once the above records are set up, you will need to validate them in WordPress Hosting. Open WordPress Hosting for the applicable account, navigate to the **Domains** tab, and select “Connect Domain.” In the dialog, add the root domain you want to connect. If applicable, check the box to add the www. address.

From here, WordPress Hosting will regularly check to ensure those records are in place. Until it finds the records you created, your added domains will be marked as Pending. You can check to see if your domains are propagating by looking them up on MxToolbox:  
  
**A record**: Enter your root domain: [https://mxtoolbox.com/DNSLookup.aspx](https://mxtoolbox.com/DNSLookup.aspx) <br/>The A record that is returned should include an IP address of 34.149.86.124  
  
**CNAME record**: Enter your subdomain (e.g. www.business.com): [https://mxtoolbox.com/DNSLookup.aspx](https://mxtoolbox.com/DNSLookup.aspx) <br/>The record that is returned should reflect a Canonical Name of host.wordpresshosting.com

:::tip[FAQs]
**What is the base requirement:** To link your domain to WordPress Hosting you must use at least one A record or CNAME record. We recommend that you hook up both the A record and the CNAME record when setting up your new domain.

**Do I need to do anything to setup SSL**: All WordPress Hosting sites are automatically provisioned a Let’s Encrypt SSL certificate, so you would not need to follow any extra steps to set this up

**How do I set the preferred URL:** This can be done from the domains tab of WordPress Hosting. Select the kabob menu next to the domain you want to use, then select Make Primary. This will make it so that when the site is accessed from any of it’s connected domains, the user is redirected to your primary one.
:::