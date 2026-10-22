# INCCM App Privacy Policy

The privacy policy for the INCCM App (Google Play: `rocks.uxi.inccm`), published with GitHub Pages.

- `index.html` is the policy page.
- `delete-account/index.html` explains how to delete an account (in the App, or by email without it) and what is deleted or kept. It is the **Delete account URL** Google Play asks for, and the policy's "Deleting your account" section links to it.
- `assets/` has the shared stylesheet (`site.css`), the logo and icons. The pages use system fonts only, no scripts, and no third-party requests.
- `.nojekyll` makes GitHub Pages serve the files as they are.

## Publishing

1. Push this folder to a GitHub repository, for example `inc-cm-privacy-policy`:

   ```sh
   git init -b main
   git add .
   git commit -m "Add INCCM App privacy policy"
   git remote add origin git@github.com:<owner>/inc-cm-privacy-policy.git
   git push -u origin main
   ```

2. In the repository, open **Settings → Pages**, set **Source** to *Deploy from a branch*, choose `main` and `/ (root)`, and save.
3. After a minute or two, the policy is live at `https://<owner>.github.io/inc-cm-privacy-policy/`.

Use that URL in the Google Play Console (**Policy and programs → App content → Privacy policy**), App Store Connect, and the app's Settings → Privacy & Security.

For the Play Console's **Data safety → Data deletion → Delete account URL**, use `https://<owner>.github.io/inc-cm-privacy-policy/delete-account/`.

## Updating

Change the policy whenever the app starts collecting new information or using it differently (for example accounts, Parent Mode, analytics or push notifications). Update the effective date in two places in `index.html`: the header `<time>` and the footer.

When the app's account deletion changes (where it is in the app, or what the server deletes), update `delete-account/index.html` and its date (header `<time>` and footer) too.
