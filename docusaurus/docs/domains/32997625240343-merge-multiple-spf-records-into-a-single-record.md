---
title: "Merge multiple SPF records into a single record"
sidebar_label: "Merge multiple SPF records into a single record"
description: "To merge the SPF values, simply include all the parts into one single record, without repeating any mechanisms. Here's how to merge the following example SPF"
zendesk_id: 32997625240343
zendesk_url: "https://support.vendasta.com/hc/en-us/articles/32997625240343-Merge-multiple-SPF-records-into-a-single-record"
updated_at: "2025-06-23T18:18:31Z"
labels: ["SPF"]
section_id: 27570129178007
locale: "en-us"
---

To merge the SPF values, simply include all the parts into one single record, without repeating any mechanisms. Here's how to merge the following example SPF records for Outlook and MailerLite:

**v=spf1 a include:spf.protection.outlook.com -all**

**v=spf1 a mx include:\_spf.mlsend.com ~all**

**1\. The SPF record always begins with the version prefix:**

**v=spf1**

**2\. Both records contain an "a" mechanism and the MailerLite SPF record contains a "mx" mechanism, so include both in the new record:**

**v=spf1 a mx**

**3\. Then add both "include" mechanisms into the record, resulting in:**

**v=spf1 a mx include:spf.protection.outlook.com include:\_spf.mlsend.com**

4\. Lastly, we need to define how emails should be treated if they don't comply with the set rules. We do this by using the **all** mechanism. The last part has to be either **?all**, **\-all** or **~all**. It’s not possible to have more than one, so it is ultimately your choice which declaration of **all** your domains will use.

**The merged SPF record would look like this:**

_**v=spf1 a mx include:spf.protection.outlook.com include:\_spf.mlsend.com ~all**_
