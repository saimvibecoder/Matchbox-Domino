MATCHBOX CASCADE: web app
=========================

This folder is the whole game. Put it on any web host and share the link.
It installs like an app (home screen icon, full screen) and works offline
after the first visit.

FASTEST WAY TO GO LIVE (about 1 minute, free)
1. Unzip this file so you have the "webapp" folder.
2. Open https://app.netlify.com/drop in your browser.
3. Drag the whole "webapp" folder onto the page.
4. Netlify gives you a link like https://something.netlify.app. Share it.
   (Create a free account to keep the site and rename the link.)

USING VERCEL INSTEAD
1. Put the folder in a GitHub repo (or run "npx vercel" inside the folder).
2. Import it at https://vercel.com/new. No build settings are needed.

ONE SMALL STEP AFTER IT'S LIVE
So the preview image shows when the link is shared on WhatsApp, Facebook
and X, open index.html, find this line:
  <meta property="og:image" content="og-image.png">
and replace og-image.png with your full link, for example:
  <meta property="og:image" content="https://your-site.netlify.app/og-image.png">
then upload the folder again.

INSTALLING ON A PHONE
- Android (Chrome): tap "Install the app" on the main menu, or use the
  browser menu > Install app.
- iPhone (Safari): tap Share > Add to Home Screen.

GOOD TO KNOW
- Each player's sparks, matchboxes and best scores are saved on their own
  device and browser.
- When you upload a new version, players get it the next time they open
  the game with internet on.

FILES
index.html             the game
manifest.webmanifest   app name, icon and colours
sw.js                  offline support
icon-*.png, apple-touch-icon.png, favicon.png   app icons
og-image.png           link preview picture
