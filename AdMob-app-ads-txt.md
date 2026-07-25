# AdMob app-ads.txt verification

Your `app-ads.txt` line (required by AdMob):

```txt
google.com, pub-5043317693312133, DIRECT, f08c47fec0942fa0
```

Live file in this repo:

https://soheltanvir0699.github.io/Universe-of-Alien-Support/app-ads.txt

## Why AdMob says “details don't match”

AdMob does **not** only check the file text. It also checks that the
**developer website on the App Store** matches the domain that hosts
`app-ads.txt` at the **site root**.

Preferred setup for GitHub Pages:

1. Host `app-ads.txt` at the **user root**:
   `https://soheltanvir0699.github.io/app-ads.txt`
   (repo named `soheltanvir0699.github.io`, file in the root — not inside a project folder)

2. In **App Store Connect** → your app → **App Store** version / product page →
   **Marketing URL** set exactly to:
   `https://soheltanvir0699.github.io`
   (no path, no trailing project name)

3. Support URL can stay:
   `https://soheltanvir0699.github.io/Universe-of-Alien-Support/`

4. Wait up to **24 hours**, then in AdMob click **Check for updates**.

## Do not use only the project URL as Marketing URL

If Marketing URL is:

`https://soheltanvir0699.github.io/Universe-of-Alien-Support`

AdMob often looks for:

`https://soheltanvir0699.github.io/app-ads.txt`

and reports a mismatch even when the project path file is correct.

## Checklist

- [ ] `https://soheltanvir0699.github.io/app-ads.txt` opens and shows the Google line above
- [ ] App Store **Marketing URL** = `https://soheltanvir0699.github.io`
- [ ] App is linked to the correct App Store listing in AdMob
- [ ] Clicked **Check for updates** after publishing
- [ ] Waited (can take hours, sometimes up to 24h)
