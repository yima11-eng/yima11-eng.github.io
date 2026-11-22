# Yima website

Static pages for the store listings and AdMob: home, Privacy Policy, Terms of Service and `app-ads.txt`.
Made by `python3 tool/make_website.py` from `PRIVACY_POLICY.txt` / `TERMS_OF_SERVICE.txt` (edit those, not the HTML).

Before uploading:
1. Once the app is on the App Store, set `APP_STORE_URL` in `tool/make_website.py` and run the script again
   (`PUBLISHER_ID` is set: pub-5445072695739642).

Live at https://yima11-eng.github.io (GitHub repository yima11-eng/yima11-eng.github.io; upload changed files there).
Host it free on GitHub Pages, Firebase Hosting or Netlify. `app-ads.txt` must be at the root of the domain, e.g.
`https://yima.app/app-ads.txt` (not in a sub-folder). Then:
- enter the same domain as "Developer website" in Google Play Console and App Store Connect,
- put the Privacy Policy URL (`…/privacy.html`) in both stores,
- update the links in `lib/core/config/flavor_config.dart` (`termsUrl`, `privacyUrl`, `websiteUrl`, `appStoreUrl`).
