# VociApp Support Site

Static public support website for VociApp.

Purpose:

- App Store support URL
- App Store privacy policy URL
- Google Play privacy policy URL
- Google Play account/data deletion URL
- public AI, data, support, and legal information

Pages:

- `index.html`
- `support.html`
- `privacy-policy.html`
- `terms.html`
- `account-deletion.html`
- `ai-and-data.html`
- `store-disclosures.html`
- `404.html`
- `styles.css`
- `.well-known/apple-app-site-association.sample.json`

Support contact currently used in the site:

- `vociapp.support@gmail.com`

Before publishing, verify this mailbox exists and is monitored.

Policy references used while drafting:

- Apple App Privacy Details: https://developer.apple.com/app-store/app-privacy-details/
- Apple App Review Guidelines, Privacy section: https://developer.apple.com/app-store/review/guidelines/
- Google Play User Data policy: https://support.google.com/googleplay/android-developer/answer/10144311
- Google Play Data safety form guidance: https://support.google.com/googleplay/android-developer/answer/10787469
- Google Play account deletion requirements: https://support.google.com/googleplay/android-developer/answer/13327111
- Google Play AI-Generated Content policy: https://support.google.com/googleplay/android-developer/answer/14094294
- Google Play Payments policy: https://support.google.com/googleplay/android-developer/answer/10281818

Worldwide readiness notes:

- The site now includes regional privacy language for EEA/UK/Swiss, California/US state privacy rights, Brazil/similar jurisdictions, minors, international processing, and a Store Disclosure Checklist.
- Before worldwide launch, verify whether the App Store / Google Play listing developer name, seller address, and support contact exactly match the public policy pages and console metadata.
- Consider legal review before launch in highly regulated regions or before adding additional SDKs, analytics, ads, social login, payments, or child-directed positioning.

Local preview:

```sh
cd /Users/schmitdo/Development/flutter/VociApp-support
python3 -m http.server 8000
```

Then open:

- `http://localhost:8000`

Deployment:

- Intended GitHub repository: `git@github.com:client23/VociApp-support.git`
- GitHub Pages can serve this repo from the default branch root.

Notes:

- The site is written as static HTML/CSS to keep hosting simple and privacy-safe.
- No analytics, cookies, forms, or third-party scripts are embedded.
- `account-deletion.html` is designed to satisfy Google Play's external account deletion web resource requirement, but the in-app deletion path still needs to exist in the app itself for full compliance.
