**Set up your Chrome browser to automatically redirect to Smile.Amazon.com so that your purchases contribue a small amount to charity**


<br />

**Step 1** - Install the Chrome extension "Custom JavaScript for websites"
https://chrome.google.com/webstore/detail/custom-javascript-for-web/poakhlngfciodnhlhhgnaaelnpjljija

**Step 2** - Navigate to Amazon.com

**Step 3** - Click on cjs in the extensions bar and add the following script

```
var currentUrl = window.location.href
var newUrl = currentUrl.replace("amazon.com", "smile.amazon.com");
if(!currentUrl.includes("smile.")) {
    newUrl = newUrl.replace("www.", "");
    window.location = newUrl;
}
```
