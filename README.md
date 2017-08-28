# cozy-usetracker

Activate cozycloud's piwik in your Cozy application.

## Install
fetch the cozy_usetracker.js script and add it to your app.

## Use

Then call it at the begining of your app :
```javascript

cozyUseTracker()
.then(() => cozy.bar.init({ ... })) // avoid cozy-bar complaining about missing Piwik.

```

##  What does it do?

1. Check for user activation or desactivation of usetracker.
1. Initialize piwik settings, with current appName, and cozycloud's piwik settings.
2. Load cozy's piwik script.
3. _onLoad_, resolve the promise.
