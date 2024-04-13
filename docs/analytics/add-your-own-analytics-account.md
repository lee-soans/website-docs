---
sidebar_position: 1
---

# Add your own Google Analytics account

Website Pro has a built-in dashboard that displays highlights of your site’s visitor information using [Google Analytics.](https://www.google.com/analytics/analytics/) However, we understand that you may want to dig deeper using your own account. That’s why Website Pro provides an easy way to do just that.

_Note: Plugins meant to support Google Analytics are available, but these often fail to track gather data in the Website Pro environment._ 

1.  [Sign up](https://analytics.google.com/analytics/web/) for Google Analytics and configure it for your site, or just log in if you’ve already completed that step.
2.  Click [Admin](https://support.google.com/analytics/answer/6132368)
3.  Select your site’s account from the menu in the _ACCOUNT_ column
4.  Select a property from the menu in the _PROPERTY_ column
5.  Under _PROPERTY_, click **Tracking Info > Tracking Code**. Your [tracking ID](https://support.google.com/analytics/answer/7372977) is displayed at the top of the page
6.  Copy that Tracking ID
7.  Sign into to your Website Pro site’s WordPress admin panel
8.  Navigate to **Settings > General Code** and scroll to the bottom
9.  Paste that Tracking ID into the **Custom Google Analytics Tracking ID** and click **Save Changes**

Please keep in mind that this ID will run concurrently with Website Pro’s built-in analytic tracking, which will remain on the Website Pro dashboard.

![Under "Settings > General" you can enter a Google Analytics Tracking ID connected to your own Google Analytics Account.](/img/smaller_GA_tracking_id.png)