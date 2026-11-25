# AeroFarm website

Upload these to the AeroFarm GitHub repository (replace the old files), keeping the same names
so the QR link keeps working:

- index.html            (updated: install button, iOS add-to-home sheet, directions button)
- assets/               (unchanged)
- manifest.webmanifest  (new)
- sw.js                 (new)
- icon-192.png          (new)
- icon-512.png          (new)
- icon-maskable-512.png (new)
- apple-touch-icon.png  (new)

All four new icons, sw.js and manifest.webmanifest must sit in the SAME folder as index.html.

## Installing as an app
The site is a PWA. Over https (GitHub Pages is https) Chrome and Edge show an "Install app"
button in the header, and Android offers "Add to home screen". On iPhone/iPad the button opens
a short sheet explaining Share -> Add to Home Screen, which is the only way Safari allows.
Rotation is free (portrait and landscape) because the manifest sets no orientation.

If you ever replace index.html and an installed app still shows the old page, open it once with
an internet connection: pages are fetched from the network first and only fall back to the cache
when offline.

## Location
The footer "Directions to AeroFarm" button opens Google Maps directions to 31.2670589, 30.1713273
(Al-Maadiya, Idku, Beheira).
