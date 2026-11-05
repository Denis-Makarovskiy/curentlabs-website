# Open Curent Labs LLC — GitHub Pages

Static one-page site, ready for a repository named `curentlabs-website` in the GitHub account `Denis-Makarovskiy`. No build step or dependencies.

## Publish a preview

1. Create a **public** repository `curentlabs-website`. Upload these files at the repository root on the `main` branch.
2. In **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
3. The preview URL will be `https://denis-makarovskiy.github.io/curentlabs-website/` once deployment completes. Relative asset paths work at this project URL and later at the custom domain.

## Connect curentlabs.com later

In **Settings → Pages → Custom domain**, enter `curentlabs.com` and save. GitHub will create a `CNAME` file for branch publishing. At the DNS provider, configure four `A` records for `@`: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`; configure `www` as a `CNAME` pointing directly to `denis-makarovskiy.github.io` (without a repository path). Remove any old conflicting A/CNAME records for these hosts. After DNS and certificate provisioning, enable **Enforce HTTPS** in Pages. Preserve existing MX records if email will be configured.

## Contacts

The public page displays “Coming soon” for email and phone because neither was supplied. Set verified public values in the `CONTACT` object in `script.js`; links will be created automatically.

The artwork and mark are SVG files in `assets/`.
