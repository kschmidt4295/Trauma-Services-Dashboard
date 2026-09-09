# Trauma Services Dashboard

Interactive revenue and paid-media dashboard for Trauma Services, Scene Clean MN, and Georgia Clean. Prepared by elk.

The dashboard is a single self-contained file: `index.html`. All the data is inside it, so there is nothing else to install or connect. It does load a chart library and font from the internet, so viewers need to be online.

---

## 1. Publish it on GitHub Pages

1. On GitHub, click **New repository**. Name it (for example `trauma-dashboard`) and click **Create repository**.
2. On the repo page, click **Add file → Upload files**. Drag in `index.html` (and this `README.md` if you like). Click **Commit changes**.
3. Go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, set the branch to **main** and the folder to **/ (root)**, then **Save**.
5. Wait about a minute. Your live link appears at the top of that Pages screen, in the form:
   `https://<your-username>.github.io/trauma-dashboard/`
6. Share that link.

---

## 2. Update it later

You do not lose the ability to change it. Two cases:

- **New data exports:** send the new export files to elk, get back an updated `index.html`, then in the repo click **Add file → Upload files**, drop in the new `index.html` (it replaces the old one), and **Commit changes**. The site redeploys at the same link in about a minute. No need to reshare the link.
- **Design or feature changes:** same loop. elk edits the dashboard and hands you a new `index.html`; you commit it.

---

## 3. Share specific views with clients

Add parameters to the end of your link to control what a viewer sees.

**Account** (locks the view to one brand and hides the account switcher):
- All accounts: `?account=all`
- Trauma Services: `?account=trauma-services`
- Georgia Clean: `?account=georgia-clean`
- Scene Clean MN: `?account=scene-clean-mn`

**Client mode** (add `&view=client`): hides the internal sections (paid spend, MER, goal pacing, AdNexus), leaving a clean client-facing view.

**Data set** (add `&dataset=all`): opens on All jobs instead of Internet-sourced.

### Examples
- Georgia Clean, client-facing:
  `https://<your-username>.github.io/trauma-dashboard/?account=georgia-clean&view=client`
- Scene Clean MN, client-facing:
  `https://<your-username>.github.io/trauma-dashboard/?account=scene-clean-mn&view=client`
- Internal, all accounts (default): just the plain link.

Employees open the plain link and can switch every filter freely. Each client gets their scoped link.

---

## 4. Privacy note

Free GitHub Pages is **public**: anyone with the link can open the site, and because free Pages must come from a **public repo**, the `index.html` (which contains revenue and ad-spend numbers) is also viewable in the repository itself. For sharing scoped client views this is usually fine, but if you do not want the raw numbers publicly discoverable, either keep the links private/unguessable, upgrade to GitHub Pro (private repo with Pages), or host somewhere with password protection.
