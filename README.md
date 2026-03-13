# Nagish — AppsFlyer Smart Script

This repository contains the AppsFlyer Smart Script used for marketing attribution on the Nagish website. The script was previously hosted on Slater (`slater.app/4870/8766`) and has been migrated here for version control and self-hosting.

## Script

### `appsflyer.js`

This is the complete AppsFlyer Smart Script (Build 2.7.3). It handles attribution, event tracking, and deep linking for Nagish marketing campaigns.

## Integration in Webflow

This script should be loaded in the **Global Body** custom code section of your Webflow project (before the closing `</body>` tag). Replace the old Slater loader with the new jsDelivr CDN URL:

**New Script Tag:**
```html
<script src="https://cdn.jsdelivr.net/gh/Kunsho85/nagish-appsflyer/appsflyer.js"></script>
```

**Old Script Tag (to be removed):**
```html
<!--🤙 JS: Slater.app/4870/8766-->
<script>var v="1.0";document.addEventListener("DOMContentLoaded", function() { ... })</script>
```

```

This ensures the script is loaded on all pages of the Nagish website.
