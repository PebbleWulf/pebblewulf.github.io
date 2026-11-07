# Pebblewulff site (GitHub Pages)

## Fill in before publishing
- `index.html`: `[GAME NAME]`, game blurb, `[CONTACT EMAIL]`, Play Store link once live
- `privacy.html`: `[DATE]`, `[CONTACT EMAIL]`. Re-check it if you add analytics, in-app purchases or accounts.
- `app-ads.txt`: your AdMob publisher ID (AdMob ▸ Settings ▸ Account information, e.g. `pub-1234567890123456`)

## Publish
1. Create a public repo named `<your-github-username>.github.io`
2. Upload these files to the repo root (README optional)
3. Settings ▸ Pages ▸ Source: deploy from branch `main`, folder `/ (root)`
4. Live at `https://<your-github-username>.github.io/`

## Custom domain (pebblewulff.com / .com.au)
1. Settings ▸ Pages ▸ Custom domain ▸ enter the domain (GitHub adds a `CNAME` file)
2. At your registrar, point the apex domain at GitHub's A records and `www` at `<username>.github.io` via CNAME
   (current IPs are in GitHub's "Managing a custom domain for your GitHub Pages site" docs)
3. Tick **Enforce HTTPS** once the certificate is issued

## Play Console / AdMob
- Privacy policy URL: `https://<domain>/privacy.html`
- Developer website in your store listing: `https://<domain>/`. AdMob looks for `app-ads.txt` at the root of this exact domain.
- `app-ads.txt` must be at the domain root, e.g. `https://pebblewulff.com/app-ads.txt`
