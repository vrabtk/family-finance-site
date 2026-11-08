# Family Finance: public pages (privacy policy, delete account)

Google Play needs two public web addresses: a **privacy policy** and an **account deletion** page. These files are plain HTML, no build step.

## Before publishing
1. Contact email is already filled in (a.harikrishna108@gmail.com). Change it in the three .html files if you ever want another address.
2. Check the text matches what the app really does (see "Keep it true" below).

## Publish free on GitHub Pages
1. Create a new **public** GitHub repository, for example `family-finance-site`. Put only these files in it (no secrets: everything is world-readable).
2. Repo **Settings > Pages > Build and deployment**: Source "Deploy from a branch", Branch `main`, folder `/ (root)`. Save.
3. After a minute the pages are at `https://<your-user>.github.io/family-finance-site/`:
   - privacy policy: `.../privacy.html`
   - delete account: `.../delete-account.html`
4. Enter those two addresses in the Play Console (App content > Privacy policy, and Data safety > account deletion).

## Keep it true
Google compares these pages with the app's Data safety answers. Update the pages **before** a release that:
- adds analytics, crash reporting, ads, or any third-party SDK,
- collects new data (location, photos, notifications, contacts),
- changes where data is hosted or how long backups are kept.

This text is a plain-language draft, not legal advice.
