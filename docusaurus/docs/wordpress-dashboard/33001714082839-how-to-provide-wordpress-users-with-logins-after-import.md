---
title: "How to Provide WordPress Users with Logins After Import"
sidebar_label: "How to Provide WordPress Users with Logins After Import"
description: "When an existing WordPress site is imported into WordPress Hosting, the users from the original site won’t automatically retain their login access. To restore"
zendesk_id: 33001714082839
zendesk_url: "https://support.vendasta.com/hc/en-us/articles/33001714082839-How-to-Provide-WordPress-Users-with-Logins-After-Import"
updated_at: "2025-06-23T20:17:28Z"
labels: ["login", "WordPress"]
section_id: 27570091751191
locale: "en-us"
---

When an existing WordPress site is imported into WordPress Hosting, the users from the original site won’t automatically retain their login access. To restore their ability to log in, you have two options:

### Option 1: Create New Users

1.  Delete all existing WordPress users.
2.  For each person who needs access, create a **Business App** user.
3.  When these users access the WordPress Dashboard for the first time, a WordPress user with Administrator access will be created automatically using their email.

### Option 2: Sync Existing Users

1.  Create a **Business App** user for each existing WordPress user.
2.  Ensure that the email used for the Business App user matches the existing WordPress user’s email exactly.

**Important:**  
The email addresses must be identical. For example:

*   If Bob’s WordPress email is **robert@email.com**, the corresponding Business App user must also use **robert@email.com**.
*   Using a different email (e.g., **bob@email.com**) will create a new WordPress user, resulting in Bob having two separate accounts.

By following these steps, you can ensure that WordPress users regain access seamlessly while maintaining proper account management.
