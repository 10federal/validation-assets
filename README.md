# validation-assets

Public host for **validation screenshots and recordings** referenced **inline** from issues/PRs in the private [`10federal/10Fed-Storage-Website`](https://github.com/10federal/10Fed-Storage-Website) repo.

## Why this repo exists

GitHub renders inline images in markdown through its **camo** image proxy, which fetches the bytes **server-side and anonymously**. A `raw.githubusercontent.com` URL from a *private* repo therefore 404s in camo (no auth) and shows as a broken image — even for members. The only ways to get inline media in a private repo's issues are the drag-drop `user-attachments` flow (browser-session only, not scriptable) or hosting on a **public** URL camo can reach. This repo is that public host: `gh` pushes here, and the private repo's comments embed `![](https://raw.githubusercontent.com/10federal/validation-assets/main/validation/<issue>/<file>)`.

## Rules

- **Public-site content only.** These assets are world-readable. Only commit screenshots/clips of the public marketing site (footer, search, OG cards, public pages).
- **Never** commit anything showing the Payload admin, customer/tenant PII, credentials, internal dashboards, or non-public data.

## Layout

```
validation/<issue-number>/<file>
```

e.g. `validation/334/recenter-demo.mp4`, `validation/415/2-mobile-nav-48px.png`.
